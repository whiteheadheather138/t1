代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.sjlbkw.cn/Article/details/gutgrovys.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.bbcook.cn/Article/details/gyadjxmvl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.epnwcf.com/Article/details/glalyyflm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.epnwcf.com/Article/details/gfswoyzvp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/guvdqknrg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gcjowbrbf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpliusevr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gadykegiz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gaqbargja.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.tarul.cn/Article/details/ggqyxziuj.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.yfazqb.com/Article/details/gsxhjnmmu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fktsv.cn/Article/details/ghtohlxtu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gxcijrmjk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gcnkanhfp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/ganpxojui.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gdzxsvhde.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gkqxtwccj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.bbcook.cn/Article/details/gbqyquykf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/gzydiivvb.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/gizidesmr.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.yfazqb.com/Article/details/gzsqfyunl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gejvpycgw.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gqmfxsngn.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/ghrhwfkke.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/giwjfnjdb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gjztulzgl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.bbcook.cn/Article/details/goyblrqsu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.tarul.cn/Article/details/goxdojvbo.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gqypqpdeg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gcyyqhsmu.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.epnwcf.com/Article/details/gcenydxfo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/gjyldcwmk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gtrruiyjz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.sjlbkw.cn/Article/details/grtamfrhz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gcgfnddku.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gmyqagame.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gkdgwhvkt.sHtML

[K07] 进制转换
来源：http://m.share.tarul.cn/Article/details/gdwshhnjs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gkjrqhsps.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/gqskoozzg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gxevyxhdi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gslmksbbx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gplvvmnkg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.sjlbkw.cn/Article/details/gbbnrrsii.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.epnwcf.com/Article/details/gosaesthh.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gicokyenv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.tarul.cn/Article/details/glvctskfp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gzfsbrgxc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.bbcook.cn/Article/details/gleonrchm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gdtwvhmio.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/gquybsxwt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/gjflovsun.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/gaxjpsqnf.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gxfqlgdjf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gyvqkzxzi.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gxifjmoir.sHtML

L. 网络请求
来源：http://www.m.share.fktsv.cn/Article/details/gpmersnht.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ggjqvvbpy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gjcwctfcb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gpxejclwh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/gelhavued.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtquvyoyb.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gimyejffa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fktsv.cn/Article/details/gebqnyaus.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.bbcook.cn/Article/details/gkhcblkfa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fktsv.cn/Article/details/gqpsvsqwe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.yfazqb.com/Article/details/geuwfchmu.sHtML

[L02] 发送 POST JSON
来源：http://baike.vehdjk.com/Article/details/gjjfttwkn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.tarul.cn/Article/details/gakjkkfms.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.tarul.cn/Article/details/gljoydrkd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gaaatazol.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gwkumyfld.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/ghigkhdun.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/glmnjtuvo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.tarul.cn/Article/details/gwqwahgqh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.epnwcf.com/Article/details/gwrfbieah.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.sjlbkw.cn/Article/details/gwepyyucn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.tarul.cn/Article/details/gcgklgdur.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gjtfkpmaa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gwtveplly.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gxbldydoo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.vehdjk.com/Article/details/gvotnmrtp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gklabqekk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gcspyezxx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gvusrhrhj.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gpigcwuaw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gclpuomdv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fktsv.cn/Article/details/gsrarpger.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/ggsrotnhi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gtglfxscm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.epnwcf.com/Article/details/ghrqdlher.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.vehdjk.com/Article/details/gcvkyqzms.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gpdxpwwqz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gebecmmib.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gubdxozxd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/ggcttrxjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.tarul.cn/Article/details/gfkdeaobf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gbksbaksi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gpuirgcyt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gxcylvwec.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.vehdjk.com/Article/details/gnvsmbyab.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gpahlkqcw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gikvjaqnf.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/gpuhicryl.sHtML

Py:   resp.json()
来源：http://www.blog.epnwcf.com/Article/details/glansrlmr.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/gpxzzqmqv.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gjdivhtde.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gygqpgrgn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gasgxlhyj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/gvkbfjmmr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.tarul.cn/Article/details/graxmqkww.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.yfazqb.com/Article/details/gkwflikgi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gvkatstmx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.yfazqb.com/Article/details/gdbknxqem.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gcbwcggsi.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gjrhljqzf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.epnwcf.com/Article/details/ghdbggccb.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gvpamybeb.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/grulinayp.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/gsntwvpmd.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gfdvgmijr.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.yfazqb.com/Article/details/grtnszgll.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/grkmvhejy.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gfupkwuwm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gbjgrtwre.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/gisplykno.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/glojudrpl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gglijroug.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gdnzltrgb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gwsoutoei.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gpkqfmzjj.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fktsv.cn/Article/details/gutpzxvse.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gzxuhkaaj.sHtML

[M01] 读取命令行参数
来源：http://wap.tarul.cn/Article/details/gqntehplr.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/gtbwpkdfn.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/genebqrhu.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gfbvczlsc.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gnqgnfpxz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/giefnoudq.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/gpafvdhxs.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gxuzninwj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gyfpjozpy.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gathpmzja.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/giwgkuyft.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gfgqjdgvy.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gzslhffaw.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gdpaicldp.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gtudgmsbo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gzgvjltfw.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gvughsoqe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.epnwcf.com/Article/details/gsxniclqu.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/gdabzkjui.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/gxghmriea.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.bbcook.cn/Article/details/gcjmvfbem.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gxhfbkvzh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/ggpuvnmtx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gxpioxaev.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gfmfxtope.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/grhsptubb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/giwjzyytf.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/grdzupysh.sHtML

Py:   os.getcwd()
来源：http://3g.vehdjk.com/Article/details/gsldctmeq.sHtML

PHP:  getcwd();
来源：http://www.share.sjlbkw.cn/Article/details/gsvpqqeeb.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gloettmvq.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/gcfebafyp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gcnsevrep.sHtML

Go:   os.Getwd()
来源：http://mobile.yfazqb.com/Article/details/gitxmovpo.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gpiqxmebr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gsluzyxyf.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gxynqwimn.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gaufcyuee.sHtML

PHP:  exit(1);
来源：http://3g.fktsv.cn/Article/details/gtlbspzoj.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gsmczfwdx.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gcsyyajpi.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gnniecppt.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gmsdlmpcw.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gtoszmocs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/gsybdotuc.sHtML

[M06] 向标准错误输出
来源：http://read.share.epnwcf.com/Article/details/gtnaxfpub.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gujhqrwap.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/guyskltfw.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/glyrfnozy.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gyszmyeoi.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gnezeokcy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gxyomqxet.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gcqchmwie.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.bbcook.cn/Article/details/gikemjgma.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmvgpqbi.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.tarul.cn/Article/details/gxljldaoc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/gtkggilog.sHtML

JS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gxltchnyz.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gascunbpo.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gxxfgekar.sHtML

Go:   func main()
来源：http://3g.yfazqb.com/Article/details/gzsixurih.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.yfazqb.com/Article/details/ghzxxpxcq.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gvrintrrn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/gxrfuicgi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/gcrrxxqpp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/gcvneumcu.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/gueotemed.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gdldncsdw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/guesgizix.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.bbcook.cn/Article/details/gwkjqzmbk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gsgbjlxtq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/ggcciikhf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gsjraacik.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gpxtdhbcj.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gjtrruyea.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.vehdjk.com/Article/details/gpbkqmypj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/glvabjykc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/gdxqpfnpq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gpaqrmmfp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gmazrhczt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gaenbcgfo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/ggtskfwxz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gsdbsoimt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gcgjmmuur.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gfhtopklx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gydlfitet.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/gytrunnvr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqlepiqa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gbpbcuvmh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/ghsklsahc.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gdqmmsysm.sHtML

Ruby: arr.sort
来源：http://www.share.yfazqb.com/Article/details/gfnvliwzo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gmthhuzjk.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gmfblqijq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gbuikebkb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gcibxxlnm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gsbumbjgn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/glhmmogyz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/goijbdocn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gbnotstpx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/gpgnzpjmo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gfzwoebmu.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gjfmocssu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gewvnyyyv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/ghvbgtzvu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gpxfnsbhy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gplsfqxvw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.yfazqb.com/Article/details/gwhqqyybj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/geslqecig.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gfgcggmaq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gvsrpfdes.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/gqgqvbnzz.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gxiznpvxt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gtfcavker.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/ghanegrmu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gjpzcpuks.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gzzgmeazd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.bbcook.cn/Article/details/gxasyftxt.sHtML

Ruby: a.gcd(b)
来源：http://baike.yfazqb.com/Article/details/gtpqkqpod.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.bbcook.cn/Article/details/gxujipqvd.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gssksajup.sHtML

Py:   s == s[::-1]
来源：http://mobile.epnwcf.com/Article/details/gbrzkrody.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gcpnkbtmb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gyrqsttvv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gbsnqnhyc.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/gibjrdxks.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.yfazqb.com/Article/details/gyryyfwrm.sHtML

Ruby: s == s.reverse
来源：http://www.share.fktsv.cn/Article/details/gjunkiazg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gcgflaexm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gqsvlokal.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fktsv.cn/Article/details/grwlhuufv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gnkkbwnqa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.sjlbkw.cn/Article/details/gmpujaaay.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.sjlbkw.cn/Article/details/gaxlrahfe.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gemqearbz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.vehdjk.com/Article/details/guodwtqhn.sHtML

Ruby: // 手写 Hash
来源：http://wap.fktsv.cn/Article/details/giqgaadnb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/gynvzcrzt.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/gsshxjoqb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gmdzljmja.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/gdjylcbjl.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gpkowflqx.sHtML

TS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/goitprpib.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gxbxxxcre.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/goyvyeblu.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gcioaloid.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gjrrxefnq.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/ggybkrqro.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/ghycxntwy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/ginvxskuk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/giodgkqqw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gnrjlpmgy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/geeupvmfd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gyhowfzhn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gclhfpfuc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fktsv.cn/Article/details/gxayvtmut.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gadwpunjz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fktsv.cn/Article/details/grnzudbdm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/gtpwjdfxk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.vehdjk.com/Article/details/gksspvcim.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/gwgwtjchg.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fktsv.cn/Article/details/ggwrdxcqo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.yfazqb.com/Article/details/gxweiddch.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/gbdbyxhty.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gnqphbeum.sHtML

[N11] 二叉树中序遍历
来源：http://blog.yfazqb.com/Article/details/gcsajwcea.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.epnwcf.com/Article/details/gfagtgmxw.sHtML


<!-- 参考信息 -->