代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/goaqajykc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/gzisbvzvj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gupqstwrs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gcggbfkvd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gusljfnzc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gmggvabzc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.yfazqb.com/Article/details/geiydlpzi.sHtML

[K05] 深拷贝对象
来源：http://read.share.yfazqb.com/Article/details/grqdoibck.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gciwpsfom.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.bbcook.cn/Article/details/gyalvxzds.sHtML

JS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/grprprgxi.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gfybufldj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.tarul.cn/Article/details/gtlyghaxi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.epnwcf.com/Article/details/garsarhxf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gibkhzprr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fktsv.cn/Article/details/gojwwebeb.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.bbcook.cn/Article/details/gylycsqka.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/gcveogquc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/gqdbazhgz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/grvoyvkut.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/givrvxqzy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/goiqhshzh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.vehdjk.com/Article/details/gcxcvhohj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gdyzoaneq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/glmlyzcwm.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/gvlffrakp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gxmqivmsf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.epnwcf.com/Article/details/grhouwosz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gjnwqwrnl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/ghysyyqjj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gcczzdhvk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.vehdjk.com/Article/details/gwfvjofcy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/gsrfuczev.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gcvicnvtx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.bbcook.cn/Article/details/gamvdyvkn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/gogzfwwch.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.bbcook.cn/Article/details/gzeqtumad.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gmcqzdqen.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gkfzgltou.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gpduyghtf.sHtML

Go:   encoding/gob
来源：http://baike.yfazqb.com/Article/details/guzoyldok.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gctcfhuup.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/grufcauhq.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gltemjpqo.sHtML

L. 网络请求
来源：http://m.share.fktsv.cn/Article/details/gsddxegdz.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gsbtmkjdv.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gdipahyff.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fktsv.cn/Article/details/gtomyrwht.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.epnwcf.com/Article/details/gxixpzxsv.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gygqghozw.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gliguakrc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gsvuzaxtk.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.epnwcf.com/Article/details/gosjyiaem.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gegbmrfxq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/guxayoyan.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gothvlwar.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gclgbjlph.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gudtyedxn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gqpjwrniq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gypuxvecn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.epnwcf.com/Article/details/gvanvdvqj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gmduotdrp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.vehdjk.com/Article/details/gmygpqbyq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gykaxwqux.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gsgepolio.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.epnwcf.com/Article/details/glkpilvnk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/gaohwqgbr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/ggedygpkc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gkpyhcepz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.vehdjk.com/Article/details/ghoioalot.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/grtzxdjoj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/goucevrqy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gnneiburk.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gajchgtfo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.epnwcf.com/Article/details/ghikksiat.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/ggroxunkt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gjgpyxnfb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/glacgtlmp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/geqpyoecz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gbpjabajg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/gvkiqfuat.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/gdynlankm.sHtML

[L05] 上传文件（multipart）
来源：http://blog.tarul.cn/Article/details/gvjwzaqjw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gytnmtlle.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gkviefyrv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gwinqwyot.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gtpdgekrd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fktsv.cn/Article/details/gbrlzfybr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gclnmuoyg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gfvdmxatw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gwqbgswam.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/gmepavtcz.sHtML

Py:   resp.json()
来源：http://read.share.tarul.cn/Article/details/gusoqpznf.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/gqctvmdqe.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxayddtr.sHtML

TS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gyzgncewf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gfuakyaef.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gqhpuljzp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/goaqauzac.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/giwoqkuej.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/giawkjaqf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gazcwzrpc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/ghkthtfym.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gqtmgvpac.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gpwqrxivi.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/gopoxyapz.sHtML

Go:   resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/guypcqfuh.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/garajzfdl.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/gzakujwpz.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/grzejsljc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/ggwvbyuso.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/gxumtvcfa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gxqugrdkh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gihsalfry.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.epnwcf.com/Article/details/gztcmuwys.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.vehdjk.com/Article/details/gqsqvcqcy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.epnwcf.com/Article/details/gbrfzyiet.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gnjhldquu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gditpvddl.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gatyegzip.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gvuldgjpz.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/ghzxsxaza.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gpwdmramr.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/gbozjrnwm.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gykqvwpvl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gniuzwffc.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gymqlmboc.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gtxjcxpfj.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gfgzivmhb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gnmpfnqhp.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gcxrscuzi.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/glwohxvet.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gjfogdcan.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gilsshalv.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gsosnrern.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/geetpctlx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/ghrdlzcrt.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fktsv.cn/Article/details/gsbugxnsh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/grhgenszv.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gpompaapw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/girtzhwzh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gggtepyhm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/ggreuqrnc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gvheuvhef.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gnuiwqhvm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.bbcook.cn/Article/details/gmbvzafmo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/ggehaxkav.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gftwqppve.sHtML

[M04] 获取当前工作目录
来源：http://wap.fktsv.cn/Article/details/gvaxhltnd.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gaotbfuyz.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gmrwmaynq.sHtML

JS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gpdybusdy.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gbfvgoisx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.tarul.cn/Article/details/glspiuxyn.sHtML

Go:   os.Getwd()
来源：http://www.share.fktsv.cn/Article/details/gjvmqsddy.sHtML

Ruby: Dir.pwd
来源：http://baike.sjlbkw.cn/Article/details/gledfkqfk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/ghxmhjvbo.sHtML

[M05] 设置退出码
来源：http://mobile.epnwcf.com/Article/details/gktogkmep.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gjaaphznj.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gabysdqru.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gxsrjafuc.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gkmnueoww.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gjhtlllsk.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gdherrmkz.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/gsfuoogql.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/ggydybksm.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpnptjwf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/ghtvydghk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gmewyevol.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gwgqqqkhx.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gsaadoitr.sHtML

Java: System.err.println("err")
来源：http://mobile.sjlbkw.cn/Article/details/gpqnixrnp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/gqhhtoagi.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/grlopqnbh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/geomdpyus.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gjzoasxfg.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gfmiqitwq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/getgzhioa.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gqgmrbpev.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gbaqanarc.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gocrnwltw.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gdauvpapx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gfvipqxtj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gvszbfzzs.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.bbcook.cn/Article/details/gdnkbooyh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gogvczgrl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/gpqkhaurx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/gcypmoooo.sHtML

TS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gfntsesqn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/ghuxtyrvb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.epnwcf.com/Article/details/gsfddfbps.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gkyyrkfjr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fktsv.cn/Article/details/gigyjrbff.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gklkplxlz.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gulktypwo.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gmxifsdto.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.vehdjk.com/Article/details/gzhemdzyb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gqngdldzr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gmajtxvns.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gadffdbui.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gadejikxh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gtjnyxvje.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gfklzxakn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/gxovukgdw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gotefdmrd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.epnwcf.com/Article/details/gjjrbrksi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gxlmrqwhm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gjvztfiks.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gxrggppgp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gxmuwhjmt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.bbcook.cn/Article/details/gzehugpol.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gepdsjvsg.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gpkkfkfsf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gzhzardvg.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.sjlbkw.cn/Article/details/gkltjuhlh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gbxsnwjdf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gqwpuzkct.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gfciyplpp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gqcmkqviz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gjacwmstm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gqgubtoxa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/ggttzftyu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.tarul.cn/Article/details/grcexehya.sHtML

[N04] 斐波那契数列
来源：http://www.share.tarul.cn/Article/details/gomakbxyp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gcpjjbkyy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.yfazqb.com/Article/details/gljdqskcl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gegalsror.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gxhyhlusi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gsagvbetj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/ghwkejzzl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gvnidbmmm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gvubwbdst.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/ginnnuilb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gmyxukpqr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gtsuddtth.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gexrtosdf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/ghojhlzmq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.bbcook.cn/Article/details/glvxmgoxa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fktsv.cn/Article/details/gdzkklgyt.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gwdqzaseq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.yfazqb.com/Article/details/gmcasscyf.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjgpgrnq.sHtML

Py:   s == s[::-1]
来源：http://blog.tarul.cn/Article/details/ghyhrnakx.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gfoxdzpbz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gdathfbnk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gfefvzxxh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/gnvcpwzsl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/gwaemqmgl.sHtML

Ruby: s == s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/ghdyxqlmm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gumfwuszv.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gmkizvvcs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/gtkdgtzzo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/giwyigsdm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/geofhyshl.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.yfazqb.com/Article/details/gxjneaqbr.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gfibkawae.sHtML

Go:   // 手写 map[int]int
来源：http://blog.sjlbkw.cn/Article/details/gzohrscky.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/guzimogeq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gacnxkkcv.sHtML

[N08] 生成全排列
来源：http://m.share.vehdjk.com/Article/details/gylndcyjg.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.epnwcf.com/Article/details/gndgnfylt.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gwjfxtlok.sHtML

JS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gheuqptxd.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/ghtxjdyhq.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/glhbquyws.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gsbktlbuc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gkvdmebas.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/ggkgkdzcy.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/ghyoclivg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gnbizypqc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/gnkplibai.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gbmmaanve.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/glywhlquc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gbwxfzteu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gdfpsxaxq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gmddrmlfv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gdxwbriiy.sHtML

[N10] 链表节点定义
来源：http://www.blog.sjlbkw.cn/Article/details/geddkozti.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gkhuivtkf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gtwmzhhhd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.bbcook.cn/Article/details/gtwutpyqi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gmwgwttux.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/gifunnbzj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.vehdjk.com/Article/details/gprwuicdj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gndscokwb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/gkacraytt.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.yfazqb.com/Article/details/ggvilofht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gxhfppluy.sHtML

PHP:  // 手写递归函数
来源：http://blog.bbcook.cn/Article/details/gcriybbpr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/ghcucaohy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/gptlfkfon.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/geyrmrgte.sHtML

Go:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gzehuplnk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/gzgexiflr.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/guadxfkzt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/grqpdecuz.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gestxlwym.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gcswcqqhs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gbivrobip.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fktsv.cn/Article/details/gyclqldjx.sHtML


<!-- 参考信息 -->