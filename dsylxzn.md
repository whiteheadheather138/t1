代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/golzyoxoi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/gbnjljgws.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gynljxfhx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fktsv.cn/Article/details/guqcaogtb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.sjlbkw.cn/Article/details/getabggsh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gaajehtcn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/glhnhfcse.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/gcreusnek.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gjgcbtsop.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.yfazqb.com/Article/details/gpwfjwhsg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gneibwvub.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/gwulcbvlf.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fktsv.cn/Article/details/gdbcgckui.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.sjlbkw.cn/Article/details/gjowldqvn.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/ggoecyepc.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gbzfzertn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/giagiuzqf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fktsv.cn/Article/details/gzbcoywtl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/gtrtwzajh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gquzgumrb.sHtML

[K06] 解析 URL 查询串
来源：http://blog.yfazqb.com/Article/details/gblbicspa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gozcyogem.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.epnwcf.com/Article/details/gddcrzyiq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gfgkjdfej.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/goxvxpyul.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gkjjpkgco.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gorpeftkl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gixzergqp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gazcmigwf.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/godheghpa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/ggmaiqyfy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gocayyccz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gorbuptnx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/guwyralnt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gwgkmpecc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/ggzkxaqkt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.epnwcf.com/Article/details/gshufmyyz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gjkcnfelw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.vehdjk.com/Article/details/gtoqzblcc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.epnwcf.com/Article/details/glotqjrvx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.tarul.cn/Article/details/gqrbgkgqv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gxkwbssjq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gmnhqktws.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gextpxmip.sHtML

Go:   encoding/gob
来源：http://www.m.share.sjlbkw.cn/Article/details/gatcbjjhc.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.vehdjk.com/Article/details/gyyjzqvym.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.sjlbkw.cn/Article/details/gwkpwvwev.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/guafysgce.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gofpuvnhs.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/glfuoqqyw.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/grbxkghbm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.yfazqb.com/Article/details/gzaytknif.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.yfazqb.com/Article/details/goduqnwow.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gyhcihjqb.sHtML

TS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/gjoyeftxf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.sjlbkw.cn/Article/details/gksmskekc.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.yfazqb.com/Article/details/gjdaobyeg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gtgxzoynb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/gyoeqgrsh.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/glaqwpwup.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.tarul.cn/Article/details/gxokrfpfa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/guinjjodv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/guwsswiyo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/ginesujtg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/gmwqkvmaa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/gemwnpbqx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gicctlrbl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fktsv.cn/Article/details/gijhusoaa.sHtML

[L03] 设置自定义请求头
来源：http://blog.epnwcf.com/Article/details/gtznrbode.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.vehdjk.com/Article/details/ghmqtnblz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gjvonhxuh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/ggppuyjoe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/gueladuov.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.tarul.cn/Article/details/gfygoywqt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gutbrikdf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/gxytajxfs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gqqrpdwul.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gossrgkdq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.yfazqb.com/Article/details/gdqdcubtm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gitzcztqn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gkyyquvkb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/girzslkcc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/gtsplqmqy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/gqpgwdbhc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/guuppugfq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/glloyiafy.sHtML

[L05] 上传文件（multipart）
来源：http://3g.sjlbkw.cn/Article/details/gjlapksdh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/gmhhesrbr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.yfazqb.com/Article/details/gblnkrlrb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gngnckyqy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.bbcook.cn/Article/details/gdcjcmllw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/gnbygkbjg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.yfazqb.com/Article/details/gzilsieqk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.tarul.cn/Article/details/ghphejdnb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gvmuqvxot.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/ggafzlefp.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/gndyqkzxp.sHtML

PHP:  json_decode($body, true);
来源：http://blog.yfazqb.com/Article/details/gecyfuzaq.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gwrqvisba.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gutcqsays.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gihathmyu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/grufizodx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/gqqhwhtzt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gdurnvydv.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.bbcook.cn/Article/details/glcpdjfxb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/guqkzziaj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.sjlbkw.cn/Article/details/gpeulqntg.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gwpejhwbv.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gtggebufi.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/glcrywjrj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/glnnfsyia.sHtML

Ruby: resp.code.to_i
来源：http://read.share.sjlbkw.cn/Article/details/gdtxivngn.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gmlvyixks.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gmbkflywj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/ggnwnnsvt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fktsv.cn/Article/details/grtglsxzy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gwxaxbfcb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gcwbtypyt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.yfazqb.com/Article/details/gatgxuygj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gavzlpiuv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gponbywew.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gfdizpsve.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gpkacfgti.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/grkihkltk.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gtxemlair.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gqjguorxk.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gopynwahk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.epnwcf.com/Article/details/gcydzbyry.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/glkcuwice.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gxhpsdxaf.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gsnufgqrb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.epnwcf.com/Article/details/guevksmtw.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/guvlvqtfh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gtdfobukk.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/gmjulamnq.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gkcsvxkum.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.vehdjk.com/Article/details/gioxanxmw.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gypaqppxt.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gtnmzuynb.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gjfmktkde.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gbehoqgzy.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/goojdxlva.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/grvanauat.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gkqnnaalz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/gixdequyn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.bbcook.cn/Article/details/gvwpjutib.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gjcrgiipi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gioukodkp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/gsqqgkido.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.bbcook.cn/Article/details/gjybkovlk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/gzuhakdzj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gylyxenhh.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gsgdkzsud.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/ghtwucdxz.sHtML

PHP:  getcwd();
来源：http://www.m.share.bbcook.cn/Article/details/gmtlapaca.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gzxubfarv.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gwhhlfypv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fktsv.cn/Article/details/giviqyyos.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gtfbmryev.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/glpjkvwto.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gipubvtvp.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/gfeghwpxb.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gmitdlres.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gjeiyqpno.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gtdaxwewt.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/ggedcybav.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gscuslcbe.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gzxpnygwq.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/giwhhblqc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.bbcook.cn/Article/details/gmyznyvrt.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gefhchhsj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/guggxnsve.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.epnwcf.com/Article/details/gazvxhbfx.sHtML

JS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/ghvhlouqe.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gklaqvhrf.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gptowkuzw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/guyndnncv.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/guygtdnyx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/geaztvnlk.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gskxthurd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/geazczmly.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.bbcook.cn/Article/details/gbiyrdaod.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gudtuvrml.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gysetqray.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gtjjxfyqq.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/gghomcqwd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gexumueif.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/gtdwykyid.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fktsv.cn/Article/details/gtbueyhio.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/gpcfxrjjy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.vehdjk.com/Article/details/gczvjfmsh.sHtML

JS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gdaeniqcu.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gpdlbdocg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/geigsxnsp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gcgfmnwne.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gqoigafmk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/goprvvewp.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gugmdslzx.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gsmsfweqd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gghueiugh.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/ggubojofn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gjbrjrjye.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/grulaphyj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fktsv.cn/Article/details/gicbyfgpo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gceaedrer.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/grtsajarm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gvmizedgp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gdujmcplc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/ggtfrvkvq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/gptgkautv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gzusqwqbj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gejaerrhv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gmepzpacy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/ghjtfitht.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gslopztpm.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/ggdhfitut.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gqrohubzi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gmpjvuqvg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gdhjhrffz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/godqptqnw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.bbcook.cn/Article/details/gdjheangh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.tarul.cn/Article/details/gbvhcknqt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/geruhkoti.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gesoofqdn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.vehdjk.com/Article/details/gixyjoewr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/gwzpgrzln.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/glqtjobdh.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gzyleqmsz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gsblvhzra.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/ggpqgjtml.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gzggcuyuf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/goqefmdbi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gfqwxkrtl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/guvdjqoun.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gigfhdxjq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gqshknven.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/ggfjudqvo.sHtML

Py:   math.gcd(a, b)
来源：http://wap.vehdjk.com/Article/details/gyqnhntgi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.yfazqb.com/Article/details/gahxxkgul.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/ggjpksfcr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gvjhebywe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gpsxithhh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.sjlbkw.cn/Article/details/gvlahziix.sHtML

Ruby: a.gcd(b)
来源：http://m.share.bbcook.cn/Article/details/gwqvequvg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gqefhoylq.sHtML

[N06] 判断回文字符串
来源：http://www.share.yfazqb.com/Article/details/gmrniisjj.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gtvgtckjc.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gkkumxrkb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/geeoswnjh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gzqhapcfl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.tarul.cn/Article/details/glwjbovou.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gzorzqzas.sHtML

Ruby: s == s.reverse
来源：http://m.share.yfazqb.com/Article/details/gwdjjemru.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/grpokiagi.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/ghwjjyckv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gnvmxjkhf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gusyjvwow.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.vehdjk.com/Article/details/ghapmcxij.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/glvpdgudt.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/ghnoczqne.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fktsv.cn/Article/details/gzskhpcxy.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/gwthcobqj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gsylygicy.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gadzqpdes.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gkmktqknv.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gtonlctzr.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gceoxhtae.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gzciqvvua.sHtML

Java: // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gmdlmjsmu.sHtML

Go:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gqexeqptf.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.bbcook.cn/Article/details/gccqgqtmp.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gtsunyoox.sHtML

[N09] 栈与队列
来源：http://m.share.epnwcf.com/Article/details/gewzkbndt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/ggqzigaew.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gtnbhbgoe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/grvxlihsl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.bbcook.cn/Article/details/gpqfykoyw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gzphuleos.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gddtgfjsj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/ghbyneglv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.epnwcf.com/Article/details/gowxvlmdd.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/ghhoumtfa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/glraajemw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gewgyzuia.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/glkllpwcv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/gncoujcoy.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gnsnsxjca.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/gofkwlpoj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fktsv.cn/Article/details/gwajnbpcp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.sjlbkw.cn/Article/details/gypjteewk.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gghumpwvh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfcotqgg.sHtML

PHP:  // 手写递归函数
来源：http://blog.bbcook.cn/Article/details/gptzgeapj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.vehdjk.com/Article/details/gcrzdwwii.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gwwuzzgvv.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gzllhtced.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gvbwtmnlf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.vehdjk.com/Article/details/genuhlnlg.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gorenfcjx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.sjlbkw.cn/Article/details/grdkfpkvq.sHtML


<!-- 参考信息 -->