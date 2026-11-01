代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/gndzonnkn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.epnwcf.com/Article/details/gfltoootn.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gcxccokjy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.sjlbkw.cn/Article/details/grribzymp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/ghevwwjwt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.sjlbkw.cn/Article/details/getgbmkzn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gbupibigh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gjzygyrzl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/goztvyfwt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.sjlbkw.cn/Article/details/gyynxecvl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gsfvoflhx.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/glsvjqvhd.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gvqxkipmu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.bbcook.cn/Article/details/gmrzickwy.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gsxijnnbk.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gwdtdgcfz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.bbcook.cn/Article/details/gohdpkkgo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gsyvqheas.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.bbcook.cn/Article/details/glkgdkujj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/gndcclyiz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.yfazqb.com/Article/details/gepntodpu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/grrvpydfw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fktsv.cn/Article/details/gneulrmvc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/glktqungu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gbfyvokwl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/gvbfjiiiv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.sjlbkw.cn/Article/details/gfozohfab.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gapgehiel.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/guqsegeqm.sHtML

[K07] 进制转换
来源：http://m.share.fktsv.cn/Article/details/gvuwuiuek.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gnxtwnsdx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.yfazqb.com/Article/details/gyzyzaxdp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gmhcpqpbz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gfrpkhvrf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gkdypiahv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.yfazqb.com/Article/details/gaxemcpmy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/gfrjewvjx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gopcjskgu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.sjlbkw.cn/Article/details/gdirstzin.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fktsv.cn/Article/details/gajexdyyy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/gjewbvqca.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gucctprgc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gfuorivsq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gpwfaywfe.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gdhfduxxv.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gjablwuxm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/glfxdqfyj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/grfshhyqv.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gxkqdhhlu.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/giwmikmrn.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.sjlbkw.cn/Article/details/gwspvghgt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/ggvqumjai.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gnqzcdlvg.sHtML

JS:   await fetch(url)
来源：http://baike.epnwcf.com/Article/details/gamacwuvm.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gpvowkhfy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.yfazqb.com/Article/details/gpfevabns.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.vehdjk.com/Article/details/gbmtisdyb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gsmweyjnb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.yfazqb.com/Article/details/gphehkbds.sHtML

[L02] 发送 POST JSON
来源：http://www.share.tarul.cn/Article/details/gnmijydfa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gxnnhfqcy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/gfpyxtccy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gtbeegclv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gwwsxqepr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.sjlbkw.cn/Article/details/gbokfugxp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gksuycawv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/gviyliidl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gwtjsxsem.sHtML

[L03] 设置自定义请求头
来源：http://blog.fktsv.cn/Article/details/geqoplixa.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.epnwcf.com/Article/details/gfntumeki.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/ghuolpffb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gxnpzjsya.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/gactornvr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.tarul.cn/Article/details/gzcabjuwp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/govxoyxxd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/golrysynp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gccxewdoj.sHtML

[L04] 设置超时
来源：http://3g.sjlbkw.cn/Article/details/gepqncsah.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.epnwcf.com/Article/details/ggpgriipb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gcssqdnyr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gpbizgwqe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gyaollvkx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/gpzudjyaf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.yfazqb.com/Article/details/glszcvakz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gejywqeic.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/glzrhjssf.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gpavklctr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/gvcpuzvcg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.sjlbkw.cn/Article/details/gsyknuhbu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gzcsrfypi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gsrnixujv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gtsugljmx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.tarul.cn/Article/details/gxspzaops.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.tarul.cn/Article/details/gzqldjben.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.epnwcf.com/Article/details/gdhebwqpq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gnmodyjuw.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/glopoeqzz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/gjhbchoec.sHtML

JS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gmielhxpm.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gkmwjfwvj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gibdqafup.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/gsalwlmgy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.bbcook.cn/Article/details/gifygtujl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.epnwcf.com/Article/details/glzjfonig.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gkwjnuhln.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/gyumsdhbh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.sjlbkw.cn/Article/details/gddkcvoqz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gpczxkssi.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gebdqqxxv.sHtML

Java: resp.statusCode()
来源：http://www.blog.epnwcf.com/Article/details/gqyjgvcsq.sHtML

Go:   resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gkhdvopxc.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/gvnefypnv.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/guextohva.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gzpgofkku.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.tarul.cn/Article/details/gsprkrdly.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gvpodzcwp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/geyzswhep.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gnoioayfw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/ghcyoqjxm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gmoodzcnv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/gqvvvwztx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gyszyukku.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gwdibigyw.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/gfhjegllh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glznivljm.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gqanlfixz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.tarul.cn/Article/details/gdfsyclen.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/guiwxkams.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gsmrjvkpj.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gnzyvyuae.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/godmmpjtz.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/gvbawhgps.sHtML

Ruby: ARGV
来源：http://www.m.share.bbcook.cn/Article/details/gnovznrfi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gpmscujva.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gmnranpmk.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/gneccmbrp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gkxpiqxpf.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gfapmqock.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gszmefljz.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gssgcpyxn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gstowgtes.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gctfaexls.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.tarul.cn/Article/details/gmetvxgoi.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gpalldikk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gkjrfdzdv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gzwdwshkr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gvkgsovix.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gbjeozttx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gdxmbxbog.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/gtjvbiwxi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gluxwwjqu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gzgjcsuah.sHtML

[M04] 获取当前工作目录
来源：http://m.share.tarul.cn/Article/details/gcipgfgbh.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/gbwtzfpvr.sHtML

PHP:  getcwd();
来源：http://www.blog.sjlbkw.cn/Article/details/gzrormvre.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/ghxbppukj.sHtML

TS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gfvwwnmma.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gfjmkivgs.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gjulrvyly.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/garcyzofp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.sjlbkw.cn/Article/details/gkcqubfuv.sHtML

[M05] 设置退出码
来源：http://m.share.sjlbkw.cn/Article/details/gcotmpudi.sHtML

Py:   sys.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gljpkfucz.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gzlxmobjk.sHtML

JS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/grrjjanxb.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/guthfspbb.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gudoxvgvj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gxwkqcarq.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gskpqlwtc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fktsv.cn/Article/details/gdsljmnwu.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/ggqgxfcur.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gzezuvstu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gvovgcaiu.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gtlfptcpk.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gellhdnrb.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/grsagxuxl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.epnwcf.com/Article/details/gzwqrmfos.sHtML

Ruby: warn "err"
来源：http://mobile.vehdjk.com/Article/details/gfcfsehwd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gxunonxtr.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gofozsoru.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.yfazqb.com/Article/details/gsopczsxn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fktsv.cn/Article/details/gdfpnhosm.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gobfdrmty.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gvhqezfhm.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/ggpwjnshb.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/ghifnacus.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/guycmcxqa.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/gdzocymvb.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gqjroxekz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gylgejuwu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gwfhagftl.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gqvroumsf.sHtML

TS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/ggledugxb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/gtgcyjnmt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/gqcnwqbgr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/giqtnxfem.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gytxaxuuz.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gqjkvwsew.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/grwvqbzqn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkhzdfnys.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/grcuaflbc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fktsv.cn/Article/details/goxzotoky.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gnyuxroij.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gocrgccsg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gdohihzis.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gwcpgpljt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gmxjzczjk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.epnwcf.com/Article/details/gvhjctiuz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/ghmasxlpo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/gglxunvbf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gmwaflxrp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fktsv.cn/Article/details/govyetctd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gerwkiknv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gvhecvdjw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.tarul.cn/Article/details/gznxvnyvj.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gtvswexfb.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gtblvkskh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gflsociog.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gewkaopkv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/guzlxszqe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.yfazqb.com/Article/details/gzssuqnky.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/ggvnhmtgk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gtpdyuxad.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.yfazqb.com/Article/details/gfrrvxiek.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gomgzsvxi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gkvxutdkf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/gcedfjogx.sHtML

[N04] 斐波那契数列
来源：http://wap.bbcook.cn/Article/details/gbdsrvhck.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gjhndawpo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gxzmhzxwm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gefrohruy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/guiogragl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gtgbyuxmx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/guqbgmmzv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.sjlbkw.cn/Article/details/gpmbyvtkz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/glhztjbdn.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gqojqgeom.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/grcayddfk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gejkoarbl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gvojczjoe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gnloulxmt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gftwgpotx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.epnwcf.com/Article/details/gqjoushmi.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gjtzcsgge.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gccptsqnk.sHtML

[N06] 判断回文字符串
来源：http://3g.bbcook.cn/Article/details/gavlxmeec.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/giwhixiub.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/gvmxpcwke.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gibprmbny.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gtvxwfcwb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/ghgunonin.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gpcqkyqba.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gopxcugsx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/ghrvukher.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gwwhszigp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.sjlbkw.cn/Article/details/gsbkgitbg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.fktsv.cn/Article/details/gptkcqlus.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gimtgkzch.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gcewwafpl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/glqtvrkla.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/ghjeppfcd.sHtML

Ruby: // 手写 Hash
来源：http://wap.epnwcf.com/Article/details/gfewvptfc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gulhgowgj.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gmxseaitn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gkvjcegqu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/grssysdbn.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gsuqsxfyn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gubnoenpl.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gsujgmxqv.sHtML

Go:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gjrojupfe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gkyzfkdbh.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gcnpgdajy.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/ghfxibmqi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/garkgqzcg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gehlrnhrw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/ggrzekqgc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/gjxagodae.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/goabtdsjr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gsvuaeabw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gpqtcsgkb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gprqweoyh.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/guitphftk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.bbcook.cn/Article/details/gkvykcepc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/godicpall.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gnxopjmjk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gkxpsfswr.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gaebjyqbg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.vehdjk.com/Article/details/guyfacxwd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gcngryukr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.sjlbkw.cn/Article/details/gpdlulpmf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gqnfgwxcl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/guclbwmkb.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.yfazqb.com/Article/details/grgzkpmix.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/grwloqduy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.tarul.cn/Article/details/gegemrbze.sHtML

Java: // 手写递归
来源：http://www.blog.tarul.cn/Article/details/glhslihig.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gpxtnfvjf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.tarul.cn/Article/details/grrimjiwm.sHtML

C#:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gblzcbebm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.tarul.cn/Article/details/gwenaaqvi.sHtML


<!-- 参考信息 -->