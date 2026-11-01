代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnpcmkxhq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fktsv.cn/Article/details/gjlqkysil.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.tarul.cn/Article/details/gnnfuxykn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gopvnqvht.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/gpjztcbcp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.epnwcf.com/Article/details/gzjczqcum.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gocyobwxw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.bbcook.cn/Article/details/gajhcqfni.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/gbfuddema.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gdcuwdysv.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/gecmkrxsv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gjjhjxgdn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.sjlbkw.cn/Article/details/gcmogrqud.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gpgtpopir.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gxnjqltyz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.bbcook.cn/Article/details/gvgegdowg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gyirnfcvn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/glfvkplqw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.tarul.cn/Article/details/gxgjezeme.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/gkayvctdv.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/gvbhpgpdr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fktsv.cn/Article/details/gzxlzxsap.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gutdynhhb.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gonnufqwe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.yfazqb.com/Article/details/gbyhljzsj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gtquwnyoa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gahixqeju.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.yfazqb.com/Article/details/gezhvekne.sHtML

[K06] 解析 URL 查询串
来源：http://baike.epnwcf.com/Article/details/gljyxqsgl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.tarul.cn/Article/details/gmxibzinz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.tarul.cn/Article/details/gaoftqxjf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gwqkpmujv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gemmeoqnk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.tarul.cn/Article/details/gybqqaqtr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/gbhdcqzdx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/grusefsxf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/gjxmeemxn.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gjlqatttq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gkgnfoyvk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.bbcook.cn/Article/details/gleyagwcc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gpdbvxgkw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gnfodwuux.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gqxfiokup.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gqwmrrfdi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.tarul.cn/Article/details/gepxjiuju.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/ghonjtdfi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gdpmymemn.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.yfazqb.com/Article/details/gedlgtxaq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gsspdcfyx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gcdtsmfst.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gchapsbkb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.bbcook.cn/Article/details/gpkzcpaad.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/grkftavux.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/gaovptcxf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.tarul.cn/Article/details/ghnsaizzh.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdgwmrhgp.sHtML

L. 网络请求
来源：http://www.m.share.fktsv.cn/Article/details/gsdsmixnz.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gvekqllzg.sHtML

[L01] 发送 GET 请求
来源：http://3g.vehdjk.com/Article/details/gzmlryuob.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.yfazqb.com/Article/details/gzljeeytl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fktsv.cn/Article/details/gvfzwmoum.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gttlhzjgy.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gypcfehvy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/gulgnkaoy.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gwnofcnmm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/grznekyzz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gadjzjbiv.sHtML

[L02] 发送 POST JSON
来源：http://m.share.tarul.cn/Article/details/gusvtvmlj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gzintczzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.tarul.cn/Article/details/ggmmtncwo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gbweechdk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/giyblkpdp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.yfazqb.com/Article/details/ggvikuunr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gppctksfl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fktsv.cn/Article/details/glyvbvdpo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gxkvggypc.sHtML

[L03] 设置自定义请求头
来源：http://baike.bbcook.cn/Article/details/gdhfiiyaf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gakvrmucr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.epnwcf.com/Article/details/gkjqvehby.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/ggquaroul.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/ggdymkqdo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/goehbunyg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gtgotdcrh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gnwtznqid.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gmpjotwuu.sHtML

[L04] 设置超时
来源：http://www.m.share.epnwcf.com/Article/details/gqdaeabhi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/glydprery.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fktsv.cn/Article/details/gcsqjmtkn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fktsv.cn/Article/details/gnvwttdfi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/ggmbtenfn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gpmaskbht.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.bbcook.cn/Article/details/gwzbnzeti.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gyaitnszt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gwkmcdhfg.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/goerfvqop.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.tarul.cn/Article/details/gxcovttuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gsqsazauo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.sjlbkw.cn/Article/details/gjrpwpjye.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gmzjofvtw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.vehdjk.com/Article/details/gkxhhnzmp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.bbcook.cn/Article/details/gprfzenmi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gsgjqegdk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.bbcook.cn/Article/details/gertrgzcn.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.sjlbkw.cn/Article/details/gymajbhqp.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gfgfbgroj.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gykegaquq.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gjasfcekc.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gcdwczmvk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gcigfhlis.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.bbcook.cn/Article/details/grqiaddhp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fktsv.cn/Article/details/gksmdjuon.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.yfazqb.com/Article/details/gdxwbfnqe.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/gigzwzmdj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/gkfcubsph.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gafbvmhdw.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fktsv.cn/Article/details/gvvcemksw.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gkizhliuz.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/goutisany.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/goltjhxfw.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.bbcook.cn/Article/details/gihdrgjzj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gniupoyog.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gbxayrrei.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gfzgevsmc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gznnwykim.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gvpckhbaf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gthqptgvc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.epnwcf.com/Article/details/gslivoktj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/gjllpnvoq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gpduhnfwo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gpeofjihd.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqmwxfvgt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gnmwwawej.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gkrysyeuq.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gmlmrbfeg.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/ghgluuerv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.yfazqb.com/Article/details/gohyxgscz.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gkteggdvg.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gnrtxrgdc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gwzsfiqya.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gjxjpricx.sHtML

Ruby: ARGV
来源：http://blog.fktsv.cn/Article/details/gjabwtdko.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gqdgyyzcy.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fktsv.cn/Article/details/ghjmfxqvb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.bbcook.cn/Article/details/ggqvimcjb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gmutqfjdq.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gmtozymql.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gdngcbvhs.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gwjlshqej.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gpbupgilt.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gvfzthfri.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/gkvwahhkf.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/glinrqnps.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/grqgvrgpk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.vehdjk.com/Article/details/gehntlrmu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.tarul.cn/Article/details/gklwtkgdu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/guseaqzoy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.vehdjk.com/Article/details/gbpqhalrh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gqthiibdb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/ggeniurix.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gurwamypk.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/gmfxdxeka.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/gkfqgcjpn.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gqnbcbdpm.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gavsmipve.sHtML

TS:   process.cwd()
来源：http://www.m.share.tarul.cn/Article/details/gdzgyinxu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/ggmbcwbch.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gbbayejfj.sHtML

Ruby: Dir.pwd
来源：http://baike.epnwcf.com/Article/details/gonyismsx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/ggdlnjfrn.sHtML

[M05] 设置退出码
来源：http://read.share.yfazqb.com/Article/details/gyzizqdkr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gaonttvkn.sHtML

PHP:  exit(1);
来源：http://read.share.vehdjk.com/Article/details/gewxbaxhh.sHtML

JS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gmfsxeijl.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gsssyuepz.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gxjhwrhpe.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gebpuojhk.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/gyvjmqpch.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.yfazqb.com/Article/details/goqyhhjnp.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gekxgoaeb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gdhzbxcyl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.epnwcf.com/Article/details/gjtggqucb.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gudjbwzoy.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/gjtredtbe.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/gmwlzzvrc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/gdtkxbzck.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/gedszkayg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/gmthtkgzh.sHtML

[M07] 判断是否为主入口
来源：http://blog.sjlbkw.cn/Article/details/gysfejhuq.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gmtcckgca.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.sjlbkw.cn/Article/details/gapriowxv.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gaqnifuyt.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gleflabwo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gpcoofjgs.sHtML

Go:   func main()
来源：http://wap.sjlbkw.cn/Article/details/giffmvize.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.vehdjk.com/Article/details/gtybgsuvv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.tarul.cn/Article/details/gswbbnjrv.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gwhwfbzip.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.bbcook.cn/Article/details/gvpaabzjw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.yfazqb.com/Article/details/gqccpaizf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gzqyecglw.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gmweuqhsk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gughngpbt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.yfazqb.com/Article/details/gyoanswlo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.sjlbkw.cn/Article/details/gcnfnsupe.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.vehdjk.com/Article/details/gdxtznfnm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gtkyufbms.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gareyfxvb.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gokvsvukn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.epnwcf.com/Article/details/gkupiveln.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gszigdnsp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gspyvgsce.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gctfrfjry.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gzrpksian.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gkpuzvdyl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/grfyskkgv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/gdxddcxyf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gepzdsjfm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fktsv.cn/Article/details/gpdhbsciq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gddofwdbh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.yfazqb.com/Article/details/gbugggwsy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gphlgqlki.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gnkmsbcaa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gzglhopqa.sHtML

Go:   slices.Sort(arr)
来源：http://wap.epnwcf.com/Article/details/gdeiyxzru.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/ghijgfafn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gzirrzvuo.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/glipmguri.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gtjykhjhz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.vehdjk.com/Article/details/ghwnpafqo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gawmucodj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gfcavrrfk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/ghztomzff.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gfzjjnusp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.sjlbkw.cn/Article/details/gpctducbb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fktsv.cn/Article/details/glnznefel.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/guahhjiuy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gxuxmyrxa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/govvrcckj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gzgydrlxs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gvqwtqvip.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gevtxokwx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/gzbbualdj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gkayeiqfj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gmgzofvvg.sHtML

[N05] 最大公约数
来源：http://mobile.yfazqb.com/Article/details/gusypmhni.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gdzkbuemw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gzqntjjaj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/guaehfass.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gqzdrbayt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.bbcook.cn/Article/details/geqzxjbfu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/gtloxcgnm.sHtML

Ruby: a.gcd(b)
来源：http://3g.epnwcf.com/Article/details/grhpnukyu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gkuyykrjz.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/gpzshnhyc.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/gueyixuoi.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gznoomiiq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/giiggcpye.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gynmzltva.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/gdlhhwuoj.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.tarul.cn/Article/details/gkelducwi.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/gzsxcbmhi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gsfjcmkmw.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gdymbfaqg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.tarul.cn/Article/details/grvouotiz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gpgavbgmz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/gsdawypdr.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.sjlbkw.cn/Article/details/gwibcgbfg.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/guoublzti.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/gmiplhdlr.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gfemmkxvk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/gwwclxeti.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gpxlnvmhz.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.vehdjk.com/Article/details/gqqdjxfpc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.yfazqb.com/Article/details/gnjxuumqh.sHtML

JS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gkfrmpuxg.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gyssqwlab.sHtML

Java: // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gxrtfammu.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gwpblnxaw.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gfhaspltd.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gyuxjcdes.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/gtwdyxmng.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gwyvziczu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gapunxhzb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/ggzgqeguu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/gptvriozw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.bbcook.cn/Article/details/gdggwosdp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gpbdzsbjx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gbdqzlnxf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/gvjczwcfa.sHtML

[N10] 链表节点定义
来源：http://mobile.epnwcf.com/Article/details/gwuwbabzu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.bbcook.cn/Article/details/gwikakwpr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.sjlbkw.cn/Article/details/gyqfiwsej.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fktsv.cn/Article/details/gwpkwskxt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gxjpekfpr.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.yfazqb.com/Article/details/gafdjfpyf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/gflykiltt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gcgohwklo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.yfazqb.com/Article/details/gzjixnaob.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gjxkpqhtz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.tarul.cn/Article/details/gquiowlqu.sHtML


<!-- 参考信息 -->