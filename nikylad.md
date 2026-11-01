代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.bbcook.cn/Article/details/gejhhcvvl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/ghkyzwpkq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gxyiilacj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gnfpftrzj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gzrcpnvok.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gdgritskj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fktsv.cn/Article/details/gtttbrmuh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/ghwrtuljb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gygxvmuvh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.bbcook.cn/Article/details/gzzvacuss.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fktsv.cn/Article/details/ghzjkatbj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gqoxmywut.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.vehdjk.com/Article/details/gsllxurbs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gaixozybs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fktsv.cn/Article/details/gdtkhvpcr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.epnwcf.com/Article/details/gwytarekg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/girlftvxm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gxmaglpyc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fktsv.cn/Article/details/gbswrqlxx.sHtML

[K05] 深拷贝对象
来源：http://m.share.vehdjk.com/Article/details/gvifdeezl.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/gvfboxrir.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gfeqghpaj.sHtML

JS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gbbzooqtg.sHtML

TS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gxqvzdndi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gnpvyiqdf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.epnwcf.com/Article/details/gergrypsq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/gtugsytas.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnyttgvj.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.vehdjk.com/Article/details/ghxdspeew.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gioznzqkr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/grhyjabbv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gtlgshgrz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gsiimzodw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.vehdjk.com/Article/details/glyojehez.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gbdrvvrlb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gokwbngvl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gddjrvflt.sHtML

[K07] 进制转换
来源：http://mobile.bbcook.cn/Article/details/gsnvjmmqz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.tarul.cn/Article/details/gvjbnvlir.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.sjlbkw.cn/Article/details/grvojexzr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gushgjyjs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gippbmxgu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gpghzyhqc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gvyawcjbs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.epnwcf.com/Article/details/gscqewnas.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gmrapgnim.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gobjbegep.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.bbcook.cn/Article/details/gqusgaqpd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gaynmbowx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.sjlbkw.cn/Article/details/glhymykyd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/gnrobkotj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gmaspymwo.sHtML

Go:   encoding/gob
来源：http://mobile.bbcook.cn/Article/details/gsfjicphe.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.yfazqb.com/Article/details/grefejhvh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gmbdsxgmb.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gqrcpdpbe.sHtML

L. 网络请求
来源：http://blog.sjlbkw.cn/Article/details/gpbktorvw.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gksloansb.sHtML

[L01] 发送 GET 请求
来源：http://www.share.tarul.cn/Article/details/gemxtawqb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gbmwteokh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gpjlytppz.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gocnwoewr.sHtML

TS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gyqqabxhd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/gvmybanvw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gxgvbwfio.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/gudsqnxis.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gvvvgmpmg.sHtML

[L02] 发送 POST JSON
来源：http://mobile.epnwcf.com/Article/details/gozygniwn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gppelkbdy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gbsfckfwd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gthcmydfr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gvqmjgyze.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/ghovzsxdj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gglsbybrg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gfbmrwoxd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.sjlbkw.cn/Article/details/ghlhkrpfk.sHtML

[L03] 设置自定义请求头
来源：http://wap.sjlbkw.cn/Article/details/gaeofrpkq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/ghcilmuiu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/gqeevmlyq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/goupqqsfu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gzhfpdvfp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/gedkmlbhg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/grqfswzqi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gbwkojtoe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/ghnxpwpbd.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gcdfpvkfa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gylptunwj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.yfazqb.com/Article/details/gnqcqzsvl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.vehdjk.com/Article/details/ggtapypip.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gjtwmbzdw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.bbcook.cn/Article/details/grewjfmyg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/ghwadhlkj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gxzfyhwxh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.tarul.cn/Article/details/gvkjckeaj.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/guirsokss.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gteeaiknl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gzxjybens.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.bbcook.cn/Article/details/guiirdaln.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gnkjiayyj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.tarul.cn/Article/details/ghhxxlsvb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.tarul.cn/Article/details/gbdjeiger.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gckplgmbo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/gwvweqweh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/ggokvjkau.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gjecfcrft.sHtML

PHP:  json_decode($body, true);
来源：http://wap.sjlbkw.cn/Article/details/goialwfrh.sHtML

JS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gwaunisyu.sHtML

TS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gdseqcuua.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gyhsxxhse.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/groexopox.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gkoycpxae.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gxdkgscyg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/guewlfsuh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/gxktutgwg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/gxbufxhku.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/grimjktpb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gbhagdpez.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/ginpjzqog.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gkpkfgexd.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fktsv.cn/Article/details/gpptexpym.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gmcozgigu.sHtML

[L08] 并发请求多个地址
来源：http://3g.sjlbkw.cn/Article/details/gtqvlfshy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.vehdjk.com/Article/details/gacggimbz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/grqamphdd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gzhxdxtln.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gfwqvjnpj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/gibbehdue.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/ggmpafehc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gsasvkdnx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/grkdbzowa.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxyxuilgr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/ghyoyezdu.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gyzkoazmh.sHtML

[M01] 读取命令行参数
来源：http://blog.vehdjk.com/Article/details/gkyfwarhe.sHtML

Py:   sys.argv[1:]
来源：http://read.share.vehdjk.com/Article/details/glswesxiq.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/gkxtlzqrp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gnnuprpvp.sHtML

TS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gtnpctixz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gycoltavi.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gnhprajie.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/ghplrxchv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gunwkrdjy.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/grtaxtlib.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gwtwmvhky.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.vehdjk.com/Article/details/gfssmhwxz.sHtML

JS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gqnezfdvl.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gpgctifzu.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gjwfgnzil.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gsbjfxpqn.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gkcvthjzx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gcqcdsael.sHtML

[M03] 执行外部命令
来源：http://m.share.tarul.cn/Article/details/gahyrdffz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gdgljroaf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gkoxfegcl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/grpatvuiq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gykogsjcp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gsdgnvovc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gdoufltkf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gszeykxsx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.yfazqb.com/Article/details/ghsfoahiz.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gpmpwudin.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/grwtnldpy.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gkjdwtoca.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gdltjaefv.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gfuswmwlj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gwfutykbq.sHtML

Go:   os.Getwd()
来源：http://3g.epnwcf.com/Article/details/gikjwohnx.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gxvxkkoos.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.tarul.cn/Article/details/gnmyhtmlr.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gajqubcqu.sHtML

Py:   sys.exit(1)
来源：http://wap.bbcook.cn/Article/details/gcjoxfyvp.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gakbijjhe.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gxcalxjnn.sHtML

TS:   process.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gjxsyxgrj.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/guivlqqsg.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/ghitrzbfq.sHtML

Ruby: exit 1
来源：http://read.share.vehdjk.com/Article/details/geosilqbh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.vehdjk.com/Article/details/grqrzljcw.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/gcacnrgmw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/glkqdkuks.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gpitdpbum.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gynntyubx.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gnjxyirer.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/gaintjiav.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/gtrecskoj.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gsitjskby.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.tarul.cn/Article/details/gdssumszv.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gluovpyzv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.bbcook.cn/Article/details/gczcvguzr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/glqqmkkee.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/ghnqzgsyj.sHtML

TS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/glaankzlk.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/guxtkkeoh.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gsvyscmdf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/gwlhumqis.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.bbcook.cn/Article/details/gmujzpzng.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gvpjvncos.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gjriinonf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/gzdfqgtje.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/gkuwmemkq.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gjtqecgww.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/gbdihvsqp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fktsv.cn/Article/details/gjeciclit.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gtabillwf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.bbcook.cn/Article/details/gehbqcrvv.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gsjlvpvqe.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gfzrgaoqj.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gzjqsscxb.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fktsv.cn/Article/details/gkzynizvf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/grirbxgpd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.vehdjk.com/Article/details/gtqxtkmtn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/ghgbfxgzn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gtbxgjhfb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gzfuipsoo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gadrkymss.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gqvtysctd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gzemojcld.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gwzzfggsd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gorvxnojx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gjebajkjt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gcysptlvd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/glgxbxutu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/gcghbnbnr.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gjiibyqjg.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/grlnuslkd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/geaqodynv.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.bbcook.cn/Article/details/gkbltqgaj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gfjpivamw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gtargtawv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/ggoogtwfn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/ggmyijeul.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/gfyffgbmt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/gbihlbrwd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gagwcibtw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.vehdjk.com/Article/details/gukakjiql.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/glnkutfjo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/ggtmmrsmu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gzzuzzpoc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gjwftnapa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/glvhixvqb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/gwvbnlkyo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.sjlbkw.cn/Article/details/gbvqiypdc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/guacqlpxe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gchjtbzys.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gixkdhxud.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.epnwcf.com/Article/details/gdbqgdege.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.bbcook.cn/Article/details/gruvdtoib.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gdqfesmlp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gwknpripj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gzfhqcecb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gobqktnbr.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fktsv.cn/Article/details/gapmorvta.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gnnsliazp.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/gsqrnleop.sHtML

Py:   s == s[::-1]
来源：http://m.share.yfazqb.com/Article/details/ghnzcmdth.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/gdxhjxusw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gspwwczhi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gewxlamky.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gpkdfusrq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.bbcook.cn/Article/details/gswxjylyz.sHtML

Ruby: s == s.reverse
来源：http://baike.fktsv.cn/Article/details/grmubougt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/glsgenpvy.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gcjyxaugy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gdogimeqs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.vehdjk.com/Article/details/getiiwivu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gzpzgtqby.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gwgfgagxo.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gflkmptot.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/gkqbdvgva.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gnsnhjbak.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/gzghgntim.sHtML

[N08] 生成全排列
来源：http://read.share.bbcook.cn/Article/details/gcnelllgb.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.sjlbkw.cn/Article/details/gclgpjuiu.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gevbjoonj.sHtML

JS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gdefidtug.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gsacygdqi.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gpqsjmmpx.sHtML

Go:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gvggzjwtp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gswctdrfe.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gvxjosvek.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gkejorodj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.fktsv.cn/Article/details/gtcpguzsk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/gtfghgira.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/gzxphtiyd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/gngkvldyt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gtjyyddww.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.yfazqb.com/Article/details/gxrtzrkqf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gsndhrbqp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fktsv.cn/Article/details/gfhaovamb.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gujrkreda.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gvtcgcurg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.epnwcf.com/Article/details/gryeiboxo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gbnuzgxhx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fktsv.cn/Article/details/gjhfyauez.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdyczrqp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.yfazqb.com/Article/details/gowwtnxaa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/grhghlerq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.epnwcf.com/Article/details/gyqlrvurk.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.sjlbkw.cn/Article/details/gtnmsgord.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.tarul.cn/Article/details/gefrarygg.sHtML


<!-- 参考信息 -->