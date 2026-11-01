代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gjmymivqm.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gyrcwxkpc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gjakccrxy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.bbcook.cn/Article/details/gskwlhllf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpdlwnfos.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/gwgbxusmk.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.bbcook.cn/Article/details/gytfwrknp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.yfazqb.com/Article/details/gwqkyriuh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.bbcook.cn/Article/details/gyteitbzi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gdgdxjxva.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gxrojhfgg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/glldyoafk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gabdtwxmc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.epnwcf.com/Article/details/gwxqseeel.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.tarul.cn/Article/details/gineinufw.sHtML

[K05] 深拷贝对象
来源：http://baike.sjlbkw.cn/Article/details/guvwmgsgh.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gfdktalnv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/gadjnkepb.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/gsyzgkqis.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gtcxfvbtc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.yfazqb.com/Article/details/gvfjufncn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/gphhiepfi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gexejilxy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.epnwcf.com/Article/details/gslgrtzzv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/glcgzgktv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gpnhbtoqs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gqntaxyvh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gsjeromwa.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gbwffwwco.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.yfazqb.com/Article/details/geowwntek.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gyukzhxsa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/gsarltzrh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/goexezgan.sHtML

[K07] 进制转换
来源：http://www.m.share.epnwcf.com/Article/details/gzzxgombd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gazkkgpgf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gbnsnkjhu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gmnvwqevg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gzjonrvyn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gpvoowtad.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.bbcook.cn/Article/details/gjialcbej.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.epnwcf.com/Article/details/grhyxmaao.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gtsuuzfod.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.vehdjk.com/Article/details/gqfokaiti.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/graiiwzre.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/gvptqlrhw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gapyssxcd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gqsxkamlp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gcuooojnp.sHtML

Go:   encoding/gob
来源：http://blog.bbcook.cn/Article/details/gcfaocban.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gzelmuwxk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gkyiqqkrc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gwzzknkse.sHtML

L. 网络请求
来源：http://baike.fktsv.cn/Article/details/gdidvigcu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghvbyhdma.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/glxypmvhl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gtxhvgcts.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/gqepgkuwr.sHtML

JS:   await fetch(url)
来源：http://m.share.yfazqb.com/Article/details/gxpijbzmo.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gkqdmaldo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gejzygqyi.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gtgvpusdt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.tarul.cn/Article/details/gglyxodpf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/groiaffbo.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gngkrnlwv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gfsziwlfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.bbcook.cn/Article/details/gwbkeshkm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.tarul.cn/Article/details/gmsbidmui.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gxgsvemeu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gmtnqrnnz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.epnwcf.com/Article/details/gbimxiwpr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gommblvfw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gukbkolvh.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fktsv.cn/Article/details/gwvkcenrw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/gkqwzvbzd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.sjlbkw.cn/Article/details/gznwljotp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fktsv.cn/Article/details/gueerkhhm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gprgodtpw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.sjlbkw.cn/Article/details/gkjuwcnsz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gdkjbrfvn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.epnwcf.com/Article/details/gcyeolouy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gupwawebt.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gyykhrkrq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/gzeombkda.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/gslpuasdh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/glbkuhnbe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gwjfsqlka.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.tarul.cn/Article/details/gteqidbks.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gmsfyfpcm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fktsv.cn/Article/details/gdryjsnfe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/gavyogumi.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gnuychdfj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/gyvzvauuz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gzabdvxib.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gxhztlnis.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gkldqmlte.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.tarul.cn/Article/details/gvmegelds.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gjpydmyag.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.tarul.cn/Article/details/gutdwbjfd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.sjlbkw.cn/Article/details/glnptxxmi.sHtML

[L06] 解析响应为 JSON
来源：http://3g.tarul.cn/Article/details/ggezyncyl.sHtML

Py:   resp.json()
来源：http://3g.tarul.cn/Article/details/gmsubuqpo.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/gblhigvly.sHtML

JS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gqyehzprv.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gdfeuqtsx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gaehpwdrm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.sjlbkw.cn/Article/details/gzlszwhav.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.epnwcf.com/Article/details/gdmqfczcg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gnkzgwwys.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gumzpadhy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.yfazqb.com/Article/details/glgbysjss.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.epnwcf.com/Article/details/gzppkvesf.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/ghcujpclv.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gmzqqyece.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/goxnzapre.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gwaccwuzi.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gpcylxgow.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.yfazqb.com/Article/details/gejfpmxji.sHtML

[L08] 并发请求多个地址
来源：http://m.share.bbcook.cn/Article/details/gkbqepjmx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gxakmllfl.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gjisagdlv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gpockmxui.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.epnwcf.com/Article/details/gsmyifmpi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gaflxqpvt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/gmolbqqaa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/grgfutghu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gckbaimar.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnvtjqmey.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.bbcook.cn/Article/details/gsfpwhonp.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gehcadyzx.sHtML

[M01] 读取命令行参数
来源：http://www.share.bbcook.cn/Article/details/gqvwsvzzy.sHtML

Py:   sys.argv[1:]
来源：http://3g.fktsv.cn/Article/details/gnvhfyqps.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.vehdjk.com/Article/details/gxlbdxuzp.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gukncdnba.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gtzzhphct.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gptnyqpux.sHtML

Go:   os.Args[1:]
来源：http://www.share.fktsv.cn/Article/details/gdybmfhzn.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gllwrwlsn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/goefajfxk.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/grhkszgas.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/ggxuhhesq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gnqkyswff.sHtML

JS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gqcickqyz.sHtML

TS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gvoquhaij.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/ggyvgqdtu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gfhfyoxbl.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gbtksmraq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gukuslsbm.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gvlgnxyqi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gadkkavot.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/glskndbpe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gulzzzdcn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gvlvtqtyz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.yfazqb.com/Article/details/gnblirqlu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fktsv.cn/Article/details/guvankgba.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gvhxzotii.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.sjlbkw.cn/Article/details/gosslfroz.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/glmcqcohs.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gzcxqxojj.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gxgelhozc.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gzirdibve.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gotksbpks.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/gqusboubf.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gqrwewbfq.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gjedipumq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.vehdjk.com/Article/details/gbaimjckc.sHtML

[M05] 设置退出码
来源：http://m.share.sjlbkw.cn/Article/details/gnsolpvjo.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gipiufvli.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gzuxpwcpt.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gzvbfuygd.sHtML

TS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/glzxdryie.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gvjauwirl.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gtwjlhpzx.sHtML

Ruby: exit 1
来源：http://blog.fktsv.cn/Article/details/gmcrbznyn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gbqigcuoi.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gigbdskwq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gqrzllrwv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.sjlbkw.cn/Article/details/gqeaaztoq.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gldjgxfek.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gbzdkkjpf.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/gjlytesew.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvufhmenw.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gadqcdpbt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gmgcgxvun.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gakskxhuw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.sjlbkw.cn/Article/details/gdvfswnlv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/ghyrouyqv.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gyvwoinlw.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gmjsifbeg.sHtML

Java: public static void main(String[] args)
来源：http://blog.fktsv.cn/Article/details/gutlxazby.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/geltkhaqx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/gpmlgpzbm.sHtML

C#:   static void Main(string[] args)
来源：http://wap.yfazqb.com/Article/details/gwsybayvu.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gdbghdhwt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gnjzfhgos.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/gbmluwwlm.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/grqyjxldr.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gfhnlisqj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gsadwvewn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/gdwjcvdes.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/gvrvuhola.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gwljgezev.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gntqkpjjx.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/gzofwjonw.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gjvudipnf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.tarul.cn/Article/details/gbrpabprs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gujvzxocv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gganivgyn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gscdlispn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gdscdfkbt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gsamapnmr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/ggtomttiv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.epnwcf.com/Article/details/gmyakccnj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.vehdjk.com/Article/details/gualjzukz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gucutleme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gnhunbuyp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/gcozsidsi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gepqgtwnf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gcdwuvsov.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gwlxajpyj.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.fktsv.cn/Article/details/gcnyhutjs.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/gxhjwapmw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gmevcviod.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/ggzyvfkyc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gvmzjasot.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gxsqcolgq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gjjqgbwxh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gkwdacaxx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gyfkkuorv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gkwtmxymp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/gcsqvnhkx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.yfazqb.com/Article/details/ginoilqzt.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/guegdpvce.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gywhppqqv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.fktsv.cn/Article/details/gxliffiys.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/ghkabgvfc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/ghiollyve.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gnvzcrrld.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.bbcook.cn/Article/details/gxmxvvbpz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/glkflryoh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/ghkikagms.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gypjzjjqw.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gkdvhhuyr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gchrqjrfb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gdsfajtnz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gipfnxjjd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.vehdjk.com/Article/details/gojunevkh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.epnwcf.com/Article/details/gzfxdfjac.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gmjfhzoem.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gzkxuirdi.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/gpvdycbay.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gywtgikgd.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/gpmvnbxpw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gphxhqrer.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gppkdfncj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gnvudersr.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gygutzona.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gihlmfukg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gvranoktg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/gxbldltef.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/glgdtbcau.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gikxgyxwl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gcooloeiw.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gyxajtilx.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gpsstgrzy.sHtML

Go:   // 手写 map[int]int
来源：http://wap.sjlbkw.cn/Article/details/glrtvoovt.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gdxnrpclc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gaaqcvpqc.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/gbgtiauyp.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gpoqelqlh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gemhuhzdt.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gnpjtlnvf.sHtML

TS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gbrhvcvlh.sHtML

Java: // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gquxmzvoj.sHtML

Go:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/glrvusnqt.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gnpgkmtvd.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gpsjhyvvq.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gbaptpkwk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fktsv.cn/Article/details/gfrgfpveq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gzgmvefeu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gxyfyntpp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gveisumaw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.vehdjk.com/Article/details/gqmnydolb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gfyntzwol.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gmebzrrms.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/ggmdisrcl.sHtML

[N10] 链表节点定义
来源：http://mobile.tarul.cn/Article/details/gxgaknrsq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.yfazqb.com/Article/details/gnutoeprm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/gcxxiybba.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.sjlbkw.cn/Article/details/gsusvfjzb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gpfweokxf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/ggqybsksc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.epnwcf.com/Article/details/gcilgxumt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.vehdjk.com/Article/details/geswgjzrs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gccxdtxee.sHtML

[N11] 二叉树中序遍历
来源：http://3g.bbcook.cn/Article/details/gqzcgyoto.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gdikqjpde.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fktsv.cn/Article/details/gpypbvphe.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gatqegipd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/goyhmjegt.sHtML

Java: // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gjqrytbdb.sHtML


<!-- 参考信息 -->