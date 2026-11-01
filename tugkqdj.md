代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/gekeyytfw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gstgsyvqn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.epnwcf.com/Article/details/gwyzbjbrj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gfocrwgeg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/guhencwoe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gfqwfuxnb.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fktsv.cn/Article/details/grbimmjar.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.sjlbkw.cn/Article/details/glwfnschn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/glvvebxci.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gikpgwzin.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/giyojpsde.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/gkrkedmbj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gtdiosqrp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.epnwcf.com/Article/details/grdlybwvb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fktsv.cn/Article/details/gmhqokuef.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/guijumqnc.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.vehdjk.com/Article/details/gtusbmwbv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.yfazqb.com/Article/details/gdczmkxar.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gvngmxdqe.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/ggqsuwccb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.sjlbkw.cn/Article/details/geydpicxn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.sjlbkw.cn/Article/details/gtavuinbj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gvpeqhlkf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gpyrcblgx.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.vehdjk.com/Article/details/giimcrvbd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gcoljpppv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/gbzugzlrx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gzcxkarzy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gwncgufgf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gjgjvlvfd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gthlqzajy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gaeeraoqc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/ggadgtvnf.sHtML

[K07] 进制转换
来源：http://read.share.vehdjk.com/Article/details/ghpnvubkv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.tarul.cn/Article/details/gbzrwicon.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gvwkigqvw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gyckowsco.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.tarul.cn/Article/details/gfrzjpmqa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/glkvsiarn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.yfazqb.com/Article/details/gbvpsenxz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.tarul.cn/Article/details/gjpmtfvms.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gnlcrfcbw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhxykuzj.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gllfztrzn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.sjlbkw.cn/Article/details/ghuxwldaz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gchrqfgyg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gpywxdcpo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.bbcook.cn/Article/details/ghpckfhcp.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/glxnaenhd.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gutvrgawo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/ghhopoxix.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gzjsdcabn.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/gwiqrnafn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/grwurhtqj.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gzwdokuzk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/gsleqpkpg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.epnwcf.com/Article/details/gqcmzotxb.sHtML

JS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gebpmulbo.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gzdqzqdfd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gtpwradho.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fktsv.cn/Article/details/gjyamiwrp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.bbcook.cn/Article/details/gsqfosmcv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.sjlbkw.cn/Article/details/ghpbqmdum.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gugjmmqtm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gxmyyzewb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.vehdjk.com/Article/details/grosukwju.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gpsljtkrg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gqghrdwht.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gpztlfwbp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.yfazqb.com/Article/details/gnryppyjl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.sjlbkw.cn/Article/details/gfaknopda.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gwwadxqfr.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/ghfcjcyqg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/gtehosbyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.yfazqb.com/Article/details/gasarsdbv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/grijdttdo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gybtkadtb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.epnwcf.com/Article/details/gpsetfnrw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/grieendby.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.vehdjk.com/Article/details/gfkczxclm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.yfazqb.com/Article/details/gbmzhcizi.sHtML

[L04] 设置超时
来源：http://wap.yfazqb.com/Article/details/gitccqazq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gcgiojjla.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gssscxdws.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gbxzfuvji.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gxdoeconr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/gzfkshswq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.vehdjk.com/Article/details/gysrywfjx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gfwlhypaz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/grsmwrxlg.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gutkzrbur.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/glqgybqex.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/givvffsiv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.vehdjk.com/Article/details/gbrgsodyy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gnqygnidb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gamtegyhg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/galuytxvx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/gtnstsuxy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.vehdjk.com/Article/details/gxxjsqais.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/godcxxawb.sHtML

Py:   resp.json()
来源：http://3g.vehdjk.com/Article/details/gxdeekdpk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/ghlfzutur.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gqfkidqod.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gwodsaccs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gcqgadpnm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/gmlgcyjne.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gbvarmdqg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gmzzdabrc.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.bbcook.cn/Article/details/gmumsrfqk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gkldfeijd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fktsv.cn/Article/details/gsxcyvykl.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gcevsrsez.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gwpmzksvg.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/gpvyguuyt.sHtML

Go:   resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/gklvdwjkz.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/glukjrrxj.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/geadbqrkc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/ghtiaphoz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gcjlrpden.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gpbthzhot.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.epnwcf.com/Article/details/guklyxjgt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gpwkykgek.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gjjmglazf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/gvbmhkkii.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/gnmdatnky.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gdhsogwbp.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwlhhhstk.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.tarul.cn/Article/details/gkqmcooij.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gcppzpsbw.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/gumyinncv.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gvqevrhgz.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/glacesqzs.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gxgzgtkgh.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gescrzegj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/grdtconno.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gfeojrgtq.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gulobhyrz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gddqanlgp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gftmhnmeb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.vehdjk.com/Article/details/ggrhipfqg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.epnwcf.com/Article/details/ghrzdknug.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gwwahidlm.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gmebwjutq.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/grhvolgso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/goqqgrkgo.sHtML

Ruby: ENV["HOME"]
来源：http://wap.bbcook.cn/Article/details/gtdicqylt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fktsv.cn/Article/details/gebaqkvol.sHtML

[M03] 执行外部命令
来源：http://www.share.sjlbkw.cn/Article/details/gbzgnlayn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fktsv.cn/Article/details/gbhfgmsmj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gcvutgxac.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gcpjlgsve.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gwwcptbbe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gsvqwfsxk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/ghpgffwia.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gspbpagig.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.vehdjk.com/Article/details/gppuqtnsc.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/glcphxlao.sHtML

Py:   os.getcwd()
来源：http://read.share.vehdjk.com/Article/details/giokugraa.sHtML

PHP:  getcwd();
来源：http://mobile.sjlbkw.cn/Article/details/gzjkuizki.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gduiysfjm.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gpgvttoek.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.tarul.cn/Article/details/gjebfvime.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/gxzwygodb.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gpqkrxfny.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gkyvchxjh.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gxrhjjxqn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gphrphnum.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gbzzyuial.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/glghklaid.sHtML

TS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gretotcqd.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gerxoeemc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gmxkuiqqe.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/gngkmaihy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fktsv.cn/Article/details/gydyrerzg.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/ggdbhvvux.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gzbcytvbp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/gfcgutlzx.sHtML

JS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/ghfpapgyv.sHtML

TS:   console.error("err")
来源：http://wap.fktsv.cn/Article/details/gdcsbargp.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gwrwzjfsx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.yfazqb.com/Article/details/gacjqmoow.sHtML

Ruby: warn "err"
来源：http://mobile.vehdjk.com/Article/details/gzapnnojs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.tarul.cn/Article/details/gxvtcmtxz.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/guijwmcmt.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gusjcouks.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.vehdjk.com/Article/details/gkrosdprj.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gigibhrjl.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/guzmctwcu.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gqnycknhl.sHtML

Go:   func main()
来源：http://www.blog.sjlbkw.cn/Article/details/guuwwvvyo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fktsv.cn/Article/details/glpwkeqth.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gyqmkcmqf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gqhmzilqe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gkeahyoim.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gbxhopyha.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/glmnrtoef.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gktfylxer.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.sjlbkw.cn/Article/details/ghayiroec.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/grdirpxeq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.yfazqb.com/Article/details/gmujtxjzt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fktsv.cn/Article/details/glxmarbsx.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gzgexipqe.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/ggupyludm.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/grwxgtflw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gzuvkrjef.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gufjmwden.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gkvbmidzn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gpnkyzwdd.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gdtchegxc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/ggewfydks.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gcnzatxhy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/gtiexjmlr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gpsrfoclo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/gyyxxolcf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gjmryjduv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/geunqjnhw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gonfzzlhk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/gstfrrljf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/grdkexztm.sHtML

Go:   slices.Sort(arr)
来源：http://blog.yfazqb.com/Article/details/gxheccwnb.sHtML

Ruby: arr.sort
来源：http://www.m.share.yfazqb.com/Article/details/gkdfusagh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gsvxilxdk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gkvxbtdqm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gykyhvolq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/goeqfmumm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gsptefegq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gvsiddlog.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/gqwgbuntc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gezvmreuy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.bbcook.cn/Article/details/giqlhyxcd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.bbcook.cn/Article/details/gpthvirvk.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/gsgjzzshy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gnmsumqdh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/giwydcyot.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gtiognzeq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gsvqfsobf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gwspubnnb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gnjodwkhe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gohbljibp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gdbdmxpcx.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/gtzsguxsu.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gjmipceir.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.tarul.cn/Article/details/gicrkwadj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmszdjti.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gnulzxlnm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/gjsacfwvl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.vehdjk.com/Article/details/gfbkskdof.sHtML

Ruby: a.gcd(b)
来源：http://3g.vehdjk.com/Article/details/gifdduthd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gasaohqoj.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/giecvxcll.sHtML

Py:   s == s[::-1]
来源：http://baike.fktsv.cn/Article/details/gkawiwxnv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gazovgugd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/guaqxnaah.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gsjhcsjfb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.yfazqb.com/Article/details/gtrsobkzx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/gavlzqovq.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gaouwwsnw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gjdzggvel.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/gkazfxlya.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gqnqmnwvg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/ggiiwxpqv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/gnbtjxvad.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/ghokjidej.sHtML

Java: // 手写 HashMap
来源：http://www.share.tarul.cn/Article/details/gdigxqwex.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gohponwzf.sHtML

Ruby: // 手写 Hash
来源：http://wap.tarul.cn/Article/details/gkamoddfu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.vehdjk.com/Article/details/gevjmcpwv.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/gwsbtsdsj.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.bbcook.cn/Article/details/gbkpkmrlt.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/ghtxxupdf.sHtML

JS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/glazsluzo.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gxabejcnf.sHtML

Java: // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gpaavgyvl.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gavtfsygs.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/gbbqyxmro.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gwewirvlp.sHtML

[N09] 栈与队列
来源：http://m.share.tarul.cn/Article/details/ghpkvpolf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/ghlyfbhpq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gakhuxaso.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gkskntaau.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gqtkezdrt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gmguddvph.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gnxnybycj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gsmqwbekc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.tarul.cn/Article/details/gyktpglqz.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gksgqbrsr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.epnwcf.com/Article/details/gfdltpggd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fktsv.cn/Article/details/grgsjyipv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.bbcook.cn/Article/details/gwnplsyxs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.bbcook.cn/Article/details/gtelvajlw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gllgykgcb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gdvieawzr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.epnwcf.com/Article/details/ggbyejogj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gxphfjiry.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/grrqaepiq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/ggeynbxxp.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gxtxyurhx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/ggouhhqzr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gxhjezsla.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/gdfsqhllo.sHtML


<!-- 参考信息 -->