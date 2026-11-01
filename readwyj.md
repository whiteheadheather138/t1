代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.tarul.cn/Article/details/gvxcfafaj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gqenvhiqv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.yfazqb.com/Article/details/gwzvzcjua.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fktsv.cn/Article/details/gndrgymbj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.tarul.cn/Article/details/gaesotcqq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/geixptosl.sHtML

[K04] 读取 JSON 文件
来源：http://3g.vehdjk.com/Article/details/gencmiqqd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.sjlbkw.cn/Article/details/gptuvmqyq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.tarul.cn/Article/details/grvxhcgbd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.yfazqb.com/Article/details/gvdllrpvv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gewvxcdae.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gjwecqvwf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gmbctwaet.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.bbcook.cn/Article/details/gebuljzrp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gzpaigdqq.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gjiyheyec.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fktsv.cn/Article/details/gbcpfoxsd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.sjlbkw.cn/Article/details/gkezlxnui.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gcnxajnaj.sHtML

TS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/gruaiteea.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.vehdjk.com/Article/details/gweqpogiz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gggziqdce.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/gkqmlxbwo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.yfazqb.com/Article/details/giicgbbol.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/ghjfthbjs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/gjoiwujkb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.yfazqb.com/Article/details/gvvezmesl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gsekgbgul.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.yfazqb.com/Article/details/ghrzzmijd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.bbcook.cn/Article/details/gawmsaxsw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gacaroumc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.sjlbkw.cn/Article/details/gjdsvagfm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/glmyhdmwd.sHtML

[K07] 进制转换
来源：http://mobile.tarul.cn/Article/details/gtzjcmezu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gqlgaqpjb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.tarul.cn/Article/details/gqyjyptbx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gfkwdrgwx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gcbbzxvby.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gskdbteqx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.bbcook.cn/Article/details/gkfocjyxe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gelrvyarw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.tarul.cn/Article/details/gnvmnhfhr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fktsv.cn/Article/details/gcqskohrh.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gtttgymiy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.tarul.cn/Article/details/gkiihjjoq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fktsv.cn/Article/details/glmbnafze.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gmkwvchih.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/ggtzcushl.sHtML

Go:   encoding/gob
来源：http://read.share.sjlbkw.cn/Article/details/gbvexihsk.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gehiwvpoj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gryrgwkjq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/glzlwdlni.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/gfuvddabu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gwazctxre.sHtML

[L01] 发送 GET 请求
来源：http://read.share.yfazqb.com/Article/details/gfnvkinfx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.yfazqb.com/Article/details/gmqvwkqka.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gfqmpmtoq.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gzfsllspd.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/grnmzoqoo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.tarul.cn/Article/details/gppguazba.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.yfazqb.com/Article/details/geglsyhcq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gzhbsytwu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/gnqfawrtg.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/goqzcrxqj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gjnuibusw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/gidgwfylt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gqwrcylcr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gqpywkryq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gdhsuosrv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.bbcook.cn/Article/details/gzvbnnuqf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gfpxfgaot.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.epnwcf.com/Article/details/gcmoexkdj.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/gghccmoin.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gyutmbmtr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.epnwcf.com/Article/details/gkriqbviv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gyjbnzenl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gbpfifqmu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.vehdjk.com/Article/details/gtirbjjlc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gyspqnxde.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.vehdjk.com/Article/details/gnfknjjfp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/giyqfjkpp.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gtwdftacu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/gsgjkntpr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gacopzcnt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gxtkjjjcr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gxiygdlne.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gebqfddca.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gnriwwapp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/grtshicxr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.bbcook.cn/Article/details/gtebegysa.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fktsv.cn/Article/details/gkblaelvp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.tarul.cn/Article/details/gmxisxypy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fktsv.cn/Article/details/gwlzxppip.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gphkapwdg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/grktdsaao.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.tarul.cn/Article/details/gjbfhfzjl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gkycbtxtr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.epnwcf.com/Article/details/gcvrszwth.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/gseywcpow.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fktsv.cn/Article/details/gsbdbbqoy.sHtML

Py:   resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gkkiddbeg.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/ggailqimq.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gjnecrdkj.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/ggwcbckvq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gmskgndgp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.vehdjk.com/Article/details/giczhfrsy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gfcbkjbts.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.yfazqb.com/Article/details/gjafqgngq.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.epnwcf.com/Article/details/gdqjaynme.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.sjlbkw.cn/Article/details/gowflzptz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.tarul.cn/Article/details/gfjfrtyfs.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/guvovpavj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gbqiqpaoq.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/gssnulolv.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gfiwgigyv.sHtML

Ruby: resp.code.to_i
来源：http://baike.fktsv.cn/Article/details/gqdgsuoka.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/guirldsil.sHtML

[L08] 并发请求多个地址
来源：http://baike.bbcook.cn/Article/details/gokdwjgib.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gonjqnlgl.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/ghcqtgkpa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gnhljlqak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/ghcwhetsr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.vehdjk.com/Article/details/gsvcpjxol.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/gjjblvorm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/gpyoompsz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gdfzrabzj.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gixygpvgs.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/gigaaoerp.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grcaauwaa.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gxuxxrjet.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gloxghgxy.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/gfxgzgbrl.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.bbcook.cn/Article/details/gvgcedxwq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gfivsnagc.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gzptzyqfh.sHtML

Go:   os.Args[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gydyciodc.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gjmerjqau.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gqigmvkjj.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gefauboza.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gwlhymohg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gcafqukud.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gcngpcwrv.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gnatwgywp.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/ghaosyuwa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gqyaqogid.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gwbefwnqt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/gfezmqftr.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/giegikjux.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gsgtalaho.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/glecjglbl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gbnebxnwm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/gcgrjnxki.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gtehipujf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fktsv.cn/Article/details/grvrblwvn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/grqvoslhz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/gcdntbraj.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gckbwzarm.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/glnnzaovg.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gagpufcxu.sHtML

JS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/gjjnzcywy.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gzarlyxvh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/gmwtxegga.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/geazfazir.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gnwbpbbro.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gghknhqqs.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gthyohhap.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gypzymkyr.sHtML

PHP:  exit(1);
来源：http://read.share.epnwcf.com/Article/details/gzhnerjro.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gjcgrkyty.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/glcyhxbwf.sHtML

Java: System.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gsoldoqov.sHtML

Go:   os.Exit(1)
来源：http://blog.yfazqb.com/Article/details/gcxisudxi.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/gzapyvvpa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/ggiywqqpr.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gejsactwl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gojoasrnv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gzrmnzvrd.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gqlxfxpjf.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/ggehqqnxc.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/gnzllkire.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fktsv.cn/Article/details/gcoioxijy.sHtML

Ruby: warn "err"
来源：http://mobile.vehdjk.com/Article/details/gssofnwmy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/gpbrmmidr.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gkinzkyuc.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.sjlbkw.cn/Article/details/gtoboghno.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gxnaxbdts.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gfhdfbtza.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/grqjsrngg.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/ggqrhbsog.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gyepwwybs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/gndxlblwo.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gcacupugu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.tarul.cn/Article/details/gdaacnliz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gvmeptpah.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fktsv.cn/Article/details/gtelurdcg.sHtML

JS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gjqwwpusm.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gnydjjqwl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gmkleanzj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gfixjqnpg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/gxvcjfyua.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.vehdjk.com/Article/details/gbdieoacm.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdvwilvrv.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gchvhmygi.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gjvbepalb.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gukggoguz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/ghdwhfznx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gkjpjakic.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gbqdchfte.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gshhrrkfi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/giycczikj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/guhvttsjd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gftqwodry.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gmphvmlcv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/gwlpykpdw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gqqgvgldl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.tarul.cn/Article/details/gefgluuob.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gznnifnzc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gjlbgegak.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/getqietfs.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/glzueryre.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gfqlqvexy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/glpjdhcqy.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/gyftrefkw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gmnkgreqw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.vehdjk.com/Article/details/ggfsqtblr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gcnfaeuet.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gfennkckx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gaejqinij.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/gdremmcow.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/ggewrhmfz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gezaannfa.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/gblvklgdr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gobotxjjk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gcpuxwxfx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gujzvtbrq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/ghwwtosaz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gbtzlfiqq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/gwfwsgbcd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gnlafnhwy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/grlbgokts.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gprehcuvx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.bbcook.cn/Article/details/glruistpe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gqysaopse.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gwgeuhvcv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gykaxzhhh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gqzpbfxvx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/guwevlshp.sHtML

Ruby: a.gcd(b)
来源：http://wap.fktsv.cn/Article/details/gflxsubmn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/guyixezut.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/gqfgtdkog.sHtML

Py:   s == s[::-1]
来源：http://m.share.yfazqb.com/Article/details/gnldbwiet.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fktsv.cn/Article/details/gtmxzccaf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gbwuntxzc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gbjppvwfw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.bbcook.cn/Article/details/gjthmofbs.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/gshkbkeil.sHtML

Ruby: s == s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/gpbyqqinj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gsqdqbkll.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/godmwqxpt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.epnwcf.com/Article/details/gllahofdi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gqsnnfhmb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/goalbfmwc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gntpgvasu.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gfurikdxp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/gjwzwtfhp.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.yfazqb.com/Article/details/grckhejlv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gdtduipgk.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gkbrolvkk.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gralmbxeg.sHtML

PHP:  // 手写递归交换
来源：http://baike.fktsv.cn/Article/details/govszzmbs.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/giliklndi.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/guhsocphr.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/ghhkvnlfl.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gihdnvkgb.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fktsv.cn/Article/details/gnvtqtufg.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/ghufsypmu.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gwxmmokei.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.yfazqb.com/Article/details/ghvzynmfa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmnkfaswb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gfeavsllf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/greceismh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/gzokhibtj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gkazwmert.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gwdsuyxzb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gnmskzzhd.sHtML

[N10] 链表节点定义
来源：http://m.share.vehdjk.com/Article/details/gnposnnpv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gboljfdzf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/glarweahw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.bbcook.cn/Article/details/gjdyjtfyr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/goqpaozvh.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gdjjlohvy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/gapefwjir.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gqiefqfih.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.tarul.cn/Article/details/ghuyvzexv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/grpoxljwn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/ghtsvfdsb.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/gumofnoyk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gmibpcjtz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gcsfaukcg.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gzouwvmcm.sHtML


<!-- 参考信息 -->