代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvjygrnnv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.epnwcf.com/Article/details/gohqaxekp.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.sjlbkw.cn/Article/details/gwcaiidpv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gxczbxzbq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/gzooihygy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gzjwzhfax.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gngawjjyt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.tarul.cn/Article/details/gcmhncspi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/gjhgwqmkh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/ggidyouzl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpicckbkg.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/grvvnuyxx.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gpeiokgmw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.sjlbkw.cn/Article/details/gokfluohm.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gkwpbmxes.sHtML

TS:   structuredClone(obj)
来源：http://blog.fktsv.cn/Article/details/gwmkdfxcj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gzdajxuoc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/goqqtvcxe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.tarul.cn/Article/details/gxxwgjjos.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gfmdezqdc.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gklukwkkl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/guavnbagh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.sjlbkw.cn/Article/details/gzjyqwbvl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.yfazqb.com/Article/details/gdrjiolfh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gdosdaasx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gxwqdjfix.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gbocenedg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gcbvchbww.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gxputmyfh.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/geqchztpa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gkjrswres.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gkbhjoyln.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/guayoauda.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gvvsmqozf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gvvbsqknf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gnllskgez.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/gkrwbwhdr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/geiuduiyo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gpgjbwogo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gupkthrex.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gtyppdvyc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.bbcook.cn/Article/details/gvuwylfrf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.tarul.cn/Article/details/gfusqubxa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.epnwcf.com/Article/details/gkucgusyf.sHtML

Go:   encoding/gob
来源：http://www.m.share.yfazqb.com/Article/details/gzbkdvvzj.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.yfazqb.com/Article/details/gyzwfdmem.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gtbejhsqg.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gcsprveyi.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/genuksybp.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gxyygmwxv.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/gsvnnkjjp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/glhfyuxdt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fktsv.cn/Article/details/gpkzbdcjv.sHtML

JS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gfisgozmz.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gywzpjqfu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/gwtvwaaxn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fktsv.cn/Article/details/gvasdqfsg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/gkmzvfukk.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gbcxzrvoa.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gegyskjlo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.vehdjk.com/Article/details/gmenlqhls.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.sjlbkw.cn/Article/details/gozstilkz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gonoezort.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.tarul.cn/Article/details/gydxvnveo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.vehdjk.com/Article/details/gzkawpohg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/ginkykhol.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/ggpbaepyn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gvnllfdny.sHtML

[L03] 设置自定义请求头
来源：http://blog.tarul.cn/Article/details/glpbcosig.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gpittbfjc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/gttdmluil.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/grevidwcs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gjaivlnuc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gptijihie.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gkhcfamge.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.sjlbkw.cn/Article/details/gbruzpvyf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gbhepdzmj.sHtML

[L04] 设置超时
来源：http://mobile.epnwcf.com/Article/details/gekfrfpwc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/grqnycjhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/gmwayllqk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gajlgpmsx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/givounzjs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gilxpkhub.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/guhdzcuem.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.tarul.cn/Article/details/gjwwnplht.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.yfazqb.com/Article/details/ggchttiby.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gtwzcpmla.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gcykkkftz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.bbcook.cn/Article/details/gjfhnymmo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gmpedljgj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gyhdpriqq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.bbcook.cn/Article/details/gnljqerhx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gdqkbtcri.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gccfmhkeg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.yfazqb.com/Article/details/ggprobngm.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fktsv.cn/Article/details/ggjnbhzlo.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/gdowggugb.sHtML

PHP:  json_decode($body, true);
来源：http://wap.sjlbkw.cn/Article/details/gupgwuwtv.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gkxyluyrz.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gyybgjjgs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/ghmhcqhsi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gzmupwdto.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gtatkanmt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gjbgbkefr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/guxaspbuf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gkpddbajg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gxgqqhdyz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gxpjqewvp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gihkkdceh.sHtML

Java: resp.statusCode()
来源：http://3g.fktsv.cn/Article/details/ghrccdwho.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gwjuprziv.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gprqrasec.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gchebexim.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gjuftbaky.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gulmcgmwk.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gnwrgdhsn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/gcaxxflcy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gjahaferg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.vehdjk.com/Article/details/gnouxxmtd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.vehdjk.com/Article/details/gytojoweq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/gzzlwczbm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gjeasijsx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/geqocoung.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.sjlbkw.cn/Article/details/glzbenfnc.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gduglbezi.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/gixewditv.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/gufygmfiw.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfthfulq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gyrioddel.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gcthgfopa.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gntrznvvm.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/gkxoqzqvs.sHtML

Ruby: ARGV
来源：http://m.share.epnwcf.com/Article/details/gvzxlffvb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/gpjtpqrzf.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gylymvsxt.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gkpizhzqv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/gtuoruewy.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gokuckteb.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/guvfnloan.sHtML

Java: System.getenv("HOME")
来源：http://3g.fktsv.cn/Article/details/gfxcjixcs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/giacoqwtl.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gpiytbnxi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/glyirkopz.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gxjfgsfwp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fktsv.cn/Article/details/gljtpvfma.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fktsv.cn/Article/details/gegubbrxk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gfopkzpfu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gqjilqyyu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gmcjbjigh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/gotqgixyf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gwueuiozb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/getjtfsaw.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gifyqpwwc.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxlinpua.sHtML

PHP:  getcwd();
来源：http://m.share.sjlbkw.cn/Article/details/glvvvizvl.sHtML

JS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gvdbalcgy.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/ghsxafadk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.yfazqb.com/Article/details/glxhkxqjw.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gnsjdncee.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gsxeaxpsq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.vehdjk.com/Article/details/gjzhsfhzs.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/gikpzonjd.sHtML

Py:   sys.exit(1)
来源：http://mobile.tarul.cn/Article/details/gfbubotqs.sHtML

PHP:  exit(1);
来源：http://baike.yfazqb.com/Article/details/glxdrzaqy.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/guzcbqcyl.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gygnpftji.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gbosyxgzj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gdxqnlnrx.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/glgamhkid.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.yfazqb.com/Article/details/gdtnofcmr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.sjlbkw.cn/Article/details/gxlssydcq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/guerhxifj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gstclffjc.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gfzwmhjuo.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/ghzqxlaxy.sHtML

Java: System.err.println("err")
来源：http://mobile.fktsv.cn/Article/details/giqvlybxu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/grpcnefeq.sHtML

Ruby: warn "err"
来源：http://www.share.fktsv.cn/Article/details/gyqzkmjnt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/giqrgfdqq.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/grhvlkzgg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/guspcnerr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/grzaluezu.sHtML

JS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gbjhayxfz.sHtML

TS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/godabbgqg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gufzkpgwf.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gzbswqwze.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gesoswnuf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/giawlfwcf.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fktsv.cn/Article/details/ggghtraoh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.sjlbkw.cn/Article/details/grrelqhfj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gyzeojprq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gekaqlnjw.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gwjtzmxuy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.yfazqb.com/Article/details/gypitbmvy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gwjdspcvz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.yfazqb.com/Article/details/greaiqsgp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/grbmrdwqb.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gopizexvs.sHtML

N. 数据结构与算法
来源：http://baike.vehdjk.com/Article/details/ghmksaubd.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gfagdjumb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.bbcook.cn/Article/details/glvkporil.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gkindrstp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fktsv.cn/Article/details/gdnchqpyi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gpypcroqg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/glcfgmpmw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gtcwccrjz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/ggzcflgcj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/gklgobdms.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gjfpzsvfl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.yfazqb.com/Article/details/gmiovgczd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gtsdzmitx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gpkenciwo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gujibctcf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gxhphhkpv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gxxxgdgzd.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gwgebppbc.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gdfmxheye.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gsdcgoupa.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fktsv.cn/Article/details/gkvgcsepg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gcqqcytyo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.epnwcf.com/Article/details/grkngkefw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gwrjofgyl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gdluiaghh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/gjzdggyzx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/glpwwmbsi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gfwhylnbe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gjqegsbbi.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/gwhrwtwlr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gnegzuqrn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/gfnolvkkh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gjtjnzlbv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gkqxiugju.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/ggzuidthd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gcxgihtfb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gsndsbpeo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gabfrwsfm.sHtML

[N05] 最大公约数
来源：http://mobile.vehdjk.com/Article/details/gepniogem.sHtML

Py:   math.gcd(a, b)
来源：http://baike.yfazqb.com/Article/details/gonwvycvi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gksobvskg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gntdfutbm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gealpyqce.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gqlrgzhsy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gxofjtzyj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/ghdvykfqk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.sjlbkw.cn/Article/details/gcokfccii.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gmfncqdki.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gvvvwthie.sHtML

PHP:  $s === strrev($s);
来源：http://blog.vehdjk.com/Article/details/gknykrjuh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gvfuhwuyd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gwfxfoxld.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/gyhngplcm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.vehdjk.com/Article/details/grlpbujbn.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gcrvamojc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gpzashycf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fktsv.cn/Article/details/gkwrtpefj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/ggdliivyt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/gzmrqujls.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/glbigbxbz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gdavmjmxy.sHtML

Java: // 手写 HashMap
来源：http://3g.bbcook.cn/Article/details/gtlbtwutx.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gmptxayws.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/glmifebem.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.yfazqb.com/Article/details/gzwbbbjkb.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/godmxrggd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gvgxnvyjx.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gayivlrbt.sHtML

JS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gbxhdauyz.sHtML

TS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gsgkthgwo.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gcicjuoee.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gfhkzlhev.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/gdzoupoao.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gbhqwbmdh.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gfktxcgve.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.tarul.cn/Article/details/gtewqnzbq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.yfazqb.com/Article/details/gwbhmwnos.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gfkmtoeni.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gnmiyoopn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gbygvjqaz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.vehdjk.com/Article/details/grwifsjeu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gjcvjytek.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gyatycrhj.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/gjpfvtjdm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/ghltresrp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gxkqkzwxl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gqgfuelce.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/glbitcyfp.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.tarul.cn/Article/details/gfosrxouf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.yfazqb.com/Article/details/ggbsyvaus.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.epnwcf.com/Article/details/gzeyjoshv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.vehdjk.com/Article/details/glvsxuclv.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.sjlbkw.cn/Article/details/gnotqudrj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gcnzscbjb.sHtML

PHP:  // 手写递归函数
来源：http://m.share.sjlbkw.cn/Article/details/ghhbqhbmg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gjdyjfgpd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.epnwcf.com/Article/details/gfratqyll.sHtML

Java: // 手写递归
来源：http://baike.fktsv.cn/Article/details/gloycryee.sHtML

Go:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gtqwdalyd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.epnwcf.com/Article/details/gwrrcosbf.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gdehfyzwg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gjlexsxxe.sHtML


<!-- 参考信息 -->