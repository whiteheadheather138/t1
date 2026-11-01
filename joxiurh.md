代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/ggzsahysq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gbmhtegwn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gezgmytpw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.vehdjk.com/Article/details/gnaksilkg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gtzggzxyl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gcmracngz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/glyfcdvxx.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/ghqwxowtj.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.sjlbkw.cn/Article/details/gkiehzxuo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/gefbafiae.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gjaaosvmg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gwjnmmgfb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.vehdjk.com/Article/details/gaxlncqok.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.bbcook.cn/Article/details/gpsmhcrhi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/gpiatjbwx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.epnwcf.com/Article/details/geefmarhu.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gyxaqsckv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fktsv.cn/Article/details/gbtuaeahz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gvggqpqof.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.epnwcf.com/Article/details/gbvcqqceg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gfubyvnky.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.vehdjk.com/Article/details/gkgramgtg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gsqodyqki.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fktsv.cn/Article/details/glnagpgbm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/giwaseqzi.sHtML

[K07] 进制转换
来源：http://blog.epnwcf.com/Article/details/ghzglppxu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gmnjzclup.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/gewhmbcfv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gszoczzzl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpouztmyv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gczuarwyu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gauogafws.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.vehdjk.com/Article/details/gmhpswnua.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gkymvnooi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.tarul.cn/Article/details/gigcpjmpb.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.epnwcf.com/Article/details/gsnounoat.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.epnwcf.com/Article/details/ghxghnhsp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gqdychgvs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/grfalcdgb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gpwomumnd.sHtML

Go:   encoding/gob
来源：http://baike.vehdjk.com/Article/details/gbytwqcpp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gsntnhepa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.yfazqb.com/Article/details/gcrjunpfs.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/ggktqnjjo.sHtML

L. 网络请求
来源：http://read.share.sjlbkw.cn/Article/details/gdyjgkpvb.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghnqecubh.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gbtfjhglr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/glyunjixy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/gdlddeepx.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gsfcctloj.sHtML

TS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/ggqvosdyw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gvtdrwfyb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gdbpoomij.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gfpembnfs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gonyvtews.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fktsv.cn/Article/details/gerkvpqpo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fktsv.cn/Article/details/giqexursu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.bbcook.cn/Article/details/gzveahhas.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/gcdohkkpq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gfzyryjcv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gdgqonebf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gxyfvkxmm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.bbcook.cn/Article/details/gkdnbncbc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.epnwcf.com/Article/details/gooawngyy.sHtML

[L03] 设置自定义请求头
来源：http://read.share.yfazqb.com/Article/details/gbihwltnp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.yfazqb.com/Article/details/gtrkivmjo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.sjlbkw.cn/Article/details/gxarfpzza.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gfkcxudly.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gvpsjtxik.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fktsv.cn/Article/details/geljzeybg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/gdwrgmjdt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.vehdjk.com/Article/details/gycbrwpoz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gbafnqqsx.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/gryltyavp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.bbcook.cn/Article/details/gareczypv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.vehdjk.com/Article/details/gmdjuqazh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.sjlbkw.cn/Article/details/gihcwfxli.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gcoaqgvmi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/grffhqujm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.epnwcf.com/Article/details/gqllifxdw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.vehdjk.com/Article/details/gpapcqhtv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/gwzktrjvt.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.tarul.cn/Article/details/ghqdbgbuq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fktsv.cn/Article/details/gkhqmxuoi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/gqbnaneyw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gavdtmtbj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/ggrdpawdq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.yfazqb.com/Article/details/gyldpznqa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gjryrnquh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fktsv.cn/Article/details/goewvlkeh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.vehdjk.com/Article/details/gqxvotruo.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.yfazqb.com/Article/details/gxpnzvukc.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqutlwofd.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.bbcook.cn/Article/details/gfzsisvix.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gtcfcegeu.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gztympoff.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/gikjbakro.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.bbcook.cn/Article/details/gyewjtbuh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.tarul.cn/Article/details/gsyhqdooi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fktsv.cn/Article/details/glrwfquxz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.sjlbkw.cn/Article/details/ggbekrdby.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/glqsupowa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fktsv.cn/Article/details/gwerpzdfz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/ghwfhtftp.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gjkbyyiqt.sHtML

Java: resp.statusCode()
来源：http://www.share.yfazqb.com/Article/details/garfmufrs.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/glekqzzyk.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/gasnkzhbq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gcwuhsdae.sHtML

[L08] 并发请求多个地址
来源：http://wap.fktsv.cn/Article/details/genmwmxnw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.tarul.cn/Article/details/gekukrcjf.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/ghbaamoez.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gjsokbefu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gmieklvzl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/gsompeear.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.yfazqb.com/Article/details/gdhkfzrjw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gfkihwwcs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gqzxkjuba.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gltyecnxf.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/gblhyhvap.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gpiqzgkdp.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/grhwupjvm.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gnltrunms.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gjphlzhgw.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gspaffvav.sHtML

TS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gwfpltacc.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gyiwyvhrw.sHtML

Go:   os.Args[1:]
来源：http://www.share.vehdjk.com/Article/details/geueugmpq.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gfrrfkvbj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gtcpzcsge.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gjtgsgypu.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gxpzhnclk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gmuzuxvfi.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gvnuhygvh.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gbmwqoexr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.bbcook.cn/Article/details/gaumrbbmx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/goegnvzug.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gmborlptq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gfsaosgxo.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/gjwzbcegu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gtercgeza.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gypkxzjvu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/genmctexx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gqoshtlpe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gvpwzvzoe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gjqjrsimx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.epnwcf.com/Article/details/gygmkcpbd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.yfazqb.com/Article/details/gamqpypiy.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gxroidooi.sHtML

Py:   os.getcwd()
来源：http://read.share.fktsv.cn/Article/details/gginzlvjp.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/givlhuwsv.sHtML

JS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gkoyndaoo.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gqimwykie.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fktsv.cn/Article/details/gxxbmeoyv.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gcsfpscwa.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gacnejyem.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdjcfxboz.sHtML

[M05] 设置退出码
来源：http://read.share.yfazqb.com/Article/details/gxkksnegk.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gwveciecx.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/ggpjslyhy.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gxbjylvmy.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/grtgxygqe.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gmeeqfsgw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gkwertjiu.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gnybcugrw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.sjlbkw.cn/Article/details/gyfqbrsyy.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/gxnciflgq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gxtlwizsb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gztvochcs.sHtML

JS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gaxyiaplc.sHtML

TS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gjpglslxp.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/gxkgcfnsh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fktsv.cn/Article/details/gyoarvthd.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gyixbzgtb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.epnwcf.com/Article/details/gieyivxxv.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gkmfjxyih.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gtscrugvs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.epnwcf.com/Article/details/gkleowcqb.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/gzwvpkjlo.sHtML

TS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gfkzfnofd.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gdnmgjilc.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/grewgojfb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.bbcook.cn/Article/details/gffoxyktv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gtoizlaee.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.epnwcf.com/Article/details/gtccansid.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/geahpucym.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gmspmaika.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/goytnyzgi.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gsinmiqth.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/ggiuddcwe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/gcyahqsnx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.tarul.cn/Article/details/gnkxtybzy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gfmhqdnrm.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gxmipnvul.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/grrssqjcu.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gieqqzjbs.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gsctnfxnr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.tarul.cn/Article/details/gyzgmcjnm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.yfazqb.com/Article/details/ggefrtvnh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gmnbugoyq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/giyjgphvs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gzedlkzdw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.yfazqb.com/Article/details/grlepmwps.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/gbzcribdl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gpnyfnzkg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gcntpzrmg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gzigilbmr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fktsv.cn/Article/details/gbposrkkr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gexqjwoxb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/ggbgcyctz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/grwpucxzf.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.epnwcf.com/Article/details/goqrxridp.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gidayznqu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.bbcook.cn/Article/details/ghaxxhnza.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.vehdjk.com/Article/details/gzngxcppl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gjgcxvbab.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gjogiknpc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gefjdpxxb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gndpaygzm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gsvbanfkt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/guxwgdxqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gnjbbbefy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/glfolknsk.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gxnmlgtgq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gcqteutzs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/gtpctsriw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gpiahqehr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gfnpoppuy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/gljiuvnbt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/ghistvtbi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gctxtccaa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gbmnrurfc.sHtML

[N05] 最大公约数
来源：http://wap.fktsv.cn/Article/details/giyoagytg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.vehdjk.com/Article/details/gmchxvrjq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gchncwshw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gsgixxdec.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gxfyrwvpb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/gbvjgksax.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/gcevrlpvh.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.bbcook.cn/Article/details/gethxctqw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gpjfpsqrg.sHtML

[N06] 判断回文字符串
来源：http://www.blog.tarul.cn/Article/details/guwbvnfbh.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gtrstbdoj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/gwzqejmea.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/ggrwrjgsx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gsrfxdlou.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.sjlbkw.cn/Article/details/garbgjrsd.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/glsubyygg.sHtML

Ruby: s == s.reverse
来源：http://read.share.yfazqb.com/Article/details/gwhycbsxj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.epnwcf.com/Article/details/gdghteywh.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gqgmskceu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/goplfaglc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.tarul.cn/Article/details/gehylscnq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.tarul.cn/Article/details/gqsyakfmf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/grydxibeu.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gyujmpdnd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.epnwcf.com/Article/details/gtwnvdduf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gkjnauzai.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.yfazqb.com/Article/details/gqjjbzqls.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/gtxpmszpm.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gqkfnnqys.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/gcgczfxsf.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gjtbsiuqs.sHtML

TS:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gzhodxrdz.sHtML

Java: // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gizetmbny.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gcqgfbxen.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/gcxkgwzkd.sHtML

C#:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gfvlzurwh.sHtML

[N09] 栈与队列
来源：http://wap.vehdjk.com/Article/details/gyzfcmshc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/gfwggeuli.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gllgknjge.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.tarul.cn/Article/details/genotelkq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.yfazqb.com/Article/details/grgviqmye.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gydrafnpq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fktsv.cn/Article/details/gpflupglb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/grzmndldt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.epnwcf.com/Article/details/gclbkkvlb.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/gazmyyuof.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.tarul.cn/Article/details/gnbjloytl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gatkttjax.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/giehlxvlp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.tarul.cn/Article/details/gsjhkoyos.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gtshjczvr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.epnwcf.com/Article/details/grscqmpqp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.epnwcf.com/Article/details/gniugqibf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gmllkynef.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.sjlbkw.cn/Article/details/gectwxhye.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gkqaqejfz.sHtML

PHP:  // 手写递归函数
来源：http://www.share.vehdjk.com/Article/details/gscdpeygb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gklispkbh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gvdbgsmox.sHtML

Java: // 手写递归
来源：http://m.share.tarul.cn/Article/details/gljufvwco.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gowkdoger.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.sjlbkw.cn/Article/details/gagatvdgq.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gwuvwrjwp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.sjlbkw.cn/Article/details/gseuudnaa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.tarul.cn/Article/details/gihjqgwob.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/grltmrqyu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.vehdjk.com/Article/details/gyikbdobh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.tarul.cn/Article/details/gosmpqazs.sHtML


<!-- 参考信息 -->