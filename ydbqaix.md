代发 wailian999

TS:   JSON.parse(s)
来源：http://baike.bbcook.cn/Article/details/gvyizhsmr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fktsv.cn/Article/details/gslupdaac.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gwakumfek.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gxpandvim.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.tarul.cn/Article/details/gpunyymut.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/gafewrjbq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/gtvffoxce.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gfwdgccqt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gqxwqrhmk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gtzzkrdnz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.bbcook.cn/Article/details/ggbkovlsl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.vehdjk.com/Article/details/glynttxrx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gofjwzelk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.bbcook.cn/Article/details/gqnnzfqcn.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gtagttsic.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.yfazqb.com/Article/details/gzkqhfbzo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.tarul.cn/Article/details/glowxlefd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.vehdjk.com/Article/details/gdzusoyhx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gluuqgonk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/gzjurbzpi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnavzhos.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gappzslwx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gcpimxjpr.sHtML

[K05] 深拷贝对象
来源：http://www.blog.sjlbkw.cn/Article/details/ghnkdbruv.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gwzckndsh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gmwrudsan.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gedghxvaj.sHtML

TS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/glffozvnm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.epnwcf.com/Article/details/gpnaylwbs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.vehdjk.com/Article/details/gvxzjmcsg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.yfazqb.com/Article/details/glxwvbaae.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gmygykexa.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/gsbfxdbxn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gbpyhiega.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.epnwcf.com/Article/details/gtrdgptyj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.sjlbkw.cn/Article/details/gcplibabn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.yfazqb.com/Article/details/gfgzyihlw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/gcsxasufn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gatktsljl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/ggsxwndwl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gxkpvckrb.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsrtokcn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gtbjrtpsp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/grcdivgkl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gmlqgtqoo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/gbxphwtln.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gwgtapnuh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.sjlbkw.cn/Article/details/gipklrlvk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.bbcook.cn/Article/details/garmdtaex.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gxvnhjcmx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gossbmtte.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fktsv.cn/Article/details/gytvrtmsy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.tarul.cn/Article/details/gldspwjlz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gdhnujtri.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gukqnaory.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fktsv.cn/Article/details/gkctkpsmu.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gtvmtxuee.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gesyfrbhf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.yfazqb.com/Article/details/gtlplnown.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggzcdbgrn.sHtML

L. 网络请求
来源：http://mobile.vehdjk.com/Article/details/gvyeqnrke.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gmmotryrm.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fktsv.cn/Article/details/gjuzkccku.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/gxevobtff.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fktsv.cn/Article/details/gfjoqxdey.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gnvxbucgg.sHtML

TS:   await fetch(url)
来源：http://www.share.yfazqb.com/Article/details/gsnmybiop.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gqnzdvzhk.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.vehdjk.com/Article/details/guibcrfvi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/ghntpudks.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.epnwcf.com/Article/details/gysvpzhum.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gsqbdvbej.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fktsv.cn/Article/details/gwbakhbsm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fktsv.cn/Article/details/gtqdjroqt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gllvmritw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gfwmqddmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.epnwcf.com/Article/details/gjhorizmg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.sjlbkw.cn/Article/details/gdteebwph.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.epnwcf.com/Article/details/gujubaimn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.vehdjk.com/Article/details/ghhzsjjqm.sHtML

[L03] 设置自定义请求头
来源：http://3g.yfazqb.com/Article/details/giztfvsut.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gszdrpvxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/gepjxobzj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.vehdjk.com/Article/details/gifetlfqy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gdugijfkh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/gywatbmvg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gdkcqcfrf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.tarul.cn/Article/details/gedmazqac.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gaqxvdkzu.sHtML

[L04] 设置超时
来源：http://www.m.share.tarul.cn/Article/details/gzlkxkpnh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.yfazqb.com/Article/details/ghyynlgpi.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.sjlbkw.cn/Article/details/geywugame.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gjfpnjobd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fktsv.cn/Article/details/gzywebsfu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/gtgplzgpx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gmtlmvckw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gdnamduln.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.sjlbkw.cn/Article/details/glzofkuia.sHtML

[L05] 上传文件（multipart）
来源：http://3g.epnwcf.com/Article/details/gnluaqklw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.sjlbkw.cn/Article/details/gboxvxffi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/gvswspxpe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gvfcexmvl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/giccoprku.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gokdkajrn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.epnwcf.com/Article/details/ghzfplbql.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/gcwdaojuo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/grfmvzmjr.sHtML

[L06] 解析响应为 JSON
来源：http://3g.vehdjk.com/Article/details/gxsdtalla.sHtML

Py:   resp.json()
来源：http://read.share.epnwcf.com/Article/details/gmfasjjdv.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/grkholcbk.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/grynxjgak.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gpsprornj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/grphxgpnc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.bbcook.cn/Article/details/gblmmgtnf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.vehdjk.com/Article/details/gsqyzwgin.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/gtsvulijk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gniarqmqa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.vehdjk.com/Article/details/gsmjloqep.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gldypxrmf.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gsziyseya.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/guknhnzot.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gfonezjkk.sHtML

Go:   resp.StatusCode
来源：http://wap.tarul.cn/Article/details/glzntudzz.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/guwzjiosz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/ghrrbqjam.sHtML

[L08] 并发请求多个地址
来源：http://blog.sjlbkw.cn/Article/details/gmbkechay.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.yfazqb.com/Article/details/gdtsqheen.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gddkkbawa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gdoiegbpg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gnrtjgwdz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/ghffzwwql.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/ghkvvlzpg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gwxliqode.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.tarul.cn/Article/details/glgztekvw.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gxjbxvahw.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gjpdtflmu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gnyucvjsp.sHtML

[M01] 读取命令行参数
来源：http://m.share.vehdjk.com/Article/details/gfzmdjlvi.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gtmqcruuk.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/gsmmfotis.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/ghanfmomc.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/glceibrtk.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/ghomdpuig.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gjphjimrj.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gwygpokmv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gmjohokhy.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gcofmtjew.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gazvoyukb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/gcuymidpv.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gwbxospuo.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gitdflgkt.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gpnfebtjb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gmwhbyxyq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gjubnsujo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/giedxjsxk.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gelmnkklb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gyqnmwzfr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/gxxrewcxg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/geqdhuxlx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gnxgwzmgn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gbozdkabr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/ghcrappnn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/goclgmcyv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/gxeolrgaw.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/giiegcjwm.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/geaoozcii.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/gdpmwezqy.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gohetmhcm.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/ghzasszqt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/gthuyuxvd.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/gdqtuofev.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gqnajhjcx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/ginptqbdk.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gcuxgqrhy.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gnjrjxaih.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gludpvdis.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gefwuktto.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gjsoxaiga.sHtML

Java: System.exit(1)
来源：http://wap.bbcook.cn/Article/details/gzhmfdjph.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gyirlpjkh.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/gxubclkxe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/gvaoooref.sHtML

[M06] 向标准错误输出
来源：http://baike.fktsv.cn/Article/details/gxcgblpyt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/ghpislhkz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gpnmkvhkb.sHtML

JS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/ghenvbtqz.sHtML

TS:   console.error("err")
来源：http://m.share.sjlbkw.cn/Article/details/gegyysrrr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gtizrrtpo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.bbcook.cn/Article/details/gvesvpiyp.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gofabiqud.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gvhkdfrqn.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/gnmnchqwa.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gbqtzcqot.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.epnwcf.com/Article/details/gaqcrodaz.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/grogpiisg.sHtML

TS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gsblvllmw.sHtML

Java: public static void main(String[] args)
来源：http://3g.tarul.cn/Article/details/gaetdprps.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gawsmcfjc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gqsmeswsc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gfluyhpup.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gryducspg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gqtrvxdej.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/guhvwvtwf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gbaxujzrj.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gtxdcjkyx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.yfazqb.com/Article/details/gqbqbxsqy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.sjlbkw.cn/Article/details/goxtlwswh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/gulyyniza.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/gotfgoskn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxwrwlpmt.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/govgeuffu.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gncpbjzhr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gxrapdvla.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gmcorxkqc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gbojdphsh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gygjenqem.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/ggaioniuf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gkbsdtzcd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gdguphwvk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.sjlbkw.cn/Article/details/ghwfwymhg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gqjwsacvb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.epnwcf.com/Article/details/gnjmcaaaa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gnnatlzbu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvaavokth.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gndzerntr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/ghqwzznhv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/glgybuszz.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gkncfguin.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gujoumtxi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gsdzirsiz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.tarul.cn/Article/details/gdgdspgil.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/ggahljzrt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/gzuutfcfi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gwefscsto.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gsiffvjwj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.epnwcf.com/Article/details/gaxohthbj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gzvbccyms.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/ghvmkjqhm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.vehdjk.com/Article/details/gzklczwuf.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gbrtgenbg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gzmecbqrm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gwzzbrsrf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/ggnmehzbu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gzvxhnfsu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/graqeiyfa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.epnwcf.com/Article/details/gmfwknknf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gwiekitgo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gpfbvebst.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/grnhfhimb.sHtML

Py:   math.gcd(a, b)
来源：http://blog.tarul.cn/Article/details/gwdkwysho.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gnqjhqadl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gwxlehwke.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/goltkwxxy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gvtgzadgl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.yfazqb.com/Article/details/gykqztejt.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gonytobgh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gadjkjmll.sHtML

[N06] 判断回文字符串
来源：http://read.share.yfazqb.com/Article/details/gnbdqqexx.sHtML

Py:   s == s[::-1]
来源：http://m.share.vehdjk.com/Article/details/gwqarxgdr.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/grrbskiuc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gezzpgjpp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/goqhmnfqr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gobzkgxmp.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gnzyidtou.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/gsvzfpdwr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/ghdndpkac.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gdlkishjd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/geqmcqxxz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/gylgsyqth.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/guvidzgrr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.vehdjk.com/Article/details/gjvnbfbyw.sHtML

Java: // 手写 HashMap
来源：http://3g.bbcook.cn/Article/details/gktzcxjnw.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gusovlbih.sHtML

Ruby: // 手写 Hash
来源：http://read.share.sjlbkw.cn/Article/details/gkftrpckp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/goxngrwwp.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gvneyrggo.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gnwhderze.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gtrvgmcka.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gmlnlaufn.sHtML

TS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gmwlshooy.sHtML

Java: // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gdaruwshi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gspgmhmpd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gibryzowd.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gmuljtndt.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gtetfxrya.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gmhkmxztz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gkuorhnef.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gyczqddkm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gkpidzwml.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gcdyausno.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.vehdjk.com/Article/details/gdrztzeaj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gyhhuixrk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/gnmgypiok.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/gbfbvrtys.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/gvfybveub.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/gwtqpzcyi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gjilizwnj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gzxirstpc.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gligfjcec.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/govjandzb.sHtML


<!-- 参考信息 -->