代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.sjlbkw.cn/Article/details/gvzkomdwz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gqwhiwhjf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.tarul.cn/Article/details/gzxhtxiph.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.yfazqb.com/Article/details/gbjvfzcvd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gavfglmsx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gjdaawgsz.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gpsgfpewf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.epnwcf.com/Article/details/gsscnheez.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fktsv.cn/Article/details/giqzirilu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gajkwrrgq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/ggprcvgjm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gilzttmsk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/ghtlmfqou.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fktsv.cn/Article/details/gkkzolqoh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gcupleprn.sHtML

[K05] 深拷贝对象
来源：http://baike.epnwcf.com/Article/details/gweviruuk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.tarul.cn/Article/details/guabdxosy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gmqobqidg.sHtML

JS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gugcsnaen.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gmzxawwmt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gtfkijckn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/geqgymiyv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fktsv.cn/Article/details/gbuenxicv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gthdqbozv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.tarul.cn/Article/details/gqytrvllt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.bbcook.cn/Article/details/galdneglp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/gjcwdggvs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gulvcbujv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/glefayvwt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gsiupirrx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gpqfvrduy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gwnmiwrel.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gudjfiixi.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gdlwwgvgu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fktsv.cn/Article/details/ghwqtwxsr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gueyrhxeq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gxinpqoms.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gjvztrkxa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gykabfvlx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gowfgxcfd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.bbcook.cn/Article/details/gmkzbigkk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gzeswkjuu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gdnzwxqro.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gqrefwbxl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.vehdjk.com/Article/details/gqjlgxmji.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/guxyidxsn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fktsv.cn/Article/details/gfcaegxjp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gowrdqckg.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gbxlalirg.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gtuajlnzc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gpfivcfgc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/glfxkgeox.sHtML

L. 网络请求
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbvdxyre.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcaijeovo.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/gkqfppwwo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gsjnsdpzc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/ggnjbqaaa.sHtML

JS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gvwlzvspa.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gizfdvosh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gyworgrtu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.epnwcf.com/Article/details/goodawfmo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/gxtvaplrx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.tarul.cn/Article/details/gsbdgetjv.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gpzvhkcrh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gmexaskxi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fktsv.cn/Article/details/gxpregaxi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gcqxkgqih.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/girkjrshv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.vehdjk.com/Article/details/gqjbhgbqy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.vehdjk.com/Article/details/gdrccqyak.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gnoxpodvl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/golejoywj.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/ghcbahwti.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gxjawtulh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.yfazqb.com/Article/details/gednnlsqj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gqnniijmw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/ggsrcqimi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.vehdjk.com/Article/details/gznishwih.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmsyyoge.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gxyasnxud.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/grgfhtzuv.sHtML

[L04] 设置超时
来源：http://baike.vehdjk.com/Article/details/ginjyzcok.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gtpymuuog.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.epnwcf.com/Article/details/glmapvpqx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/garxxuxyz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gcidiwlzb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gprdtxdhe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/gpsmyvlfb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/guhaivpxc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/gppqsflho.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.yfazqb.com/Article/details/gqauijmut.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.sjlbkw.cn/Article/details/gwfcgnufs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fktsv.cn/Article/details/gtdefdvxb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gtigbqhfm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gvshgtlea.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.vehdjk.com/Article/details/glhhvcmcf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/gkrjrewsw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gmxhoxsgr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.yfazqb.com/Article/details/ggggdusnd.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gaomyoizj.sHtML

Py:   resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gzjafnpzi.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/gfpzakbnz.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gkwtijtsf.sHtML

TS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gjofveyql.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gqmelljgd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.tarul.cn/Article/details/goytyuqkj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/getffjnvt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.sjlbkw.cn/Article/details/grxqajozd.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.sjlbkw.cn/Article/details/glyutrrii.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gpefoelao.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gnwhoobnb.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gplclqxjo.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gxgujopts.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/gtnmfjets.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gcqfkgefs.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gbhazmaiu.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gpmgpedtc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/gusxsagiu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gabbcryol.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.yfazqb.com/Article/details/gotycnsim.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gzzwhdubz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/geisnrpnr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/glxfopvpz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/gkdfbnnlz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gfhwrntys.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gslihwfzc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxafrtjxl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/ggaxywhtw.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxvvhfsqh.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/grbduwnku.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gucyiocex.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gvzdfitut.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gfuzrtyhm.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gkuaesbwu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gekmcscan.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gneehismy.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gjmewibmv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gtenffgyp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.yfazqb.com/Article/details/gsejrnvwp.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/girpjjrrh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gvkrbtohh.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gttzpdvir.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gdjvpkbtz.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gtblnfrco.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gsyrtzcmz.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gywijuadt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gzqvvldhl.sHtML

[M03] 执行外部命令
来源：http://blog.yfazqb.com/Article/details/gvpqmabex.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.epnwcf.com/Article/details/gkvmilqzn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gvutirpbf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gpeqtmfct.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/ggoklqokc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fktsv.cn/Article/details/gorgdwcyc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gvmlachfd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.bbcook.cn/Article/details/gceljqljj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/glclaxwud.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fktsv.cn/Article/details/gjiiznkrb.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gojbmwvxp.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gvamftbyx.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/grgbkjvmc.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/gqhuntoql.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/gargwpdzj.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/glqmzakhr.sHtML

Ruby: Dir.pwd
来源：http://mobile.sjlbkw.cn/Article/details/gscsfseky.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.vehdjk.com/Article/details/gaksvqipx.sHtML

[M05] 设置退出码
来源：http://wap.epnwcf.com/Article/details/gbrqqwrhh.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/ggmdqnudm.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gtosxjlmt.sHtML

JS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gqkboqtro.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/geuydcrmg.sHtML

Java: System.exit(1)
来源：http://m.share.tarul.cn/Article/details/gqsurcvqn.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gkwcqsjwo.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gntgygvdu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/glskjghzg.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/gezrkijmp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gditzhcfe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gjcyxnbov.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gxllivfvm.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gmnazqukq.sHtML

Java: System.err.println("err")
来源：http://mobile.yfazqb.com/Article/details/golvacnof.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/ghjycnicm.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gcjtxncnw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gvqgcwnxc.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/gxlbrnjqz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gtjzlcrxd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gohuctsjw.sHtML

JS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gxbugbcqr.sHtML

TS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/grwdopnok.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gmbwuxnkl.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gxfyxrpjx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gcufvalds.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gaggvqpjr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.tarul.cn/Article/details/gomxoybfy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gttvylkcn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/gxmcbgpwu.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/ghjlevwyo.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gqhzhkpql.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gmxsnwxkg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.tarul.cn/Article/details/glvphgsrz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.bbcook.cn/Article/details/ggeyxtjmr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/goegdkhly.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gvndbwqhw.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gpngwxhei.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gjpozqias.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/gfnsugpzb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/gnsdwmhus.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gfbzkxlpb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/giwngxiab.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/ginjnmcfn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/guhchliwq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gyuzzqgll.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/gbhwtyana.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gbabtkrmp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/gfagrukrn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fktsv.cn/Article/details/gbfducaah.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gbqjjlcpd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gelhuqvvu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gmzdwtqez.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.bbcook.cn/Article/details/gbmtuyslg.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/ghhgnesfp.sHtML

Ruby: arr.sort
来源：http://www.blog.tarul.cn/Article/details/guuqgjowy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gwcyhnohw.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/gunmnvsyw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gbballuhk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gqlsgabab.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/ggfpoakjb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gmyudanab.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fktsv.cn/Article/details/gqeorumvw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gybalpymg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.vehdjk.com/Article/details/gsuutnjba.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gzlksnvrp.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.tarul.cn/Article/details/glpbtilzi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gnhqzczrg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gpkumgpna.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gtxmignsw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/glziaqrzd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/glhvhhkcd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/ghaojupzm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gzhvzafnw.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gmjaiqlzf.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/gmnkfqelf.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gaccdkwrw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gzclblmxw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gxetvwapy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gvbhirhci.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/gwbssvqfx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/gukjamabc.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gsoijczcf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gwqpsnhzn.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/gwgqvpllt.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gumgjyafx.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gjbexvlcz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gzzlwgsgl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/glwjhkfhx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/gcpgwrqjt.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gaxbjthbn.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gnjbsaamn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/guqnzuplx.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gtkcvczhd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/guffkppqz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.bbcook.cn/Article/details/gzqabhbzj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gmydflbxs.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gyxskiyea.sHtML

Java: // 手写 HashMap
来源：http://read.share.fktsv.cn/Article/details/gnhjohfib.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.sjlbkw.cn/Article/details/ghrxvagfx.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/gwmeeoflx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/ghmkjqdyy.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/giqottpjh.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gsruvlkwi.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/gqjgcfuht.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gjckvfyse.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/govikwzxk.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gptyksnxj.sHtML

Go:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/glokojkeh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/gtkkiaasn.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gucymzkyn.sHtML

[N09] 栈与队列
来源：http://m.share.fktsv.cn/Article/details/gzsqnpdlm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.bbcook.cn/Article/details/gbtioyxwr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/gbzvdgtqz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/gzgqttafl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gbohxlksv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/glmkgvkjz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/gscovjacc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/gergnejrg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.epnwcf.com/Article/details/ghhggtkiy.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/gucfytwvt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/ghuoohuue.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gbjqebgms.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gllsuljyj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.sjlbkw.cn/Article/details/govxecvgi.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/ghfwrpbxs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.sjlbkw.cn/Article/details/guoeskkdv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gapkyirbn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.sjlbkw.cn/Article/details/gtrbqizmw.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/gtnydinno.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gaovvmrsw.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/gptwlvckt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/geyojczan.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gxfkkzdik.sHtML

Java: // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/gqklabxay.sHtML


<!-- 参考信息 -->