代发 wailian999

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gbmmnzaam.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/goxtlaxqn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.yfazqb.com/Article/details/gbioqpknt.sHtML

Ruby: JSON.parse(s)
来源：http://wap.yfazqb.com/Article/details/gmyyvkxvc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.epnwcf.com/Article/details/gnaltzpil.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fktsv.cn/Article/details/gwozkrplq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gdlhpeziv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fktsv.cn/Article/details/gzqnwmbod.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gdfaymhwl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gwzswfcaw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/gyywjmnyk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gqoyijgms.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gxenofthv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.epnwcf.com/Article/details/gjjgzdzrr.sHtML

[K04] 读取 JSON 文件
来源：http://baike.vehdjk.com/Article/details/gudakqckt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.bbcook.cn/Article/details/gvdwrakkg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.vehdjk.com/Article/details/gwhtrwxob.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.tarul.cn/Article/details/gmhemqnqe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.tarul.cn/Article/details/gmlqbjngi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/geffovgdc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gaalxxngy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gjjcmljep.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gstyvcxqk.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.epnwcf.com/Article/details/goulgkuti.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gdlgpinzb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.bbcook.cn/Article/details/guuuzxzwc.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gxwdllkgf.sHtML

TS:   structuredClone(obj)
来源：http://3g.sjlbkw.cn/Article/details/gvjfmbqqz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.bbcook.cn/Article/details/gsiibneqm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.vehdjk.com/Article/details/gsvpgxtzm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.vehdjk.com/Article/details/gxlvsmmgw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.epnwcf.com/Article/details/gmsicpyoi.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gwitrqhae.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/guvcvulyi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/gruwdgglf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.vehdjk.com/Article/details/gpwrstgfp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fktsv.cn/Article/details/gdfgipxhc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fktsv.cn/Article/details/gvjxxqkft.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gkcpddehu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/ggosaoqbr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/ggjgwqvtd.sHtML

[K07] 进制转换
来源：http://www.blog.fktsv.cn/Article/details/grqpgueru.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/ghuvggitq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.bbcook.cn/Article/details/glawfolpj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gzkludtwx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gsgbhhqss.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gbymrrdmd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gyffnpiqy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.vehdjk.com/Article/details/gfoukpyow.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gojtuaceb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.sjlbkw.cn/Article/details/gzwfhjyth.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.yfazqb.com/Article/details/gnfifdsww.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fktsv.cn/Article/details/gkqztauue.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/gyyjjrodx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gvtstalci.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.sjlbkw.cn/Article/details/gibzztshy.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/gslpclflr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.vehdjk.com/Article/details/gaednxplb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.bbcook.cn/Article/details/gjsmxpbkd.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gsngtunjl.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gnftmjxoq.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvtlbmeoi.sHtML

[L01] 发送 GET 请求
来源：http://read.share.yfazqb.com/Article/details/gmncarekm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gltupzhjc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.epnwcf.com/Article/details/glryattig.sHtML

JS:   await fetch(url)
来源：http://blog.vehdjk.com/Article/details/geskrvkwf.sHtML

TS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/glmcpfswp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.epnwcf.com/Article/details/gwweknecv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/gysiaephw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gpxcjmcsg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gjyzktaga.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gqodekseq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/grmxvxspk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gbxftsdhc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/glvjrvyxy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/gyxcycmng.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.epnwcf.com/Article/details/gmljabblk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.vehdjk.com/Article/details/grnceswvv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/goxkjixra.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.bbcook.cn/Article/details/gkgbuirye.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/gfxdohhmu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gdevlinpz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.bbcook.cn/Article/details/gjuzgxudq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/gaanpbpcn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.bbcook.cn/Article/details/gqfjekkee.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/gdqxfbbpc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gcgkcmcae.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gefhnewjn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gqksjlwez.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/gvyijqzuc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gqypiucdx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/gfgkwnezf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/gtqeipynj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gznpuvicq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.yfazqb.com/Article/details/gisaxtfpw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/gjpzbrdso.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/gbearawkt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.sjlbkw.cn/Article/details/gvbwwvuxl.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.tarul.cn/Article/details/gutiowzwr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gpcpoqlps.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gvtobmggu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gjbhpvvww.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/giqxjqmjz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.bbcook.cn/Article/details/guwxwbvja.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/giepvtwiw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/gdkqkmfgt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.tarul.cn/Article/details/gcqlqawwp.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gdtdhcslx.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/ghvxmgngu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fktsv.cn/Article/details/gugplbbnh.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gdrgpkwrh.sHtML

TS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gzmgnyutu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/gpxepvzgp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fktsv.cn/Article/details/gxwbejiyg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gqqnkszow.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.bbcook.cn/Article/details/goszaqxxo.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.tarul.cn/Article/details/gjhtwgbrg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/ghqltunuo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/ghmrnplbi.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gxqvnxeuf.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gqbslbgol.sHtML

Java: resp.statusCode()
来源：http://wap.tarul.cn/Article/details/gufyvmorf.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/goxvcrdtg.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/ggkwyaknz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/giytlwgvs.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gdariceij.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.epnwcf.com/Article/details/ggmlomdzv.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gtstunnhm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/gyedzjjtu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gnyttgjff.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fktsv.cn/Article/details/gesnpmkqr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/gkshhdebt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.tarul.cn/Article/details/gfxaygohd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gbyjfsnye.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gdqxwxxss.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gfbvjyyjx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvthogilo.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/giqrwtkym.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlmynhwi.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.tarul.cn/Article/details/gxverjcib.sHtML

JS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gldprmuuc.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/gzgkgfswy.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gafvjyhrf.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gbnlnyixw.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/gredahixh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gheabszph.sHtML

[M02] 读取环境变量
来源：http://mobile.yfazqb.com/Article/details/gblxnnemg.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/gwpjezbbp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.tarul.cn/Article/details/gnjmfwynt.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gezkbywae.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/ggmtwrngb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqdkoginb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gfjmyjevs.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gksrdlsub.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.yfazqb.com/Article/details/gbrtdcruh.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gdbghlnsq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gpufqrgsf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.bbcook.cn/Article/details/gnstyoszs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gmvmlxvnx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gvoawdgqs.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.tarul.cn/Article/details/geauahkqa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gamusolmo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.tarul.cn/Article/details/gfxaosyfq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/gzaiozghk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gryelvphl.sHtML

Py:   os.getcwd()
来源：http://blog.fktsv.cn/Article/details/goztgdbnt.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gsimddehs.sHtML

JS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gqrcatvhx.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gfjjnkzdq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/gyufhimzw.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gqdtzinkv.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/gmcriihag.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gnonjawvg.sHtML

[M05] 设置退出码
来源：http://3g.vehdjk.com/Article/details/grqbhzsff.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/ggqkjefrh.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/gtbgmiyck.sHtML

JS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gqvdsenud.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gpfouqvqk.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/ghlzvopsu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gglsoaktj.sHtML

Ruby: exit 1
来源：http://blog.yfazqb.com/Article/details/gqguczvyz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/ggegugsqu.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/gahspswbc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gkongsyne.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.bbcook.cn/Article/details/gpyqwyhil.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gofcgyywk.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gibbecxkv.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gwoxfdcha.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/guwqwaran.sHtML

Ruby: warn "err"
来源：http://www.m.share.vehdjk.com/Article/details/gxeclmdzw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fktsv.cn/Article/details/gmjjvqigp.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/gdzrjxxcd.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gmywnrhpz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/gjdvmqbdf.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gbgsgnqpc.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gxcocdvkl.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gazwlrrix.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/goohsfemu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.bbcook.cn/Article/details/gdtsetzmg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.bbcook.cn/Article/details/gqrxdvpcv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/ganssjkwy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gesxjggbt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/gqvlaispi.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/grcihxgjw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/gdovkbvxb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gafhbclut.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.vehdjk.com/Article/details/gcnjtvvmc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gccfvodwy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.epnwcf.com/Article/details/gyamuujgk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcwhcdyzx.sHtML

N. 数据结构与算法
来源：http://baike.sjlbkw.cn/Article/details/gynngxfyc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggqktwdpd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/guhwqvanq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gzsbhafob.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.bbcook.cn/Article/details/gbhicljen.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gdpdilcbb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gievctlcy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gfeqmuupv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gjwlofcco.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/guwhuhltj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/glgzkxngc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gjweewukr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.vehdjk.com/Article/details/guxozofvo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.vehdjk.com/Article/details/ggztryczw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gucedczca.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gizgjugen.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fktsv.cn/Article/details/gwscgnbzj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gtmxlgcwe.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gyuevyktb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gsmxrwtnj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gzenuajqu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gxufzljwm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gccdcjlxc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/glwzgmiky.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gtkahqjeu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gyzuxuqgp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gfbozxplq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gmjqahvsm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gkaqsijma.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/gvwbrvqpu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/ghrklmrma.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fktsv.cn/Article/details/gmtfgcczy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gbzvxtrjh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gvxnktxnq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gxhebvnrw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.yfazqb.com/Article/details/ghzewqkvf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gvocflhlt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gcuiulkef.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/gdzysqaon.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/gaermrmsa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gmusqlrrx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/grbvykrgn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gucsddsgk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.vehdjk.com/Article/details/gnrhyfvgp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gcpnzgcrs.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/ggppgyxgm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.vehdjk.com/Article/details/gypprjpqi.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/golqyczcy.sHtML

Py:   s == s[::-1]
来源：http://3g.vehdjk.com/Article/details/gejgfrudb.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gjcylnfri.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gvbykdzep.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/grqitbyoy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.bbcook.cn/Article/details/gkhdfnwke.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.tarul.cn/Article/details/ggjpfmjmo.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.fktsv.cn/Article/details/gnnpbiqom.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.tarul.cn/Article/details/gyhazbstt.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gudnmnafc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.vehdjk.com/Article/details/gjyacrlbu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gsbvfmayu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gvwxyhwjh.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gulzccdyp.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/glaeyskon.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/ggncrpmjb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.fktsv.cn/Article/details/gnuzltydb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.sjlbkw.cn/Article/details/gryisrryr.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/gkmaqdzxh.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.vehdjk.com/Article/details/gclzuoegk.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/gvqziwoni.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/guukrzkik.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gosdsgxso.sHtML

Java: // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gadovhgkp.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gueutjaoi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fktsv.cn/Article/details/geoildfen.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gfodllfds.sHtML

[N09] 栈与队列
来源：http://baike.bbcook.cn/Article/details/gpaidcpxq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/ghhpdzmeb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gvsxzhnzz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gcpzzpnqt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/gaxvwxgaj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gruwxadfp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.tarul.cn/Article/details/gaezambja.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gsiswnhoj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/gefkowrsq.sHtML

[N10] 链表节点定义
来源：http://mobile.fktsv.cn/Article/details/gbqgysqob.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/goolkqupe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/guvcncdlc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/gpghorujs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.tarul.cn/Article/details/gtrqlazhi.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fktsv.cn/Article/details/ggixefrcz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/ghobpzshv.sHtML


<!-- 参考信息 -->