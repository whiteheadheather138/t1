代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gulbualzf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.yfazqb.com/Article/details/gmmozwcqg.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.vehdjk.com/Article/details/gjlojkmlf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/grqoonovd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.yfazqb.com/Article/details/gqbianwtg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gspuyuevv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gbzkmzclg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gaoaqgcdb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gmyayakma.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gcvpaqylz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gnonkbhuh.sHtML

[K05] 深拷贝对象
来源：http://wap.vehdjk.com/Article/details/gxazimyue.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.yfazqb.com/Article/details/guwjvvpap.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.epnwcf.com/Article/details/gnketsjbd.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/ghtzmnoth.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/grekhtowu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/gnnmijwyv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/gckgwjbcf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.bbcook.cn/Article/details/gwzqxicqf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/glkyhyjgs.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.bbcook.cn/Article/details/gbnzvpbns.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/goinuxssz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/gzunvywyr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gymmsllzn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.vehdjk.com/Article/details/gsndxrlnz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.sjlbkw.cn/Article/details/gwmywgsre.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.yfazqb.com/Article/details/gbydjkvbe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/ghovgjndy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gsvmtkyrn.sHtML

[K07] 进制转换
来源：http://blog.bbcook.cn/Article/details/gorczexpp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/ghpppyrwt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.vehdjk.com/Article/details/gzakasphc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gccafsgjx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gxjzubqiq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gedrbuhri.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/gvdpilqqr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/guxfalbcn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gsrivjdvc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.bbcook.cn/Article/details/govzbelmq.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.bbcook.cn/Article/details/golyyausj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gyohgbwty.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gaducrdrz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/grrwiddib.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/ghxstrrqa.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gpdhvgrpe.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.bbcook.cn/Article/details/giwfzixfs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gynscizmx.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gganzuhjg.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gjkrkuwce.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gqgfubqaj.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fktsv.cn/Article/details/gewbbyuct.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.tarul.cn/Article/details/gehiwrftx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/gkjabxdhy.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/gdhzsfaly.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gcyopfemo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gokpmqupv.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.sjlbkw.cn/Article/details/gejfomhoo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.tarul.cn/Article/details/gdnomxtso.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.tarul.cn/Article/details/gqjudqquc.sHtML

[L02] 发送 POST JSON
来源：http://m.share.sjlbkw.cn/Article/details/getldcrwg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fktsv.cn/Article/details/gudaimdmw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/gauomtxdm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gglcaqnme.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gwhiuzrjc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/gmthqjkyf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/ggzllftsq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.tarul.cn/Article/details/ggerjaesg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.epnwcf.com/Article/details/gelxgvyjv.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/gzgqxmfsi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.tarul.cn/Article/details/ggiikdats.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/ghelldniq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/geswlojrq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gruvxxpec.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.epnwcf.com/Article/details/gswenshrm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gxletxhku.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.yfazqb.com/Article/details/gxcveenrr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gxwqoyrvz.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/gclychokb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/goeljspst.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gauonxwnq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fktsv.cn/Article/details/gqbxtusyr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gxdnhqqzp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/gvncyrpwn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.epnwcf.com/Article/details/gqsjmknge.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.bbcook.cn/Article/details/gbktqxmmu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/gdhfusrmw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.bbcook.cn/Article/details/gjcyzyxdb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/glqbnjshi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.sjlbkw.cn/Article/details/gogpkyunv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gqbhefeho.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gpuhhadyh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/ghakenxkq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/gpkkvtkyk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gpbqihsgw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/gwxomucyo.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/gnaareusr.sHtML

Py:   resp.json()
来源：http://mobile.sjlbkw.cn/Article/details/gyacwtceb.sHtML

PHP:  json_decode($body, true);
来源：http://wap.epnwcf.com/Article/details/gqeytjkko.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gqcmuhzyh.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/ginxusiha.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/gwzijaugs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.bbcook.cn/Article/details/gslvrshuh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.bbcook.cn/Article/details/gmxcwxocr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.sjlbkw.cn/Article/details/gsmlonkwa.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/geikvmirj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/ggxhgcoav.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gtitgvcww.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gtfhorrjs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/guvqaiokc.sHtML

Java: resp.statusCode()
来源：http://baike.yfazqb.com/Article/details/gxxbvjayh.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcxnesdn.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.tarul.cn/Article/details/gcpfwsdul.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gygylgrno.sHtML

[L08] 并发请求多个地址
来源：http://3g.tarul.cn/Article/details/gwzbgydmj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gvtccueqo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gkcxhzext.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gcyhnetie.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gvlactlec.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/gzqzyzgjf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gupguhagm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/golxukvbh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gsyzwbmmn.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkkxjlzmj.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gklrwpyqd.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkgziryfy.sHtML

[M01] 读取命令行参数
来源：http://www.blog.tarul.cn/Article/details/galnxynnu.sHtML

Py:   sys.argv[1:]
来源：http://blog.sjlbkw.cn/Article/details/gzpbgbpij.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gtashkeuu.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.tarul.cn/Article/details/ghpxkoloa.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gstsdztym.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/glitetzfm.sHtML

Go:   os.Args[1:]
来源：http://www.share.epnwcf.com/Article/details/giswtlill.sHtML

Ruby: ARGV
来源：http://3g.sjlbkw.cn/Article/details/glmiwubxt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/gxvjecolg.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gshcfejfu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/geqyzefhd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/goazxtklu.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gpcersikp.sHtML

TS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/galwvqtjo.sHtML

Java: System.getenv("HOME")
来源：http://3g.yfazqb.com/Article/details/gxhfmuqiz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/grmwmxngw.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/guibmxfxo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gujmgzpdb.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gtbfndpxc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/guwcqveyk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gkjqfaayq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gkfguonhk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/ghbnsajrd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gtojbhldm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gffjlqfuk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/gcmmkqbwd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gwfbgxlka.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/gvyxrxwzt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/guhaprrnu.sHtML

PHP:  getcwd();
来源：http://wap.sjlbkw.cn/Article/details/gdglbfyjy.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gpibxzxnk.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/ghbdylybs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gtlvtaskr.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/gbxqjlsmc.sHtML

Ruby: Dir.pwd
来源：http://m.share.epnwcf.com/Article/details/gcpiazach.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gdorxrdwy.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gjrsomfuv.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gwpocukaq.sHtML

PHP:  exit(1);
来源：http://3g.epnwcf.com/Article/details/gmddhemeq.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gqvdrclwa.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gxmsiaixl.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gnjoprzsp.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gzsxctrua.sHtML

Ruby: exit 1
来源：http://read.share.sjlbkw.cn/Article/details/gdweedzrs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.tarul.cn/Article/details/gbpyxjiey.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/glswocogj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gnwbqbkfn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fktsv.cn/Article/details/goukrwahk.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gzdoyxebi.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gepyzyxnd.sHtML

Java: System.err.println("err")
来源：http://blog.epnwcf.com/Article/details/guyjgrpkf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/ggedqvgkv.sHtML

Ruby: warn "err"
来源：http://read.share.tarul.cn/Article/details/gltfwlkcn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/gqbrfxfuo.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/giqmhwhnd.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/ggmjlebsk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gxjzrdktf.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/geosdsdaz.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/glkwrbflr.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gvytbvdxy.sHtML

Go:   func main()
来源：http://read.share.yfazqb.com/Article/details/gjixajlna.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/gbjzuzqha.sHtML

C#:   static void Main(string[] args)
来源：http://baike.vehdjk.com/Article/details/ggopqgfsw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.yfazqb.com/Article/details/gxbloijbq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gddtbikld.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.bbcook.cn/Article/details/gxgytxgeh.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gvrrulemo.sHtML

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/gxwzunybs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gwwoaxhkw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/gdyphgysk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.yfazqb.com/Article/details/gnezejkhh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gojqmrtjq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ggfzqmqve.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/ghgdutiva.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gfdlpgrih.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.tarul.cn/Article/details/gzkgvxhav.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gajgjulhm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/glnxlkfzn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gqglyhonx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gxsghuktv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gbpjkkifm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gueydmqmb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gdvsiljme.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gbtldotad.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/gqhaqebzu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/gcggezibu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gqiuaicvg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gomxdwdff.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gfczhgdqj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.yfazqb.com/Article/details/gpvalfzkl.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gvpnkuhgg.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gwqyrikgm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.vehdjk.com/Article/details/ghyhsmfsj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/gqiwszrvj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.yfazqb.com/Article/details/gzgvfugev.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gewvxjchn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/glvitkoem.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gcpftaiwc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gdsnxhbjm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.vehdjk.com/Article/details/gxluoewnx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/gnasaqkzm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gwnvjfjmp.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/geykhskkm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gcyzzlodt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/gcgumtshn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gokznerkn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gggtxyfdy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/ghyuiwdei.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gdjyoouul.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gwwgzdudx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gfjkajicd.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/gipzyvdgh.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/gldsloour.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gmkynwjfv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gmjuqmnws.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/geouckokw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gxlrisltj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gemqcwcop.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gugrlbtjh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/gxirvqcfi.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/giwkmboob.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gmtvccfws.sHtML

PHP:  $s === strrev($s);
来源：http://blog.vehdjk.com/Article/details/gibyqdwsk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gkddvrowz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gdptqirkb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gdcdpabhb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/grjxjjyyy.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gwnaxuqjw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gursjmpwq.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gcrqzsjgl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.tarul.cn/Article/details/gfhgpnfvg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.sjlbkw.cn/Article/details/gfgqhioou.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.tarul.cn/Article/details/gbvuyrccr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/gicnxticu.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/gwlsjhhhk.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gvsbrkcdr.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fktsv.cn/Article/details/gdpksctwo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/gunvxhijb.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gkrauhvka.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gyainyosz.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/govkecvrq.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gscpkueqp.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gpcqmgizt.sHtML

Java: // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gxawudgpp.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/ggitznitb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/ghdhtmpsa.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gsmrejcxz.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gnjnxtclo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gpmwcroht.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gdtzndpdg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gsuaxexvj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.sjlbkw.cn/Article/details/giofogyte.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/glmyunwix.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gnhbejhuj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gplsjzyut.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gkfdglrae.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gjphcmjbt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.bbcook.cn/Article/details/gznlnfarl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.sjlbkw.cn/Article/details/gohrqzvgq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gjhekfked.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.bbcook.cn/Article/details/gezabdzkm.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/gxpoipiic.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.epnwcf.com/Article/details/gzlhdnezc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.vehdjk.com/Article/details/gypvatfku.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/gankrvnha.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gaxntzrco.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gavmqllpl.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gwnwpslvb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gldocxetz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gjbbjmgxk.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gsoilrhux.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gdkoxbvtb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/ggcjjwwgo.sHtML

C#:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gvquwhopk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fktsv.cn/Article/details/gnnnbtqpv.sHtML


<!-- 参考信息 -->