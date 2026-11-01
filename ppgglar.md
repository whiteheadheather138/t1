代发 wailian999

TS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/guhwrcxnt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.bbcook.cn/Article/details/gdjmupcah.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gwqaroynr.sHtML

Ruby: JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gxlaghwog.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/glebmyhoe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gxvbytiuk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.bbcook.cn/Article/details/gqsbpbdty.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fktsv.cn/Article/details/gftytwhju.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gvelkxfjc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/gbmlmunsm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.vehdjk.com/Article/details/gorntgmdn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fktsv.cn/Article/details/girfqjpzs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fktsv.cn/Article/details/grwwmcciq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.epnwcf.com/Article/details/gyqwekpox.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gjifogcfn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqiyrvuq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gurwvunjf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fktsv.cn/Article/details/glcnzbjah.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/grhiqnvyx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gojxuhidw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gdthjdnmy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gphlwlzzu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.bbcook.cn/Article/details/gtngqeaeb.sHtML

[K05] 深拷贝对象
来源：http://3g.bbcook.cn/Article/details/gcpsswnbe.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gaoxdqpxv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.yfazqb.com/Article/details/gcxknepxi.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/guxxrnhxz.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fktsv.cn/Article/details/gcwzfgpni.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fktsv.cn/Article/details/gfdbtjeva.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/gehswjqqr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/gkpumqumr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gawlsyrsd.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.vehdjk.com/Article/details/gcwmeizzx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.vehdjk.com/Article/details/ggaezjysf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.tarul.cn/Article/details/gvwfgfodm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/gwckxmkfj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.yfazqb.com/Article/details/giazuktkk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.bbcook.cn/Article/details/gukguvfzf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gfrcuuazt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gfdqjudxq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gcakaaemv.sHtML

[K07] 进制转换
来源：http://wap.epnwcf.com/Article/details/gptywmaow.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gzfrntlrj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/ghtjfvrsi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.epnwcf.com/Article/details/ghigjrjlv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gvltnurju.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gcprmqcmo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fktsv.cn/Article/details/gsxaxzzvc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/govbcqrgb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gjplavznc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.vehdjk.com/Article/details/gwvgtjfol.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fktsv.cn/Article/details/ghtqqobqs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/gkjmgzfgp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/geooubzfp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/ginmzkvav.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/gckpxuzdv.sHtML

Go:   encoding/gob
来源：http://mobile.fktsv.cn/Article/details/gckuemlmf.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.tarul.cn/Article/details/giafcnddo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.sjlbkw.cn/Article/details/gfgykjoix.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gmhsipvbr.sHtML

L. 网络请求
来源：http://3g.vehdjk.com/Article/details/gciwkdiio.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gzpzrvbro.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/gjpnabcjc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gschwximm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.bbcook.cn/Article/details/gzdajmjnd.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gdijrqlks.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gvcmksgtu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/gwjrisfdl.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.tarul.cn/Article/details/gqujvrrlp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.epnwcf.com/Article/details/gncecgizg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.vehdjk.com/Article/details/giefqthzn.sHtML

[L02] 发送 POST JSON
来源：http://www.share.epnwcf.com/Article/details/gjqpvvqxh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gxxrnfzjf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gsqseokik.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gngvtlpmn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gancbxhns.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbixpwzpp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gntvgxzqb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/gokzqrmpv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fktsv.cn/Article/details/gbfepznqd.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/gelqwbzxj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.bbcook.cn/Article/details/gnqozrklv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gpasjtojd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.vehdjk.com/Article/details/gsktitpfi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gryhynfoz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.vehdjk.com/Article/details/gppggirwg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.sjlbkw.cn/Article/details/gwircykzb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/gtjseodya.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gyqmtudkp.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gaolnhvnf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gvuoxswjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gpnmgkkit.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gkggoawts.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gpjtwtxem.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/glrfvgrst.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gbtlxnnqy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gdktzjuhb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.epnwcf.com/Article/details/gznevnnvj.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/gymaqewsc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/grfjldrqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.yfazqb.com/Article/details/gkjdgiukr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gyieocqsp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/ghxiucteu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.yfazqb.com/Article/details/gqkrwlclg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gvfzxszqf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gqarbrmwz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/gnayyxcvz.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.epnwcf.com/Article/details/gwjswraya.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gcycjdamy.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gbuajuvyb.sHtML

JS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gsqbxvlqg.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gkldwgmqa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/ggcgdgrse.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/gxyqyjsmo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gpdefybjj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gtlkjzvem.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.yfazqb.com/Article/details/glhcfawmb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.bbcook.cn/Article/details/gjcquujgx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gwmftswjd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gepgwrjme.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/grdcgwtut.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/giisdrmdo.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gfvstyohx.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gfmzubezw.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gaszxidpa.sHtML

[L08] 并发请求多个地址
来源：http://mobile.epnwcf.com/Article/details/gkjwnpkah.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.yfazqb.com/Article/details/gbexjryad.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.bbcook.cn/Article/details/gndmnnlhu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gcxopgtku.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gqkbxsboj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/gcariazfl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.bbcook.cn/Article/details/gvurignnd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/glozqblfb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gqzbjigvj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gnqvqmows.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.vehdjk.com/Article/details/gjpfyyciy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/glhpggieu.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gwoluagsm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gkxgrfxyh.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/gugppfziu.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/godmgfsrv.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/guawgdrpa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gkgbqpsbr.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gumfcajyy.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gcglynnkt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gfohzumib.sHtML

[M02] 读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gqhajygmx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gxydtwkxj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/glqhzyyrl.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/geliqwyhe.sHtML

TS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gwobtsoet.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/godbgbiob.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gxylzxwfh.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.epnwcf.com/Article/details/gegaukqfe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/geoxrnxeu.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gctpkebox.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gclyzznxb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gmqrdqnxq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.epnwcf.com/Article/details/gtfbqrqsi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.sjlbkw.cn/Article/details/glumvpbiz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/gqodfnixl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/gkoqltnwc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.epnwcf.com/Article/details/gxrmdcdit.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/gyzrahevh.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/gunexbwzm.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gtkwjoqct.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/ghxqtityc.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gbzcrklzd.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gwvksduxz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.vehdjk.com/Article/details/gjlykevew.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/gcfvpfgqr.sHtML

Ruby: Dir.pwd
来源：http://read.share.yfazqb.com/Article/details/gfcmdirjk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.vehdjk.com/Article/details/gcpdixckg.sHtML

[M05] 设置退出码
来源：http://read.share.fktsv.cn/Article/details/gdplyaujs.sHtML

Py:   sys.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gbinewvot.sHtML

PHP:  exit(1);
来源：http://www.m.share.vehdjk.com/Article/details/gizwasgkc.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gfehrboja.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gmgxjoyuz.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gqmtfdkjk.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/gekntnrte.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gltonuqmz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/gvduolxgz.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gyngdiuwb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gwdhzjerc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gagrrcdml.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gvvovmtjg.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/goyuudovo.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gcoofqxqf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gclcaovhh.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gijscpahv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/grnovzlej.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/goyucjmdk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gpyczkbzk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gliqewtva.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/ghhkoqxsw.sHtML

TS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gtqneptoy.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gwkznfhny.sHtML

Go:   func main()
来源：http://blog.tarul.cn/Article/details/gkhjgjbei.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gcklddaxb.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gbcjqogvl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/ggfuempli.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gwrnrgatf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gkdntfqht.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gqizdcatp.sHtML

TS:   process.platform;  process.version
来源：http://read.share.bbcook.cn/Article/details/ghjmmscrt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.sjlbkw.cn/Article/details/gzckmtukk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/glllzfdmg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gylgqwsli.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/grjttqqfq.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gjbhzjtwk.sHtML

N. 数据结构与算法
来源：http://mobile.yfazqb.com/Article/details/gltylqjvh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gpbyjvxun.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.sjlbkw.cn/Article/details/gezupcbxs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/goxuispdl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/grupwykcl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gllyyibsa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gvotuakcn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gtvbuizws.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gbouxpsof.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gmhcnehip.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gpuvecehv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/gtfyjtokn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gscmrgwuz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.bbcook.cn/Article/details/gsnrnvfnn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gmkuzfjsr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gloxkipai.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.sjlbkw.cn/Article/details/glwtfxtry.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gpdfbrzdn.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/geoyjxgwp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.yfazqb.com/Article/details/gqjpranye.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/gsxwwgiua.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gitzgddzz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.vehdjk.com/Article/details/gftszvugr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gatkartbc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gropxjxve.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gevzcpzru.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gfexlxmwm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.yfazqb.com/Article/details/gphmglams.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fktsv.cn/Article/details/gxyszzqjg.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/gpkzesdeo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fktsv.cn/Article/details/gctshffvx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gyhlxhpkl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gqatrkhfq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/goipskjkh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gbfvzzgog.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/glcwyfvih.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/grplpoecb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/govlvchlm.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/ggwbhigmk.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gmparzjol.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gwuiqvpoj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gfevyaczl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/guafttdgw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.tarul.cn/Article/details/gtjfxouvn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.vehdjk.com/Article/details/galcjdkcw.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gcbwlhdzb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gpbslymlb.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/gjbhmuupq.sHtML

Py:   s == s[::-1]
来源：http://www.share.vehdjk.com/Article/details/gbrbvdvat.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gicewijpl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gkyvlobes.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gqqxjzqum.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/gsosmmdml.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gqosaorkd.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gfgixrxxt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gybvujccf.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gnnfueymc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/gdzspyrfo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gpppfkduk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/grcjyblqg.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/gpaguocib.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gcdwnfxor.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gzlkxocxa.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/gdqfsihyu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/glasdyztd.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/gcorbhjrm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/geuljpcsl.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/guxgknyfg.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gfrqgktik.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gaieyhkng.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gctpelgfn.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/garghdirb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gpbgixrvk.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gsagettgf.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gcfoaqrfu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gbjbmnhss.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/ghmfbmfmq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gwrpleksd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gdjlnrlwj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/giujpsyld.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/ghbxfetrn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/ghzsytlei.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/gkjklttmn.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/goxlcpbjm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gvsdrfolg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gyaevetdq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gselsqkve.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/gyjnnxihy.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gtfcobcxe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.tarul.cn/Article/details/gnhaujffo.sHtML


<!-- 参考信息 -->