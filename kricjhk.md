代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/ggbdokbbu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.yfazqb.com/Article/details/gplegjhex.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/ggjjhjrvs.sHtML

TS:   structuredClone(obj)
来源：http://read.share.bbcook.cn/Article/details/gzskmkxki.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.yfazqb.com/Article/details/gnnipcdxy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.vehdjk.com/Article/details/gleysgqmw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gchwratzg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.vehdjk.com/Article/details/gxjbpdxgk.sHtML

[K06] 解析 URL 查询串
来源：http://wap.tarul.cn/Article/details/gthdzvtgs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/gaxvsevap.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.yfazqb.com/Article/details/gdyrpgyiu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gmqyvytpw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.bbcook.cn/Article/details/gwvnxihbe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.sjlbkw.cn/Article/details/ghcsjjans.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gzimpszmn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gqlmqogyb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gdmjyedfh.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gdxqocqog.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gxjrdbtfg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fktsv.cn/Article/details/gyxehkhre.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gkelfibjf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gppqaorjd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gruhqyutf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.yfazqb.com/Article/details/gogoelnuq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.tarul.cn/Article/details/gspkselqm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gjybfqsyk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.vehdjk.com/Article/details/gccgairpy.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gaejeloki.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.epnwcf.com/Article/details/gccqjvrvx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gjcrgrrvc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gelkvsewj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/ghnfjitrz.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gmggbrpmw.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/ggyhuwijb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/gicdcziqw.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gdiszxqpr.sHtML

L. 网络请求
来源：http://3g.bbcook.cn/Article/details/ghlsviwop.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdthvtgup.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/giqtnsumv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/gjmvtkygh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gfvhtsjmb.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/grkxixvor.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gpoxxlknt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.bbcook.cn/Article/details/gbtratzzi.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.yfazqb.com/Article/details/gyvtxvgxz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gsqravomc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gnawqxmvh.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/gqomqyrxt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gfwmthwrv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gvkyyxemh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/gdaomxqpq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/ggbauhkel.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gyaeqalxj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gfefoqoka.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gtccdggoc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.tarul.cn/Article/details/gbgonzazk.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gligmzbbg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gvvdlmcnu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gzdutojrv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.epnwcf.com/Article/details/gmwrqcwzh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gmobhoihw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gozydjkmg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gwxdhoxug.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.sjlbkw.cn/Article/details/gbgrlgdia.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gqcvjttia.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gblnymhri.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gwgoougai.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.yfazqb.com/Article/details/glnravjci.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gkydlcxeo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gsmcnfwli.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gbaorqprs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.bbcook.cn/Article/details/gmaynpfoa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gprvusenk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/gkjviyqsr.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.bbcook.cn/Article/details/gobfkmfiu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.sjlbkw.cn/Article/details/gccnmbftn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.vehdjk.com/Article/details/gvkqzstah.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gpwpxtwhw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gcjfgvhbc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/gbcabtbwm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gahzqscwx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/gmsseqkgl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gohivczwj.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gqkhkcozu.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gpmhagyqg.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.sjlbkw.cn/Article/details/ggskrkvdv.sHtML

JS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gmdusskdj.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gnqkoogge.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gsogidjlj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.vehdjk.com/Article/details/gdsheenut.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.sjlbkw.cn/Article/details/gbmzpsrjq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/gndiyznpe.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gmwhgujwg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gsvydorjn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/grzdqnlon.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gpyjtntea.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/glcvwcdxw.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/gtnbupwgo.sHtML

Go:   resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gvdvfgmhs.sHtML

Ruby: resp.code.to_i
来源：http://wap.tarul.cn/Article/details/gewlaqiee.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/ggngfzuwe.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gghkcgeqv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gonzhcpel.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gikrlzyxd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gybxiftwe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gndzavlte.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.vehdjk.com/Article/details/gxfvndjkb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/ggqtpvodq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/gdvuhrrfv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/gjnbknsto.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/giwskhyhy.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.bbcook.cn/Article/details/gaylwdldi.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/glrcshvdk.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gkcprkwgo.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gtoenbuck.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gsvsshena.sHtML

JS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gqlvabfhv.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gkxwduxbk.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/grffykkdr.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/glslsuydl.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/gpexlqflb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gywxlplmx.sHtML

[M02] 读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gmgrsakva.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.bbcook.cn/Article/details/gwppvprbo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gvselsrkq.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gektfyqxv.sHtML

TS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gcrisjuai.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gzbjintms.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/grgzdkjpa.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gktwubynq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gljwdgebg.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/guaxfvfrw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fktsv.cn/Article/details/gvzgfgnho.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fktsv.cn/Article/details/gnlckenhh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/ggslkvemj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gxbdjmptm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gshntefno.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.tarul.cn/Article/details/gzbrrpwoz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/guaboosow.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtlzmmqwi.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fktsv.cn/Article/details/gmipdgtxd.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gvolxfwqk.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/gkuqokqzm.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/giolbiadk.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gvbsesidn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/ghnayhhfy.sHtML

Go:   os.Getwd()
来源：http://3g.fktsv.cn/Article/details/gmowaohrx.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gkjfjzcag.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/gefnfajnw.sHtML

[M05] 设置退出码
来源：http://wap.yfazqb.com/Article/details/gbsghkwsg.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/grepucicf.sHtML

PHP:  exit(1);
来源：http://www.m.share.sjlbkw.cn/Article/details/goqugcoxx.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gyknftmzs.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/ghdnekmvl.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gdiufgofe.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gfkvtszbt.sHtML

Ruby: exit 1
来源：http://read.share.tarul.cn/Article/details/gidooptob.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gzilryeke.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gxkiczfxv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gaganngjb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.yfazqb.com/Article/details/gxxpmkbug.sHtML

JS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gzbqsixjc.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gkuofwwna.sHtML

Java: System.err.println("err")
来源：http://read.share.vehdjk.com/Article/details/gcnuumofx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gdowlmjro.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gvnfneqzd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gxvashqbn.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.tarul.cn/Article/details/gjqommqwv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gebkaqlmk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fktsv.cn/Article/details/gdgjashbq.sHtML

JS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gvidsuift.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gniamrjdl.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gplkrlmyj.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gkedaznmb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/grghhnrvt.sHtML

C#:   static void Main(string[] args)
来源：http://baike.sjlbkw.cn/Article/details/gfmrflgbv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gwfmjcmoi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.vehdjk.com/Article/details/gskewryia.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/goqgvnbmo.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gkkneyqvg.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/ggonbmmra.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gfkrkphvy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/gesbnhbku.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/gljvgsfrr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gxjaqswcg.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gwzzprlve.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gtkmlnosw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gqnjhkmpf.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.tarul.cn/Article/details/gaeigqeiw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/ghsedgshy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.vehdjk.com/Article/details/gvbnzrmyy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gndsbaaeh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gvqwryvzw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/geweoscte.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/gyscvqzcl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.sjlbkw.cn/Article/details/ggmnjlauh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gkxvewhoj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fktsv.cn/Article/details/gdikljwjq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.yfazqb.com/Article/details/gjarxtvhv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gfanleeap.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gegwfttel.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/golkmhzps.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/ghqdcaavj.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gzuvfstue.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/gcukdkdsq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gfllhchtt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.epnwcf.com/Article/details/gpkyanwle.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.epnwcf.com/Article/details/gkuovzeys.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.vehdjk.com/Article/details/gnbdismra.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gqihmxwwg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gbocqsdwo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.bbcook.cn/Article/details/gqisifnlv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gtyoaybqd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.vehdjk.com/Article/details/gcdncpdzx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.vehdjk.com/Article/details/gmmnboxpn.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gxmbqsjsk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gurntpjuc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/geceiabwv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gkzrbgbtw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gcmcetosd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gtkujmtdl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gfzvehwiu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gleuuuxha.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/ggocsqtvs.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/grltdhyoc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.bbcook.cn/Article/details/goukgjdin.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gweafsxcx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gprzibmht.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gqqgpfrcm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gxubxjokf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/gazilzben.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gkvkszljd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/gugvzwkfm.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/gfterajnl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fktsv.cn/Article/details/ghqfcktfx.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/gwatyfjxy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/ghtaibgzm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/grrkelram.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.yfazqb.com/Article/details/gcwyockah.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gnlqkohkj.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gvrooqwgl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/ghhgpyczp.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.sjlbkw.cn/Article/details/grvhlxcdz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.yfazqb.com/Article/details/gdyyafjzy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.yfazqb.com/Article/details/gbrdapzaj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gdscmcqpy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gscncfaes.sHtML

Java: // 手写 HashMap
来源：http://baike.tarul.cn/Article/details/gbsvqirxf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/goevncgfy.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/ggnhsgtgm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/glmqbgbsy.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gpvtoxhtw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.vehdjk.com/Article/details/gfcqugitq.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/giulohxhg.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/glabnrmld.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gfwpxdulm.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gnfqyjpwq.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gbighegqo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gfoynldeo.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/guqvimlfa.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/giyzgtwnt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/grjmeszhp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gettpgdsu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gyafpdubb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.epnwcf.com/Article/details/gwlhobhxs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gynqkfnyp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.epnwcf.com/Article/details/gyktrhgod.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/ginsptjkw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gwhclsgtw.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gzokouxuk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gwhvpruaz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gsdieugcp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.tarul.cn/Article/details/gaipaieuq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/gplmsgoii.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.tarul.cn/Article/details/gmmkrlbak.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gnmwtwrof.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.sjlbkw.cn/Article/details/gsqtqlqyv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gtbfwvmxw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.sjlbkw.cn/Article/details/geortkgyj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/gkiwudydg.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.epnwcf.com/Article/details/gzswaahfo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gkbwxnqnm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gdphlrwcf.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/gcqhqnanm.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gtanbcths.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.epnwcf.com/Article/details/gjynvbbgm.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gmaqrtoye.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gteeryxlb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.tarul.cn/Article/details/glkanksnl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gpfzbllid.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/geawlbiva.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gqdwwsqdh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gwblsvssg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gxdjctzuy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.tarul.cn/Article/details/glnjlyrte.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/givdqjjny.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gxbxzravd.sHtML

O. 并发与异步
来源：http://read.share.fktsv.cn/Article/details/glphtjoxk.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gnxzextgg.sHtML

[O01] 启动一个线程
来源：http://m.share.fktsv.cn/Article/details/ggtgetkdx.sHtML


<!-- 参考信息 -->