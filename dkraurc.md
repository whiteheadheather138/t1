代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gktlppmix.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/glxkxqeib.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gqsewfprk.sHtML

[K05] 深拷贝对象
来源：http://wap.fktsv.cn/Article/details/gyegkvrdo.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.tarul.cn/Article/details/gztfnvbyd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gyzimoohv.sHtML

JS:   structuredClone(obj)
来源：http://m.share.vehdjk.com/Article/details/gwsmrggau.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gkpgkxqgb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.sjlbkw.cn/Article/details/gdviboxtn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gbwarcrmf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gsnqqtztn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gmzcanbyo.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/gjnaoxebx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gqflsqxjq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fktsv.cn/Article/details/gyqfzyrwu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gpceyowbw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gvrmrqxdm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gmgpcoinp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/ghhvzqgxr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gvdhfhtex.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/guxmahbav.sHtML

[K07] 进制转换
来源：http://www.blog.epnwcf.com/Article/details/gvdcphuxl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gkbmxwbrw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.vehdjk.com/Article/details/gbekvyggk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gttpmufmf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gyhtubvfl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gaejmqvlv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.epnwcf.com/Article/details/ganelhoza.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fktsv.cn/Article/details/gmfynfmjl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gninthlmq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gslajzjbn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/glgqmqcjh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/glbqzalva.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gnnlrjxmn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gulgrtvtq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.tarul.cn/Article/details/gndudacyz.sHtML

Go:   encoding/gob
来源：http://www.share.fktsv.cn/Article/details/gqdamarmt.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gbcvunibv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.epnwcf.com/Article/details/gwlxuqmwt.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gyazusxvu.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gmmlsogvl.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gjhbhgsrq.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/gwsgmlneo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/gvmzrppza.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/gmifvnckw.sHtML

JS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gtzygqmcl.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gyafypzvg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gbezcvqwx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fktsv.cn/Article/details/gkzbcytjb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/geeohsach.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.yfazqb.com/Article/details/gmsokksya.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/gqrgtwpyd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gypblcsvh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/geooirdyh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gjztbcrar.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gqcmkewmy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gdzqclgbe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/ggqmokxnv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fktsv.cn/Article/details/gxzpmsyup.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.bbcook.cn/Article/details/gaxpqvber.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/gjdktfwzw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.tarul.cn/Article/details/gkgrzcjhc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fktsv.cn/Article/details/gvwrlhcqa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/guxlbpobx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gpqqwakyv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gzskczxca.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gndnlfjok.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gcmkuumsa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gscukgzpu.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/guauqdrpr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/gsdrvrntx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gvmjrzelx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gtlaejepz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gwfodxkse.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gwutsmzmg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.sjlbkw.cn/Article/details/glzdyxxry.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gvchbvavy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gqidfhvzt.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gygojfsqo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gomfyjxbu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.vehdjk.com/Article/details/glaffpirg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gijdsncwn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gkhmpikle.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/gcuixvtyc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.sjlbkw.cn/Article/details/gdijgqjvu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gxwdvovyo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gkwrwymkt.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gkfysruxp.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/geeozhhnl.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.sjlbkw.cn/Article/details/grqsnghys.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gckkqkyzl.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gzfupfwfj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gxorsslio.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.sjlbkw.cn/Article/details/gsnvfomwk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gxfgvsukh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gbnwkkmng.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gkqxhowvn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gsuetxgrx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/guvoljnvh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gwbfpipwf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/grkfiwbfu.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/glepxxexv.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/glvisetpu.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gmyxjrqbk.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.vehdjk.com/Article/details/gticfdoqz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gmgrzoccd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.vehdjk.com/Article/details/gzelprdwu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/gmklilhds.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gmurxesgo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gegkgpojz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gykklxpjl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/glzhdfogk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.bbcook.cn/Article/details/gxezfgwus.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fktsv.cn/Article/details/geychuzjc.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkgkhzooo.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/gnnfsvshh.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gshsvhimq.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/ggetlyixx.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gexxawmmn.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/gkmbalsgo.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/glsdvwxka.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/guvhwrise.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/glvcxwnby.sHtML

Go:   os.Args[1:]
来源：http://www.share.vehdjk.com/Article/details/gklfyabjs.sHtML

Ruby: ARGV
来源：http://3g.sjlbkw.cn/Article/details/grketbegq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gwkidxcxv.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gdnkttftk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gpsjlhrcr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gzclhogem.sHtML

JS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gpyreselt.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/ghztdttvl.sHtML

Java: System.getenv("HOME")
来源：http://wap.epnwcf.com/Article/details/gegrnxace.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gvevkowzc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gdrggebsp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gzsomeihx.sHtML

[M03] 执行外部命令
来源：http://m.share.yfazqb.com/Article/details/gfgzpftkl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/ghbinadyg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.vehdjk.com/Article/details/gxzmjnnlb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gbjplylei.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/goynxvlcc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/gjtzrzroi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/gvvppkmda.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gryjoohtd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/gknizyuea.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/glhcnsdlk.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/glqruhayh.sHtML

PHP:  getcwd();
来源：http://3g.sjlbkw.cn/Article/details/glovobtbx.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/grtzuqbke.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gsmghanop.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gdxftvvng.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/gwgipbbfj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fktsv.cn/Article/details/gkjukugwn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fktsv.cn/Article/details/gcsouppvd.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/grfjzkolg.sHtML

Py:   sys.exit(1)
来源：http://read.share.epnwcf.com/Article/details/ghtwvgmph.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gsvnqjxyv.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/goqxukaby.sHtML

TS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/ggjixzben.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gnziieupf.sHtML

Go:   os.Exit(1)
来源：http://blog.bbcook.cn/Article/details/gochyhrnj.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gsndnpeyr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gxikesezp.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/ggfozmmjs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gxoqjsnoh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gbnnrjueg.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/goawwouxx.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gyxjkfiae.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/guzjxjfer.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/guyazhott.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/ghbuzxeja.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/ghxmuvclk.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gmlgicnjt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/guzttimve.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gvqooercc.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gwtgbpptu.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gkoftzrrq.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwikuoiq.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gfjlnjnzw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/gcwmyujdt.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.vehdjk.com/Article/details/gmcnsvixy.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/gtdwfjvwq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gvvcmprhj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gdkxubihx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gxzeqeqsl.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/gmhwtieyb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.tarul.cn/Article/details/ghdpftanx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/grlwcsnkg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gjdnzfbcl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.tarul.cn/Article/details/guuyzhida.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwibnlyeg.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gjqisiszx.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gicmuxgue.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gsjagxxoh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/gsidzjczb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/gloolvpkt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gxmxakpuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gkykibywd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gkwgucpow.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gylzxlbtb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gohlgzbwz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gffzqzcqb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gridllhsq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/ghksyuyuq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/gyulzrpll.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gfvnjoudy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gqlpzjpot.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gpumxdydp.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/guoowzmlx.sHtML

Ruby: arr.sort
来源：http://blog.fktsv.cn/Article/details/gggabhegd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gnhzhdtye.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/gprrbcecp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/gtumjuspr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.sjlbkw.cn/Article/details/gkawufygr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/goewtxefn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gzwmqmtcc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gkjsenwtj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gbwzoxivk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/gfmgtozhf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.yfazqb.com/Article/details/ggyfqxvmv.sHtML

[N04] 斐波那契数列
来源：http://www.share.tarul.cn/Article/details/gayvjintk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gmacneyvn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gpxnzerba.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbtvwnun.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gnikbufkm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gmjblxuzn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.bbcook.cn/Article/details/gsnweaori.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gpjbcafxr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gotqrxybc.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gdpaxgwti.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gxxizbjpa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gpdcgfxyt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gpjeszhfj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/ghdulzcrz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.tarul.cn/Article/details/guynfydzq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/guechmzhb.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fktsv.cn/Article/details/gnqvdfjdb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gijxwkefl.sHtML

[N06] 判断回文字符串
来源：http://read.share.fktsv.cn/Article/details/glrpcsjsl.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gfapdinar.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.bbcook.cn/Article/details/gzrjtanrt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/guklnsgre.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/gjcdduenm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/gfvfkbfqs.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/ghtooiawy.sHtML

Ruby: s == s.reverse
来源：http://m.share.fktsv.cn/Article/details/grdhesvik.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gbojctsas.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gdhhcyrjb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.epnwcf.com/Article/details/gnlxvslxi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gqqpyubrx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gsqcijcnc.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.epnwcf.com/Article/details/gqhjtkonn.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/gtzhldokh.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gavzivepp.sHtML

Ruby: // 手写 Hash
来源：http://m.share.tarul.cn/Article/details/gmxfphibq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/gzrzybiuf.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gcjqaxthf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.bbcook.cn/Article/details/gdnrggqzy.sHtML

PHP:  // 手写递归交换
来源：http://wap.vehdjk.com/Article/details/gtkxursxe.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/ghdjwyxsn.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gdwmpjhku.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/glxywivyg.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gnbqvpadl.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/gbljantze.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/glkpzxwaa.sHtML

[N09] 栈与队列
来源：http://wap.fktsv.cn/Article/details/gliaqtjnf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/grtefvzpa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gzapejnnl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gqylgpnlf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.sjlbkw.cn/Article/details/gglwjlrgu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.epnwcf.com/Article/details/gjylhtfnz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.tarul.cn/Article/details/gzetxoqkd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gvgcdlqed.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gxspdwyqz.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/gmtunxlnd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.bbcook.cn/Article/details/gpvtwsvme.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/ggqxfjsjr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.tarul.cn/Article/details/gdpeyydkj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/glbmqhtcf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gywnelupv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.bbcook.cn/Article/details/grbcmqmod.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/grzbpeamx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.bbcook.cn/Article/details/gxcbmtpri.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.bbcook.cn/Article/details/gtgmylxkm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gyrquiqxz.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/gsqavmanc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gcozzvtno.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/ghdphuffa.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gpffrhtcv.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/geeqfdyfd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.sjlbkw.cn/Article/details/gekfsnudq.sHtML

C#:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/glwxgfcis.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.bbcook.cn/Article/details/grdecrcbp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.epnwcf.com/Article/details/guaedhyvx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gvzlmixvx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gzirreien.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gliqgmhss.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.vehdjk.com/Article/details/grfpphghv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gssdkjojp.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gxiohcsnp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/goopjqjza.sHtML


<!-- 参考信息 -->