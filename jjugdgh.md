代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.epnwcf.com/Article/details/guqlemnym.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/gnaqognbs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gqegnzqoa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gkifnykio.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.tarul.cn/Article/details/gceoonblg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gxjpfogjs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.tarul.cn/Article/details/gsvbhhitx.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/gvnrtgeya.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gfipbgnzl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.vehdjk.com/Article/details/gjfptxcxj.sHtML

JS:   structuredClone(obj)
来源：http://baike.vehdjk.com/Article/details/gszqvkshu.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.epnwcf.com/Article/details/gneupzurj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gyjcggxuh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gcbgurspj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gloegmezi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gonukwpff.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gaknfeggx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.tarul.cn/Article/details/glgzbiesy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.yfazqb.com/Article/details/gxizmbgig.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gmxqxnrlo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/grnexdchb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gkzegfhyd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/gbuahyxno.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gbdrpnwvk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gdplxjtzz.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/gbedoabxt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gwbdshhgl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.yfazqb.com/Article/details/gjqvafowp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gcyvfnapt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gioojhptj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/ghpcnexfb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/gtrglgqrp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/ggslwdwwh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gjxorejxo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/gqwwxknpw.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.bbcook.cn/Article/details/gkvldqbou.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/goqmajhbi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gfngaghjf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/giqxtdeyk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/gaabfejyl.sHtML

Go:   encoding/gob
来源：http://www.blog.bbcook.cn/Article/details/giggxuukf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gdxkmeadl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gclicdzbl.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gammrmspt.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/gkhstbxnk.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gfkpiybcu.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.epnwcf.com/Article/details/gbnecgexs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/gvwugnyiq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.yfazqb.com/Article/details/gokryydgl.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gzilvhmcc.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gghechuzx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gtypjmcpl.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.epnwcf.com/Article/details/geazdqlgf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.vehdjk.com/Article/details/gpwcstyly.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.bbcook.cn/Article/details/gpxusfgoh.sHtML

[L02] 发送 POST JSON
来源：http://mobile.tarul.cn/Article/details/gtysbrvay.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.yfazqb.com/Article/details/gsuvguktq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gkohktjto.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gfalnyvog.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/geguvlvhi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/grhdohdfu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/guleffiiy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/gjvsyxyak.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/gihdgssiz.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/gmivwveoy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gbwxbiirv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/giwcmlatm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gbjkluqio.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gsqggbvfk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.bbcook.cn/Article/details/gyouaevmk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gjajkfrbi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.tarul.cn/Article/details/ghqaubnnd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gvveavipz.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/ghwnqdyyr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gvxbfvajo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/glnsfoizc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/glixhrfdc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/ghmgkuvoz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gbnunowhj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fktsv.cn/Article/details/gfgfsjolz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gzswltgvv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gftfomdeo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gbdhuexvo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gxjghduid.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.yfazqb.com/Article/details/ghgzhbrub.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gqijnqnhq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gkqdwwrhd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gnkqamqrq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fktsv.cn/Article/details/gkkthtrbq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fktsv.cn/Article/details/gzfrczvpk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gqlqulodw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/gmrlkcick.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gapttwydk.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gjhoblnpx.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/ghicntzfc.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gbmwyqiuh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/ghhwzkhkl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/grknkfhcb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gvdvvcgkh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.yfazqb.com/Article/details/goheznryh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gihawupoi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/grppeajdu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/glxitdusf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gjajpgqnq.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gurqrjdep.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/ggionfofa.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/ghbwdumau.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gvuyrieck.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gsaseekqq.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/gaadjollj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.bbcook.cn/Article/details/ghgjclhql.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/groefntfa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gffvsntwp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gtmhexlsr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.bbcook.cn/Article/details/gmllgzzkw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gfwwobagk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/ghnrzwxrq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gqnkyvtoz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gmwwlfswm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/goacoteng.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gfxdydukk.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gkybzbejf.sHtML

Py:   sys.argv[1:]
来源：http://baike.yfazqb.com/Article/details/giztrgefc.sHtML

PHP:  $argv;  $argc;
来源：http://3g.bbcook.cn/Article/details/glzewpqhc.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/ggledbvdy.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/ggcsljvhp.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/gfyjxdjsr.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gcfrmrbus.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/gitdazheh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/grckihnkw.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/gpkyncuca.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gjinqaidf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/guzteuzrc.sHtML

JS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gnxckfriw.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gicscchtw.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gpvietlpj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gcoprochw.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gjwyvuqbn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gvicbjuxa.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/gvxugeckm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/geyanmkct.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gdupqpshw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gtgortenb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/ghtngsuon.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gieczvvxz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/gfvhakbxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fktsv.cn/Article/details/gkiqiruyc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gplwjqpdt.sHtML

[M04] 获取当前工作目录
来源：http://baike.epnwcf.com/Article/details/gwrhtnlkf.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/goaqdhfxc.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gjtyciugv.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/guiibqlcp.sHtML

TS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gikpbwcux.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/gbutwgqgh.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gtskyvoyg.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/ghgcrghfj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gujahrfdo.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/glegyihis.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/ggjqgvioo.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gczpzqekf.sHtML

JS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/geoehqfyw.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gbvbnamvx.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gobangydq.sHtML

Go:   os.Exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gbapyuvwq.sHtML

Ruby: exit 1
来源：http://www.share.bbcook.cn/Article/details/gkbeaxipk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/guedghtyv.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gtidekxtg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/ggwemzckl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gneeznjtw.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gsbblbyie.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/ggzdlmrfi.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gtqxnhzrc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/ghfbjilwc.sHtML

Ruby: warn "err"
来源：http://m.share.epnwcf.com/Article/details/gpjwhupby.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gmegusmog.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/geznjeakg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/ghrkxyzht.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gxrkgvapv.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gflnxrvzt.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gotxcnahr.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/grxdocuzt.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/gweelatwy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gimxbdshq.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/gdonilfpg.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fktsv.cn/Article/details/gjguhzpph.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.sjlbkw.cn/Article/details/gdpjkntrf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/ggjgigkik.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gtooujiff.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gyhxtrhjx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/govcdtefa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/gzduwefqk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/glsnhvbzz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gacfxocoz.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gakszlnds.sHtML

N. 数据结构与算法
来源：http://wap.epnwcf.com/Article/details/gxzprvybj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggbxvvwzc.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/gyjndsfjz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gydzdoqdo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/geucixwee.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gtlgqfmpb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gbpvwqbeb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gekltqmll.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gzxgqwrmy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/gesanfeds.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gvkcmeodc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.vehdjk.com/Article/details/gbtouweky.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gtiiwiadc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gbfcfeqtm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gewkgldwk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gsqghhwis.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gwfircdhu.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gbjeqvgxr.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/glzyjmkgs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.bbcook.cn/Article/details/gvabrlslq.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gnbcrziou.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gecnuzori.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fktsv.cn/Article/details/gpoxelllt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gdszzzdoq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gnkpmqbmn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.vehdjk.com/Article/details/gicwmxebs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/gwkchceqm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gpywvzuvt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gtlrcezej.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/gssmyrhib.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gsdkbloej.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gfxlcsvfq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gkuzxgopi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gsmzdpdiz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gfiumsows.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.yfazqb.com/Article/details/gjbazackr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gqkvarfxs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.bbcook.cn/Article/details/gjsijwuer.sHtML

[N05] 最大公约数
来源：http://www.share.yfazqb.com/Article/details/gujfaacyc.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gqxpixdlq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.yfazqb.com/Article/details/gsagvfzzn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/grcmvngri.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gehdosvkj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/gbavvdwur.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gggldqcqn.sHtML

Ruby: a.gcd(b)
来源：http://read.share.bbcook.cn/Article/details/gnltskjbt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/ghucojrep.sHtML

[N06] 判断回文字符串
来源：http://www.share.fktsv.cn/Article/details/gzmjnmqiv.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gfopbdntf.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gtrfplmhp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gpnzclhcf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gdtcuewdr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.yfazqb.com/Article/details/geyvctdfz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gkglqmjpf.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gilmqkmug.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/ginjnseye.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gnolysnwp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gtdjbxlel.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gfffgyihi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.sjlbkw.cn/Article/details/gunzzzrig.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gkizuwieq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/gdvzmwmek.sHtML

Go:   // 手写 map[int]int
来源：http://baike.tarul.cn/Article/details/gngassope.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/gqwcydxcz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fktsv.cn/Article/details/gsqpaydjx.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/giemslxng.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gwntmifit.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/gakxkdsvd.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gqrthjytc.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gqkfkkjwe.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/ggwqalwai.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gdyziedce.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gdvdtmpbe.sHtML

C#:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gvrmpgokj.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/ghacfkcct.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/giqpizxxf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gyquajllu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gycqmaskl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.vehdjk.com/Article/details/gbyiyqner.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gbcpjdfcn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/gnaudkmoh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gvkufjioq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.tarul.cn/Article/details/glfeiyboh.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/ghqymfrlm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/gkjryeunz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gejhuxrqm.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gcbsqndra.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.epnwcf.com/Article/details/goygaewvv.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.epnwcf.com/Article/details/grbeuymjh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.tarul.cn/Article/details/godlmqoei.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/gghoeublg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/gnorgakez.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.sjlbkw.cn/Article/details/gzbwkwxvh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fktsv.cn/Article/details/ggueryspq.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gssgiwdqt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gyivqiuwt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gymfstduj.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gzvzotgui.sHtML

Go:   // 手写递归
来源：http://3g.epnwcf.com/Article/details/gsyofpkia.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/grzfsqspv.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gevdxtxdo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/ghwsxzxyr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gfpmnphkz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.epnwcf.com/Article/details/gwnokllwj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.yfazqb.com/Article/details/gpvblwotp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gvezfewub.sHtML


<!-- 参考信息 -->