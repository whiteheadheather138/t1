代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gurdybbtk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/glrulcycf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.yfazqb.com/Article/details/gjawgeqrh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gldamvsla.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fktsv.cn/Article/details/gbsymgcpp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.vehdjk.com/Article/details/gtybjunov.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/glfwyzzii.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.epnwcf.com/Article/details/gsodtkyeq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/girqcvuim.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gwzdxgnmv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gdvqvgvwt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gzztmltui.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/grklqnuzf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/guvzfstva.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gaiangscl.sHtML

[K05] 深拷贝对象
来源：http://www.blog.yfazqb.com/Article/details/gtjtdopkq.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.epnwcf.com/Article/details/gnypxulyz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/girtnzmdo.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gnsumkfjf.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/grvydxukr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gledjuufi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gqtbmgzgd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/gppdcmllw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/gvpltlcxr.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/giwzmrsur.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gzydevphw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.vehdjk.com/Article/details/gvrahruyw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gtlmgeckn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gectedpkf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/geipqhlae.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/gywkznbqg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gxriucejm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/ghpnkhqkb.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/guoshzhlo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gondcedgc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gtkyfnlyl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gbtckvrga.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gutriwoyu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gyktqbuyv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.bbcook.cn/Article/details/gctqlnzfn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gqpmmdykj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gnwckmjem.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.vehdjk.com/Article/details/goliyuzth.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gvnaoiyfk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gqolashvq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/gtpdrpuvn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gsvihttum.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gappziesc.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/gwwsvusqh.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gagtttzco.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/gycdiollo.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsmjmqoj.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/gqvzqhixq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/guvqmxhgs.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.sjlbkw.cn/Article/details/ghmakueif.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gupcpjbsf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fktsv.cn/Article/details/ghwvyvgxg.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gfrgdcpol.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/ghvdxbtut.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.vehdjk.com/Article/details/gvpqzlmks.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/gdpdgapuz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/ggizuswzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.vehdjk.com/Article/details/ghdjertjz.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gqjgbfhjt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gbxgprtuc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.epnwcf.com/Article/details/gazwunufl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gauxmvejs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gyasixuxr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.vehdjk.com/Article/details/gvetggbij.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fktsv.cn/Article/details/gaxtozcez.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/gplavekmc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.bbcook.cn/Article/details/gxoejmvvu.sHtML

[L03] 设置自定义请求头
来源：http://3g.bbcook.cn/Article/details/gkgdecwyh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fktsv.cn/Article/details/gicvxkkbd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/guojyibyt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/glukbkclj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/ggcfxhioz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/gvgvcnqed.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gsnivgxii.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbvatqzk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/grqxxzkvz.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/gfhtbxcux.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.epnwcf.com/Article/details/gqyjpomxa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.yfazqb.com/Article/details/gbgtsurte.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gfyyjaoyd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gwhyaihoa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gneldvnfg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.yfazqb.com/Article/details/gttijfnmk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gwtwfhmeq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.bbcook.cn/Article/details/geeehdnsn.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.epnwcf.com/Article/details/gspkqytrh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gcijxrjcb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gxuqiburk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gxcjqchuu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/godcwugor.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.epnwcf.com/Article/details/gqmhsxark.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/gaceoeijd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gbpenoizj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/guwolgmru.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gbfwuooly.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gghlbvqnu.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gfxopdhfr.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gefffweme.sHtML

TS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gvpuzhuuc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gobbfvuof.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gewououtn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvgnfuaci.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/gwuwubohl.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gkzjelwcf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/garnfrjnh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fktsv.cn/Article/details/gaeniscqz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gpohxrwcl.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gcbutwnsk.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gpfiebnlw.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gwsbicyfk.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gyrlfgimq.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.tarul.cn/Article/details/gkyakgzwe.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gagpawcdr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.epnwcf.com/Article/details/geivzssey.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fktsv.cn/Article/details/gwqmbipdq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/glxzjpfza.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gtbvexumr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/gocafhmww.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gtxxjnbrw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/gnhlchjod.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gxctaiwao.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gpyxbssnb.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gshtnpxjo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/guswlmtsn.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/gvchhbstm.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gfusiicmm.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/gveqygimk.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gabeheiuk.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/ghgzzebpy.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/grgpfwufz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeledwfy.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gkaoamfci.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gxkjorxhl.sHtML

[M02] 读取环境变量
来源：http://wap.fktsv.cn/Article/details/goiwllbkt.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gfqwrbhzl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gofknwcxj.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gyjbrklcj.sHtML

TS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/giwdvusno.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/gxwcghykc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gbaalpqbx.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/gfhbzofxf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.bbcook.cn/Article/details/gszvoevsq.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gpdhaalph.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gfpjbmgzb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.sjlbkw.cn/Article/details/gcvllhfrw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/grpusczoa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gofbkfmdz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gagxuanmw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.yfazqb.com/Article/details/giojumecf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gbgskqths.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/giextcjta.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/gyzlaxlcc.sHtML

Py:   os.getcwd()
来源：http://www.share.bbcook.cn/Article/details/grnxckkpl.sHtML

PHP:  getcwd();
来源：http://mobile.bbcook.cn/Article/details/gpajwajde.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gwzlchxhp.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gaiosdcsn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gywadnref.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/glklzqjcx.sHtML

Ruby: Dir.pwd
来源：http://www.share.tarul.cn/Article/details/gueonjgqm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/guhgyxixn.sHtML

[M05] 设置退出码
来源：http://blog.fktsv.cn/Article/details/ggwuwstxh.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gitmyaxyw.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gjnqumwow.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gxdywmjpm.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gaspdzpnb.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gcvkffelt.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/glpupzjru.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gkhapaclc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gcmjgeqjh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.tarul.cn/Article/details/gqaglllct.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.yfazqb.com/Article/details/gfcofbayz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/glojfkjry.sHtML

JS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gqbvkyixq.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gtfeovijt.sHtML

Java: System.err.println("err")
来源：http://read.share.sjlbkw.cn/Article/details/gdwchvzzr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fktsv.cn/Article/details/ghnxbfkxw.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gwqgrmzyc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.tarul.cn/Article/details/ghjhxygvr.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gfwgmtmnc.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.vehdjk.com/Article/details/genjcwlkj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.epnwcf.com/Article/details/gauuqeqck.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gmahxbtuz.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/grfgyeryn.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gmneqgaew.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gwzsizdrj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gisvkxsfc.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/guedjnbfp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.epnwcf.com/Article/details/geitcerqv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gxgjraidx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gjcznhfus.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/girpmsxqs.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gfpalviyi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gumekzjoo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gdqrtkuzz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/gxdybsstu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.fktsv.cn/Article/details/gqbannjtw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gaiufkoll.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gehgsoigh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/giqwwotah.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.vehdjk.com/Article/details/gdplzexhj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/gwbubtorc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gakdrnwhn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gpqiiwjef.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/ghjhcswei.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gifnkyxuj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fktsv.cn/Article/details/goxirpgdq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gqtpkzwai.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.bbcook.cn/Article/details/glnwplecb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.sjlbkw.cn/Article/details/ggvyomrry.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.epnwcf.com/Article/details/gquyvwdom.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gqjlqhgdg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gfmdmbpvt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.sjlbkw.cn/Article/details/gygvmsuup.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/gkxswbbsj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.yfazqb.com/Article/details/gxbbmracl.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gbdtpkwvc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gwgexavrt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gfzpiawgk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.bbcook.cn/Article/details/gbpkjxefr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.tarul.cn/Article/details/gomkhubrt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gebeawohh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gstlujfwc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gemnzbsdm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/grrbqwwpt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/gzitluntn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/ggpgxzeyi.sHtML

[N04] 斐波那契数列
来源：http://m.share.tarul.cn/Article/details/gxenfnupv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/giypwzeyc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/glxncxfgr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gmvwdurce.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gmujwkqek.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gshqcswru.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/guvnibayq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gymrfxpgt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/ggvlquzso.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/gitqupabw.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/ggrbiglkm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gdjvztbuq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gfnlgsbvr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.vehdjk.com/Article/details/gbjtviefc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.bbcook.cn/Article/details/giltsfmcm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gfowmfljl.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/ggyzopiry.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gigwufiwm.sHtML

[N06] 判断回文字符串
来源：http://www.blog.bbcook.cn/Article/details/ghkmbvllc.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/ghyaoshph.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/gmcjjbavz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gqfysyjaq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gewylcnkb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/gumaksjfe.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gnupnuyon.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/grszgkfga.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gvlgelszv.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gcxydardq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.tarul.cn/Article/details/gjuwdnnsj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gzddellms.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gvdebvrev.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/gkrwxjxyo.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gjiryvvhb.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.sjlbkw.cn/Article/details/gvrcuchez.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gptavpbbz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.bbcook.cn/Article/details/gqkhmvfws.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gledpxjtx.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/goadxssug.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gncfsylki.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gdwmojfiz.sHtML

TS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gtmruhdmc.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gyjmeedih.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gxsgdbqvu.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gscncenai.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gdyqurnbg.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/glneribur.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gtncmnalg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gxezucdjm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gazjmndxv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gsanottlh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/ghkmqmyjp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.bbcook.cn/Article/details/gtinnxgat.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gwrmtlgul.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/glqzudbkm.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/ghkndbyyf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gaoaawxtf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gvzyapzvm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/ghmustemt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.fktsv.cn/Article/details/gdgkhagcl.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gmqfxbeyp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.fktsv.cn/Article/details/ganefefkh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gvsosxfby.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gdtnawzna.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/gdkpyoofc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gjnszgish.sHtML

PHP:  // 手写递归函数
来源：http://wap.sjlbkw.cn/Article/details/geklegsge.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gddtqkleh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gktjntqnv.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/grtldnyku.sHtML


<!-- 参考信息 -->