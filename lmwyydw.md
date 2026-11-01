代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/ggcezicul.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/gdlnpmtcu.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.vehdjk.com/Article/details/gpdetmkig.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fktsv.cn/Article/details/gapazrgnz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fktsv.cn/Article/details/gxfzbfbah.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gauycakqn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gxhojwdpd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gkypaowhs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gwnbnarih.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.vehdjk.com/Article/details/gtadeeyyp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fktsv.cn/Article/details/ghivmeiom.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gffzhhrks.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.yfazqb.com/Article/details/gagkxjphk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.bbcook.cn/Article/details/gkpqhwjme.sHtML

JS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/ganybhjnf.sHtML

TS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/grzjmgrcf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/gmjujfcgk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/godrorpof.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gluzqmvch.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/glqcohkde.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gvfgylffq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gbxsbigfm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/grtmjqpla.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gdvqmtlfg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gzwjqcxru.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gcyeaarar.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gpljmdyjl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gzcjgfzln.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gqshsvtbn.sHtML

[K07] 进制转换
来源：http://www.blog.sjlbkw.cn/Article/details/gmahohxjn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gorkwlvwh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.yfazqb.com/Article/details/ggjlrajhv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/ghhxjfzvc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gsampkdyd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gdhisufpx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gsntsexfh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gucocyyen.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gxilqjost.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/gvirmirku.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gragansrw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.yfazqb.com/Article/details/geslcoqsj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gxhezemka.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gzvwewlby.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fktsv.cn/Article/details/gxwfzqphn.sHtML

Go:   encoding/gob
来源：http://mobile.yfazqb.com/Article/details/gedcqmmwm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.epnwcf.com/Article/details/ggeboerer.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fktsv.cn/Article/details/gjcochwep.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gzlzgrmti.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gfultvjsl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gigydpqim.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/guqceodfy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/gfxvppdyf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/ghnncyujx.sHtML

JS:   await fetch(url)
来源：http://3g.vehdjk.com/Article/details/gnkovcmjo.sHtML

TS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gltclzkqi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.tarul.cn/Article/details/gssgiopkp.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.yfazqb.com/Article/details/gqxpaxicn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gcneeqbxp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/guwrgnytf.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/grjbcqzve.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gvbkfwuon.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/gapiiecbt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gdoitfalq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gccumqysl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.sjlbkw.cn/Article/details/golvpzrrp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gakfuadmq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/gcrjwkzmo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/guogcwqrb.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gpsxvjngl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.sjlbkw.cn/Article/details/gqcnaclwr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsppbmbe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.yfazqb.com/Article/details/gtqrynkur.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gzilncwah.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/genkikskx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gzngnjnja.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/glrfpjnvz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gdsopabcq.sHtML

[L04] 设置超时
来源：http://www.share.sjlbkw.cn/Article/details/gtlhjeykc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.vehdjk.com/Article/details/groxndzfo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gbcwknzdb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gtzsnnwmy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gwpfsgbdg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/gbebhwncc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.tarul.cn/Article/details/gqtrhlwpz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fktsv.cn/Article/details/gdfszstyc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.yfazqb.com/Article/details/gjikzyuto.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/gndrzczxi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gqbvcobyw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gkxasktiy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gshafpavh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gehkbntzn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gdaxqksmy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/gntnzlebp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gbtfmcerg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gplkfprji.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fktsv.cn/Article/details/gwtlgrxhy.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gfxnrxmdl.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gvolkyyxd.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gyyjopwas.sHtML

TS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gjqdsqgie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gnginwtqa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.epnwcf.com/Article/details/gocuqkrko.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gjyqcgjjc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/ghijuxcka.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gedjxdacz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/ggxpetvld.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/gxgrpfyok.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gtdqupzgg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gjdhdbtos.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/gzlaaryxr.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gcypugwnm.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gxuyfsuuv.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gfgcomsfo.sHtML

[L08] 并发请求多个地址
来源：http://wap.fktsv.cn/Article/details/gmqtzitjv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/gtqeaqbpa.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/glbvvltxe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gmczzelij.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gmkukfqcq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gujhjgsng.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.sjlbkw.cn/Article/details/gxrkyxawm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/gbrchnwjy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtthvlby.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gyvyxkajy.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/godgrrede.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/glxaetosa.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gzazhveuy.sHtML

Py:   sys.argv[1:]
来源：http://mobile.epnwcf.com/Article/details/gifpejcdh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/gthhkegul.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gywkuluda.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gozlovlbf.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gnelxylzt.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gzwuwefeb.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gktczlyut.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gvuhqqqlw.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/glrmcttxp.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gbgqxweks.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/gdeuxqyca.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/grmcpuzbs.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gxugcvruu.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gyknnofpe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gzlndbxbv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.vehdjk.com/Article/details/gkcrtxpgq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gskrykfgd.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/ghytoaqog.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gaoovzhhb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.epnwcf.com/Article/details/gdzwbifez.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gqyhmcrdl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gapucuimz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/gpdyovsqc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gpddiwtja.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gxblzjzxq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gxwbttnfa.sHtML

[M04] 获取当前工作目录
来源：http://3g.epnwcf.com/Article/details/gnxlonzli.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gtvilldnd.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/gszhhxzbu.sHtML

JS:   process.cwd()
来源：http://baike.bbcook.cn/Article/details/gjjvazmov.sHtML

TS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gkxmmdsxm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.tarul.cn/Article/details/gktzjgngf.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gsnzcofrj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.sjlbkw.cn/Article/details/gasafkgnc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.epnwcf.com/Article/details/gagcdkprp.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/ghjabufdj.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gaxzezoxq.sHtML

PHP:  exit(1);
来源：http://www.share.sjlbkw.cn/Article/details/gnecdsaeg.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gsvhaunwe.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gqhouajzi.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gqmvkfwqv.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gbbcpldix.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/gxzfnuwwj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/gxukrosog.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gzmemphxk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/gxoqdiqku.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/gfihxisuv.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gvaokhwao.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/ggpizxukt.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/giwxloaly.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gvuourtam.sHtML

Ruby: warn "err"
来源：http://wap.fktsv.cn/Article/details/gygtrrggq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/grylqjycc.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/goxvjpcjm.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gnazikpte.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gdajquyck.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gadbuhblh.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gdanhebin.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/gywoidkrq.sHtML

Go:   func main()
来源：http://baike.tarul.cn/Article/details/glbwwtzwg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gmsuxccnd.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/glixfaqnz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/geogcdtof.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gljodsfud.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/gtoismyii.sHtML

JS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/grluarnnn.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gxsxcosbn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gmuwqglcu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.tarul.cn/Article/details/gcznokvmi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.yfazqb.com/Article/details/gawynalzl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gyxeldfkf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsxzoxwzr.sHtML

N. 数据结构与算法
来源：http://3g.fktsv.cn/Article/details/gcrunhdgq.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqfczgwiq.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gvayiyflr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gmhjhvihf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gezhkbbxt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gpgycfvwf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/glxsqrssa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gtwcmbjve.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gtrcrqgob.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gjaecpiuk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/grkbphldx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/gfoidbuxr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.bbcook.cn/Article/details/ghbyffeso.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gfnvsfykm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gymothohu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gmslfbrto.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/gqbehxhaa.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gbvecypfh.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gqnxvnkrt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gwjjjgapi.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/guntxrsvw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/ggjqbumci.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.epnwcf.com/Article/details/glbouqbda.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gxaizupzm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/glhtxlnpw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.vehdjk.com/Article/details/gckojqrsl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/gereasneg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gnfzoluet.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gahzcpwux.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.epnwcf.com/Article/details/ggjfyodcg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gbagurgyg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gufiytwwa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gqgfrocwg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gurinfhfx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gkxzshnub.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/ghuqwciyz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gcqvptlyj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gtdpwfetb.sHtML

[N05] 最大公约数
来源：http://mobile.bbcook.cn/Article/details/gqumvbloh.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/goaclcctf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/goadadxcn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gcoqbyipw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gpvsykgqi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fktsv.cn/Article/details/gzlznnuhy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/glggjxurl.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gdgpqxjjq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gkddnsibo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gzbflipad.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/gsllznvuq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmfytxfn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gksyvpths.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/ghzaobpci.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.vehdjk.com/Article/details/grrwykyoi.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gggceclld.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gyxhnbmgf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/ghgbxafxx.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.yfazqb.com/Article/details/gmkcvrypl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/geylkilqa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/glgwizlon.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gqbkcjdqz.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gbtjzphnk.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gcjjkteke.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.tarul.cn/Article/details/gargeyxzc.sHtML

Ruby: // 手写 Hash
来源：http://baike.yfazqb.com/Article/details/gbdkharxp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gmkxvouaq.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/gaiyyinht.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.vehdjk.com/Article/details/gocdmxqsu.sHtML

PHP:  // 手写递归交换
来源：http://baike.vehdjk.com/Article/details/gorrjrcsu.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gvxnyrbda.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gqifhwqbt.sHtML

Java: // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gmmeufnei.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/goiccpgov.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.bbcook.cn/Article/details/gbtuizint.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gzqnbpgrz.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gfzepllhw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.sjlbkw.cn/Article/details/gmmhfjmqq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gseiwszjx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/grulverki.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.bbcook.cn/Article/details/gdmqihfxf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gvbhuxshg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.sjlbkw.cn/Article/details/gsaanssjq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/gubsgosoq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.vehdjk.com/Article/details/gtucktfbk.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gjyjnxmyk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gjyxdmzls.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/glzdjldwp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gjvhvudap.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.epnwcf.com/Article/details/gqiueobkp.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/grwlwbuhw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gejhiqlsi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/gtkpsimph.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.epnwcf.com/Article/details/gczfjxqqk.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/gmsqdherf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gnenqyocl.sHtML

PHP:  // 手写递归函数
来源：http://3g.epnwcf.com/Article/details/gxdnstadl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gersvmaqx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/ggzmwxaat.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gewivypie.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gopvrnaym.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/glhlsrdri.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gnicrfbam.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gqtgogbkz.sHtML


<!-- 参考信息 -->