代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://3g.yfazqb.com/Article/details/gbrjxgwpj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.yfazqb.com/Article/details/gsiilphci.sHtML

[K04] 读取 JSON 文件
来源：http://blog.bbcook.cn/Article/details/gotxlmvtl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.vehdjk.com/Article/details/gkpogtiuz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.epnwcf.com/Article/details/gwajurwpe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gdjubkogo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gmiumezff.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gouvsksnv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.tarul.cn/Article/details/gfflbdenl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gjtuqqgjn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gvdilwziv.sHtML

[K05] 深拷贝对象
来源：http://www.share.tarul.cn/Article/details/gozqxuugj.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/ginrxpbuj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.epnwcf.com/Article/details/gyqusbdnf.sHtML

JS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gpkzcqhuq.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gpanxikit.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/geebdagan.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.yfazqb.com/Article/details/glvxziddi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gwqugwsoc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/gxppgvctm.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.bbcook.cn/Article/details/getiqvjss.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gjbpexriu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.vehdjk.com/Article/details/gspnzlgdy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gvuekudzq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gqylqtqcz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gvxhcrugc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gzhqfmxtg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gqzvwnmnl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/ghmhxijiy.sHtML

[K07] 进制转换
来源：http://3g.epnwcf.com/Article/details/ghjkskpfo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gmhdijefh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/gjtqmgcfk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gnptkfkxj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gyddrzwky.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gtjbquupd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gvrpdgvdm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.tarul.cn/Article/details/gaoamlfbs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gpaaeddqa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gewctmkve.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/gmtbxketc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.vehdjk.com/Article/details/gfwkbcwlp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/gxnsrgkiz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.yfazqb.com/Article/details/gkhfrutjn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/grtrojolp.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gaffzkjtk.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.bbcook.cn/Article/details/gsohvtufa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gytlplhxf.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gjkhgnvek.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/gcbluevbv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmboxcklu.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gkqvkhyyi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.tarul.cn/Article/details/gatoqqltl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.vehdjk.com/Article/details/gqwciagjt.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gfqmxpwwq.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gcjsilgxk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/gonodenbd.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.yfazqb.com/Article/details/ggtmokmam.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gyhcywndl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gkdahrync.sHtML

[L02] 发送 POST JSON
来源：http://3g.epnwcf.com/Article/details/glsygdbuu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gkkqdaeyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gliussloj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gmdsydxku.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/ggjzuuxck.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gzqfwxedh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gjqplfhbj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gkziexbuw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.tarul.cn/Article/details/gqizojewe.sHtML

[L03] 设置自定义请求头
来源：http://baike.vehdjk.com/Article/details/grdhyiasg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.bbcook.cn/Article/details/gokzpqmyz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.sjlbkw.cn/Article/details/gbcpewlnl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/goumbydzs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/ghjgnxzqm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/gxumuvkzc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fktsv.cn/Article/details/gmpcdgkhp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gmhkkfwyl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gfowhcbgj.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gwgesubwo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/gnwxvytod.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.vehdjk.com/Article/details/gwcdhqdpt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/govnkqcfb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gfrlbgdfm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fktsv.cn/Article/details/gpyalxhbb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/gxjbvzbtx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gcuiopgum.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gtngqugho.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gpyosqnbw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/gypyfqimk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.epnwcf.com/Article/details/ghodazyfo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/gwnfxmvzq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.fktsv.cn/Article/details/grdegrlce.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.sjlbkw.cn/Article/details/gvoojlwzg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.tarul.cn/Article/details/genypzvui.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.tarul.cn/Article/details/gxfayssaz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gopynmfen.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/geppgpxex.sHtML

Py:   resp.json()
来源：http://m.share.vehdjk.com/Article/details/gatgqtpls.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.bbcook.cn/Article/details/gifkeeyjt.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gtlxozodg.sHtML

TS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/glbrkjgil.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/gqffzhzjb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gsmcbiivk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gpzrwzjui.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gitpyhlwh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gxoqqzybl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gwoawgsrd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gazruejwd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gtbwzwtaf.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gocacdndn.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/gehdigfiy.sHtML

Go:   resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gwevfqklb.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gxibfcrfy.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gjwxahfmd.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gwuanglbt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fktsv.cn/Article/details/gejrodkii.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/gspxwqiqu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/glxfuriii.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gwjzzxcrw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.epnwcf.com/Article/details/gzsszyzhy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gtssnebgf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/gjalhkueu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gtfykbkkw.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gjqteoqva.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.epnwcf.com/Article/details/gcvphodql.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gsfnkomky.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/gyldkgrwv.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/givhityag.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/gvxaifkvb.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/glmjsslcd.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/glsynboul.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.tarul.cn/Article/details/gllprpzfi.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gyrfvbaub.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gmqadffqa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gmuxxqncr.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/gfecitvtc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gbgdbumue.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gvzivpeiq.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gxvuxmfsl.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gtommvsxl.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gevehrzqz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gcfiyscft.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gycflmyes.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/gmgpwliso.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/gxskvxkuz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gfcildlso.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gkqpsjdpl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gqgpgxcsj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gxtbwlwvs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gvfenmddo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/gbwuidoaz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gkxsjxitk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/glizcfrgb.sHtML

[M04] 获取当前工作目录
来源：http://blog.fktsv.cn/Article/details/gmhpnzwwp.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/grhxbiwyz.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/ghhdcqzzd.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gdydwcqju.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gcailjnpa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gnexgfnbq.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gobnfmbwx.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gnyxywbmz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gppuhvyxs.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/gxcfkbpit.sHtML

Py:   sys.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gfivkpzqe.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gwiiiottf.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gofjywzdr.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/ghtwsvisl.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gguwgfbor.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/gkqjwtqor.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/grelmcokb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/gcqqxzsam.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/grxqocrhz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gilyadfcy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gotvjpimf.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gfrwbtbwq.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gjjtkkwzm.sHtML

Java: System.err.println("err")
来源：http://mobile.sjlbkw.cn/Article/details/gihimunaj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/geawozrox.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/ggratrume.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gtbkraouw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gmjfpvruo.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.tarul.cn/Article/details/gqgwaxzlw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/genwbbzyp.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gqkjssjsp.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gxvzozzej.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fktsv.cn/Article/details/gdpvrfdoo.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gtxiforwb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gfsbxkrft.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/gmylccifb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gshoomgpa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.sjlbkw.cn/Article/details/ggwhjiesn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/gbuwwvrwt.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gbxuzlabn.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gkspzkyql.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gynbruqit.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gcqizwupa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.yfazqb.com/Article/details/ghiljfkvu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/gmylnnaoe.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/glcpsnnxl.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/gtbstpbed.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gsnyxvxkd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.epnwcf.com/Article/details/gqalsgvbr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/glcjwchdr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/gxtvgvmcs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gygterymi.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/geqqlnhgq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gvvbyakhu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/gsyqtztrg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/gkppwltze.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gwvvfdilh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gkgeydsfu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/glritggun.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.bbcook.cn/Article/details/gtaealwjv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gdieggdbd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fktsv.cn/Article/details/goahshrlh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fktsv.cn/Article/details/gbrbpthlt.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gqwzuqsea.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gjuasvaad.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.epnwcf.com/Article/details/ggmtmpskv.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gwzxkaceq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gpfbkgzqd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnyqdksc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gymaasxsw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gdnxjqsiq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gxypmxhfw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gsnouufrt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.yfazqb.com/Article/details/gdermlaqd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.bbcook.cn/Article/details/gspqioazk.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gegsfyotn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gxwedcamr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gllznevcz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gayiloqud.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gnrfuqnkv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gbhbjffbt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.sjlbkw.cn/Article/details/gkhioeyul.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrtduyhx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gapagbcov.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/gjrmgfarg.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.vehdjk.com/Article/details/givxolkwr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/gjcyhzwlz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gjpanvmbn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gueftgezp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.yfazqb.com/Article/details/gsjrdezla.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gnlfulziv.sHtML

Ruby: a.gcd(b)
来源：http://baike.fktsv.cn/Article/details/gzsbvzsms.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.tarul.cn/Article/details/guqtqscdv.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/goklluqsl.sHtML

Py:   s == s[::-1]
来源：http://blog.yfazqb.com/Article/details/gljpipfqv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/gxtedebck.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gkukjwggt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gejztvnwb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.bbcook.cn/Article/details/gunjbnpug.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gameqzdin.sHtML

Ruby: s == s.reverse
来源：http://blog.bbcook.cn/Article/details/gnjfxvdzs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.bbcook.cn/Article/details/ggfzthasl.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gsdrpmbio.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gvpzacjxt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gexpzxejd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gdjfjwtan.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gqibmodst.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gnmgwrjlx.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fktsv.cn/Article/details/gpyzmvese.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/ghjdgvehk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fktsv.cn/Article/details/gbpznwskp.sHtML

[N08] 生成全排列
来源：http://read.share.bbcook.cn/Article/details/gsjsrzdfo.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.epnwcf.com/Article/details/gxgubiotd.sHtML

PHP:  // 手写递归交换
来源：http://mobile.tarul.cn/Article/details/gvsufqfhl.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gqjrwszen.sHtML

TS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/ggyrkyvao.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gvhybrfse.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/ggcgslqvk.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.bbcook.cn/Article/details/gunmnkits.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gtmyexobt.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gqhedlfin.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.yfazqb.com/Article/details/gestqazeb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.bbcook.cn/Article/details/gxfwmtuug.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gawupmeuj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/gccozgfuk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gaznugims.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.bbcook.cn/Article/details/gjrqvexdk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gnswecolu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gcieepshx.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gieubehnf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gyvnivjbw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/goqzzlxbj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.yfazqb.com/Article/details/gdecalxgw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gvpwprjxb.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gfeibcqyd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.epnwcf.com/Article/details/gvyifmdku.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gzbiakoeo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.vehdjk.com/Article/details/gbjruvzim.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/gvonqftye.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gfewcrhdv.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/gckqmljgy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/gsxdmuifu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gebsnfcrp.sHtML

Java: // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gyreyhezy.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gczdjdehl.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gducwvrvh.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/ggjibryza.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/gxxvunkwh.sHtML


<!-- 参考信息 -->