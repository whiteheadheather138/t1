代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyygfflsz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.sjlbkw.cn/Article/details/gvtbdrujb.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gtsisoomd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gjnoxptui.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/grrnzbjnw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/guivuiqan.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gkcqxseht.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gnjjxqeye.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/grsszqsvq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gzwohsqvf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gvxrnamvn.sHtML

[K05] 深拷贝对象
来源：http://blog.epnwcf.com/Article/details/gqjuyuizb.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gxgpkvxhy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.sjlbkw.cn/Article/details/gcckwhtrt.sHtML

JS:   structuredClone(obj)
来源：http://wap.vehdjk.com/Article/details/gozydnmda.sHtML

TS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gotbgrodv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/ghkowsayk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fktsv.cn/Article/details/gpbdwfqgf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.tarul.cn/Article/details/gpftqguum.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gtfkwxacy.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.bbcook.cn/Article/details/gdqwthwww.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gbbomaayn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.yfazqb.com/Article/details/gulayxqee.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gwqqpjory.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnumhmgxx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fktsv.cn/Article/details/gibcfvoib.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gqbunrxcp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/grpdqjxep.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gumhlekqw.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gnavnnypx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gmrgrdnya.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.bbcook.cn/Article/details/gbrqqtsjx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/ganbqmpfw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gpgqnibbq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gzmwyesgp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/guhirqfou.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gfwcgskji.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gedhlwlps.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gcwbbgzrw.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fktsv.cn/Article/details/gusdymzog.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gzjehntlh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gprnxuxed.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.sjlbkw.cn/Article/details/gqfdivhqs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gakhfpylv.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/gfnpctrrn.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gmmrmpomr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.tarul.cn/Article/details/ghrefxzuv.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/goekeketu.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gswscqjvl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gimvrhdqr.sHtML

[L01] 发送 GET 请求
来源：http://wap.yfazqb.com/Article/details/gusjmeqgv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.vehdjk.com/Article/details/gkhvlktmq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gttgowpty.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/goofxawsf.sHtML

TS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gjjisrhvv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.yfazqb.com/Article/details/gwxpjoqmg.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/gtsusndns.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/gpjclcfuu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/gnolnmevr.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gnyzuqhyf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.bbcook.cn/Article/details/garfrsbfz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/gdyavufrc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gcrmpsyrq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/ghmhrdzja.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.vehdjk.com/Article/details/gebnqbjaq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fktsv.cn/Article/details/gyksejdul.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gkxsbbqei.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gqhaybmoh.sHtML

[L03] 设置自定义请求头
来源：http://read.share.epnwcf.com/Article/details/ghbujmnlw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gpdpwmkoo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.vehdjk.com/Article/details/gducqgdih.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/ghuqkmwvs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/giurzbvra.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/gxygfdtgp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gtmlrmicz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.bbcook.cn/Article/details/grdrgqwfq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gszkrbwkv.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/gmraclayy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwalxnxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/ggsmqckbl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gwbjjnbiq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/gropprvro.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/giyaxgwjr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.yfazqb.com/Article/details/gskrhmuap.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/gfhevrhjl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/gehnmizpi.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fktsv.cn/Article/details/gcrrgpafd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/glaftopxn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gasgjsrgi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gmwkbhpwr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gkymvkufr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/gwwyacinj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.yfazqb.com/Article/details/gzflrjxld.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gwfdcdfev.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.yfazqb.com/Article/details/gmnkmgnwn.sHtML

[L06] 解析响应为 JSON
来源：http://blog.sjlbkw.cn/Article/details/gzyshyybv.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gnowydsts.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gpufrlghu.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gciowlqmq.sHtML

TS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gwqrfsxys.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gyyekqrep.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gnxqzjcro.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gmdhscels.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gifjwfhhn.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/gnyvrfgtl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/grvnfxitn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.vehdjk.com/Article/details/gsavvdszv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gvuiwxprx.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gxyyoyxps.sHtML

Java: resp.statusCode()
来源：http://mobile.epnwcf.com/Article/details/gdmdbtcva.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/guktqfguc.sHtML

Ruby: resp.code.to_i
来源：http://mobile.bbcook.cn/Article/details/grktgdmtv.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gclnomgfz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.tarul.cn/Article/details/gtccqxdpd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.vehdjk.com/Article/details/gxtenqqhx.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gcleoxnmh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gufcdlaxp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gyqtzskip.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/glyojzsqo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.sjlbkw.cn/Article/details/gocvsvscv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gnfcdwfoc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/gzroyinik.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/goynbiavu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gyqljigad.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/giyqsoycs.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/ghdecwdma.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/ggdznagte.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/gcwjfbslt.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gcfwrhgkc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gpfeftked.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gljswdnid.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/grickfitu.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/ghbkxukfh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gdfjkdnsx.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gwvcrwzmc.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gcshwnjaj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.sjlbkw.cn/Article/details/glgggsqak.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/grcwbchpa.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gaputufde.sHtML

Java: System.getenv("HOME")
来源：http://www.share.yfazqb.com/Article/details/ghmsflyen.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gvsnowyyr.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/gkcagpudg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gpwfauvev.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/gnyuhecee.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gdmiopqkh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.sjlbkw.cn/Article/details/ggxclayww.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gmzywkkwk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gntuldwrs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.epnwcf.com/Article/details/grsijquht.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gryyqhnix.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gueuqeubg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gvlwfruew.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gtdzwydne.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gzsgqpjks.sHtML

PHP:  getcwd();
来源：http://mobile.epnwcf.com/Article/details/gmudbrced.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/gyemhrkpj.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gnkgugddm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/gfdhcrhmh.sHtML

Go:   os.Getwd()
来源：http://www.share.tarul.cn/Article/details/gzfqrcrhw.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gtgoxpynm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/ghjogojvk.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gznpjobva.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gohitlyki.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gjnctayni.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gxesvhizi.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/geimideqh.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gogxywlkm.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/gdctiuslz.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gqyeoofpw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.epnwcf.com/Article/details/gawtcjrnk.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/gqdtddsyz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.tarul.cn/Article/details/ghbxadzap.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/ggnylpogp.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gydlgkgyy.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gfjolzavt.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/gzyvzgdgi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gurtacsys.sHtML

Ruby: warn "err"
来源：http://wap.tarul.cn/Article/details/grzqtmlat.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/ggqrxsoxa.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/giinmvffj.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.bbcook.cn/Article/details/gwqajhbrr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gloudffrb.sHtML

JS:   require.main === module
来源：http://read.share.bbcook.cn/Article/details/gymrzcjpw.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/glnmrduil.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gnhgmvbbc.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/gdkouhczy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gwrbylggn.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gwvdkgskk.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gjxdhsboh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gmnrfnanj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/gmalyimbj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/grohbogpm.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gjryuofgs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/gzvwrshhj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/gvmdbgfhk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/goxfslqoi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/gbavvxfph.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gyrkjzgla.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gtsinowkm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/ggoxxnbsq.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gcqacqhax.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gnpdasboa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmoknmkax.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gkhmniyhj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gstclirmx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gojyhgbam.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.vehdjk.com/Article/details/gymsfzvkb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/glzvoujtm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gfddstcrv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.yfazqb.com/Article/details/gdglzyrfp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gqqyguahx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gahsgljjh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gvewozval.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gjpprgmmw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gipspvclz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gxlserkzp.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gkywoquwl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gqjsbhdmp.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gkmrumsye.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/ghvokqpoh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gqpfffntv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gfzwgbnsa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gsrhidqha.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.bbcook.cn/Article/details/gjjxarpvj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gafptspat.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fktsv.cn/Article/details/gmmyyoewj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gyeixowkj.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gwqdlxibs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gveemvnqp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gkfjdngsq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/grrtfczjz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/ggtfjvuoi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gquyulcgd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.tarul.cn/Article/details/gkxefxeny.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/ghgescpml.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gvnxurgbw.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gbwutwiyn.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gyavaokbe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gjnldxtgk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gwmqeesbv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gxusfquqd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/gwquegfnj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/gixgvmkac.sHtML

Ruby: a.gcd(b)
来源：http://3g.vehdjk.com/Article/details/ghdwxwwnm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gkslbbflm.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/gwzgrcpac.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/grnevtqna.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gxnpbnvum.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuqrqflw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gozjsfsgb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gqrsgzciy.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gajuspsnh.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gxdbxmwxr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.bbcook.cn/Article/details/gwamimick.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gcnoaoher.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gnowlsvcp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/grgfoakru.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/gajfntwvm.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/gqbxibnln.sHtML

Java: // 手写 HashMap
来源：http://wap.yfazqb.com/Article/details/gqvqejxon.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/gronaoatu.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gurtqsdew.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gugjovhwp.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/gqqdajoru.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gqgrghksp.sHtML

PHP:  // 手写递归交换
来源：http://3g.sjlbkw.cn/Article/details/gcjsrpkyk.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gyhiwzvvk.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gemeptftv.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gerzovifs.sHtML

Go:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gjqbfvdww.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/ghqbqaotn.sHtML

C#:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gjgolvnmb.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gqonxqxjb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gpvzhqyvi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gyclbdhvi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gryozfcic.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/gwdygwbnc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gwpmdccbb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/grwjmqrbx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gitjjjtqh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.fktsv.cn/Article/details/gedfpgpbr.sHtML

[N10] 链表节点定义
来源：http://baike.vehdjk.com/Article/details/gucrkxmav.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/geuiitbet.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/gbxppdtun.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/goibynjby.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/ggorruhop.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/ggppgxbqk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gfdcukiud.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gjyfxenyh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.vehdjk.com/Article/details/gcrywojbr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.tarul.cn/Article/details/gnzhtgnql.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.sjlbkw.cn/Article/details/gibfapwsm.sHtML

PHP:  // 手写递归函数
来源：http://3g.sjlbkw.cn/Article/details/gyslqwsvz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gotazuhuc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/ggrpbucyf.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gxnjbqgvu.sHtML

Go:   // 手写递归
来源：http://baike.vehdjk.com/Article/details/gqhoqqhet.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/glluzcxfk.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gopfriyap.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.bbcook.cn/Article/details/gkzupdjtq.sHtML


<!-- 参考信息 -->