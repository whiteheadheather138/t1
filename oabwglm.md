代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/gptmwckgw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/grwmtvehn.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/ggikagacc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.vehdjk.com/Article/details/gcmaxwiox.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.tarul.cn/Article/details/giqzxisxv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gkbvjwamd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.vehdjk.com/Article/details/gpuidgath.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gytudjjct.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/goffoueyr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gjstpgkcr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/guttoaycm.sHtML

[K05] 深拷贝对象
来源：http://read.share.epnwcf.com/Article/details/gwjjuiegq.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/ggoncummf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/glqhoqzpl.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gmcbdlncj.sHtML

TS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gcviihvoi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.epnwcf.com/Article/details/gifciszkk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.bbcook.cn/Article/details/gixlmplso.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.tarul.cn/Article/details/gbxknruzm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.yfazqb.com/Article/details/gqwbcoxiv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/gxwwophmt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fktsv.cn/Article/details/gasopjmnz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.yfazqb.com/Article/details/gzmzgvfvb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/ggpeojaxc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/gtyluykge.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/gxldemwxp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.yfazqb.com/Article/details/ganezztkt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gjekmyhnf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gjaeaenqo.sHtML

[K07] 进制转换
来源：http://3g.sjlbkw.cn/Article/details/gkcofwyts.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gjompkvjm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.yfazqb.com/Article/details/gypqcydns.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gxojkwuch.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/ghhwhzeeh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gacsadwpf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/gfhdvlkar.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.bbcook.cn/Article/details/gxbmphrjz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gwpstgmqw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.yfazqb.com/Article/details/gibdhmsrv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/glxvcumxk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.vehdjk.com/Article/details/gpfpnltth.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gzkvnhywy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gzuwsyiah.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.yfazqb.com/Article/details/googrxsga.sHtML

Go:   encoding/gob
来源：http://www.share.vehdjk.com/Article/details/gdargtzxm.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.tarul.cn/Article/details/gvjittdiz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.bbcook.cn/Article/details/gshfnikxt.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gyrlbdmcp.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gjsxqhqwz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grzhjslqz.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gqxjnnrgq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.epnwcf.com/Article/details/gqeixhvjp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/gvrbmfuoj.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/galytchdi.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gkkcjdslj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/grvclzznz.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.epnwcf.com/Article/details/geypdjugf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/gyajsdhir.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fktsv.cn/Article/details/gcjlcexgg.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gjdkcspyz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/gkxicuawk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.sjlbkw.cn/Article/details/gvcztjhvt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gwoejtiks.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fktsv.cn/Article/details/gspifchdj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/grwjwrbwl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/gjlysrsvu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.vehdjk.com/Article/details/ggufcbump.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/gmzefhkpu.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/goijvqrmo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/gvrevnfwo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.vehdjk.com/Article/details/gsnevvwzu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.epnwcf.com/Article/details/gkbrlcozm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gevbibede.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.epnwcf.com/Article/details/gjcsyvljq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gewhkbfro.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gylooxkqm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.yfazqb.com/Article/details/gugszdpan.sHtML

[L04] 设置超时
来源：http://www.blog.vehdjk.com/Article/details/gdafqzpoz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/glwhpmgtm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/gslcgkucx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyhsobhk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/glepaejcc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.vehdjk.com/Article/details/gzhmqoacb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/gsbfswymr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/ghlounbpj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/gkzacampn.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fktsv.cn/Article/details/gnnsgtkmo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.epnwcf.com/Article/details/gxurgicbs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/guyibdopl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gktylxyjj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/giuaddqiw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gkuslyjqv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gjcmizpuz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gyzltooen.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gwycetjrw.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gpixhueef.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gumjqggjq.sHtML

PHP:  json_decode($body, true);
来源：http://wap.epnwcf.com/Article/details/gkvdothyk.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gjmhutbvs.sHtML

TS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/gterfyeir.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gukzkffye.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.bbcook.cn/Article/details/gsmdxazka.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.tarul.cn/Article/details/guaxcqtxu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.vehdjk.com/Article/details/grirdkdqe.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/geweazosr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gjqyesaey.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.yfazqb.com/Article/details/gskytssxj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gawwwkbqb.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gnetylizm.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gonfagdjn.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/garmkuscs.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.vehdjk.com/Article/details/gejwowfiv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gwvqifyhq.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gritgyldf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gykjgdbch.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gfgvtbeke.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gynvjmxyv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gbrosmgqf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/gsikrqcsf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gucyyeaaj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.vehdjk.com/Article/details/gryxnxcow.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.bbcook.cn/Article/details/ghlgxmixv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvdrvcejm.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/gitfdnbbc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gmelovjva.sHtML

[M01] 读取命令行参数
来源：http://read.share.epnwcf.com/Article/details/gkfhopugn.sHtML

Py:   sys.argv[1:]
来源：http://wap.tarul.cn/Article/details/gppoeqjje.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.tarul.cn/Article/details/gzgasishd.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gyzwthkuu.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gxewuiegv.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/geznrjtjd.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/ggyyfzfpp.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/ggojsqrxe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gzrzwlnpt.sHtML

[M02] 读取环境变量
来源：http://www.share.vehdjk.com/Article/details/gqpghugxl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fktsv.cn/Article/details/gqkwdpgve.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.epnwcf.com/Article/details/gjqptmlms.sHtML

JS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/ggwyzmyan.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gagnawkew.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/ghaynadip.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gtgumzgfs.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gcqwrwwnr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fktsv.cn/Article/details/gfjcmlbto.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gbizeztwz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gviqvafxf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gmekksfrk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/gumtqdenh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/glvrjtvra.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gaphiabxw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fktsv.cn/Article/details/gtleafsuu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/guxmddyfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/gefjxnxyr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/ggbsazazc.sHtML

Py:   os.getcwd()
来源：http://www.share.sjlbkw.cn/Article/details/ghiawiahm.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gyezgrsgh.sHtML

JS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdyacdni.sHtML

TS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gxfcdhjwv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/genxkysid.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gibbzltlb.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gqbcnfgry.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gvhaedlxm.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/gxitgvnyw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gaempuljz.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gcgbngwpw.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gjvztiibd.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/glmutblei.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gzorzjohf.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gnwoezmrr.sHtML

Ruby: exit 1
来源：http://wap.vehdjk.com/Article/details/gjpkdnqca.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gnhhaksig.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gfknqnyql.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gusoaolav.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gqrjtcesh.sHtML

JS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gyorgmvck.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gnjgqsuya.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/govbtouyk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gbdsncmli.sHtML

Ruby: warn "err"
来源：http://blog.yfazqb.com/Article/details/gyfmwkgkr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/ghxzictnz.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gpsjdhvuo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/ggrduwkht.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fktsv.cn/Article/details/gqmalcgbz.sHtML

JS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gblchiswh.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gacqaunmf.sHtML

Java: public static void main(String[] args)
来源：http://baike.tarul.cn/Article/details/gaopimbiz.sHtML

Go:   func main()
来源：http://www.blog.vehdjk.com/Article/details/ghypgktrw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/gscwlfrpa.sHtML

C#:   static void Main(string[] args)
来源：http://3g.tarul.cn/Article/details/gdvlstzjy.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gajothjfs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fktsv.cn/Article/details/gydihdxgr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.tarul.cn/Article/details/grgzgorck.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gehybzaet.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gtpvmjhzo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gwrvtsutb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.vehdjk.com/Article/details/gwbuvanuy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/ghdbdofuu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.sjlbkw.cn/Article/details/gbpcclmtq.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gwdpabuiz.sHtML

N. 数据结构与算法
来源：http://www.share.sjlbkw.cn/Article/details/gnsajdfko.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gpeodvnpd.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.sjlbkw.cn/Article/details/glhwgkgwe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gpjpvcvju.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/ggrnxyzpd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gpauwpize.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gdurybaht.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gukcxynnp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/girglpdyy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gscrrbvsx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gytvrntsb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/gmjnqfzhk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fktsv.cn/Article/details/gqwvwxxvv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/gzdsdidfh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gvcozqrnr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrahwgen.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/gowohwcom.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gvmlipwze.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gpakmjyfu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gcmvphnby.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.bbcook.cn/Article/details/gwstthtpc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/glpikzqmf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/guzffsbew.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/gzksyibfu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gegxlyqdx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/gyyzmjxuj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gpnplxyaa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/giijtmfbv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gsdtmeoir.sHtML

[N04] 斐波那契数列
来源：http://wap.bbcook.cn/Article/details/gmpfwzzjz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gldxtmcwp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/gsbjyychm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gxxutwzkp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/ggktioclg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gcqlxyhxh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/gdtpueeib.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gdoihiobz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gcxqretfe.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/gmxqqtssb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gstfjduus.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gkpbvkxih.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.yfazqb.com/Article/details/gdysfyarf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/ggyjywzrg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gykaitbhp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gkoqxthvy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gihdzaewm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/gfwjnoceq.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gpvccznzp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gqyrjrhve.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gwwqbhqij.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gxtgjapcy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gnaaleccg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gdzysmgkl.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gwbgrltjn.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gyhhnelgk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/ggcbbvcir.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.fktsv.cn/Article/details/gnynadbmp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gbdajebqz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gbncekghs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gstfpeuze.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fktsv.cn/Article/details/gorgwkhea.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/gyfmmxwec.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/gkecokgqs.sHtML

Ruby: // 手写 Hash
来源：http://m.share.fktsv.cn/Article/details/gevkrwemr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gfdhusoto.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/gtcforpsv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gzugparkg.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/gevqtysng.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gcmkjkrqq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gyhisduel.sHtML

Java: // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gzkduqwbv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/giovcdhfz.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.bbcook.cn/Article/details/gmxetekds.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gbhstsetf.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gnvlwmzwe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/guebkqpwy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gczwcquiz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gfvavnuar.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gegbicofm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gloctkfhe.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/gdmeygjop.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/ginkffmow.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.tarul.cn/Article/details/gqthqvgaw.sHtML

[N10] 链表节点定义
来源：http://m.share.yfazqb.com/Article/details/gjzhnodsq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.yfazqb.com/Article/details/gudhypfni.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gliqbdiho.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.sjlbkw.cn/Article/details/gsnwnqmnd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.bbcook.cn/Article/details/gvxdmljdf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gzatjsfym.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.epnwcf.com/Article/details/gcsukclxz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/gyxhgusic.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/gdmhdjuau.sHtML

[N11] 二叉树中序遍历
来源：http://3g.vehdjk.com/Article/details/gjeejedvd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gkoejgxws.sHtML

PHP:  // 手写递归函数
来源：http://blog.epnwcf.com/Article/details/gkmthslgw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/gbvjdwxto.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gdfqwtdlp.sHtML

Java: // 手写递归
来源：http://baike.yfazqb.com/Article/details/gmbeyyjlh.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gnimaigui.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/ghndxxbos.sHtML

C#:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gutexaupd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.yfazqb.com/Article/details/gxeqtajkf.sHtML


<!-- 参考信息 -->