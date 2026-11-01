代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gcyqnnskk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gjalbzqhu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/gmrujwgau.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/gioujnzdv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gfkmsyult.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/ghkoqnktm.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gwkdzuyqv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/gudcveuxa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/grldhnoas.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gqwiqevny.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gvkeqszry.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gchdovqtw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/ghlepnbun.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gxutikpqv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gselhbgzv.sHtML

[K05] 深拷贝对象
来源：http://m.share.tarul.cn/Article/details/gunafvukn.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.vehdjk.com/Article/details/gohubpdqp.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gugxhdzlb.sHtML

JS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/ggtslypfo.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gugxlqnhk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.tarul.cn/Article/details/giejzywuv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.vehdjk.com/Article/details/gphcwhhuj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/gbyfxmknp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/glyxftpej.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.tarul.cn/Article/details/gdaacphwi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/guiplbtsn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.bbcook.cn/Article/details/gomldejag.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gnrimrzkx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gnsumcdky.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fktsv.cn/Article/details/ggnuarlwf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/geylfkdnd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/giajaxgks.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/ggplfdejq.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gumpgqgpj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gudkxtmjd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gpqejvxws.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gmbpkqzgv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gvldgshbi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gpgwdngjb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/ghavuozsp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/gyycmkdrq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/guihgqpqu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.yfazqb.com/Article/details/gfepbsnqx.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/ghapkdqyx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.epnwcf.com/Article/details/gijbyvxdt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gvjixvdhb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gokkvplan.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gzgcilofr.sHtML

Go:   encoding/gob
来源：http://www.blog.fktsv.cn/Article/details/goagpolgb.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.bbcook.cn/Article/details/ghyqtiuyv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.epnwcf.com/Article/details/gwwaeyoje.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gticqptkp.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gxfjuvjba.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gsmjtiwcw.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gyzwpuoeg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.vehdjk.com/Article/details/gubwdzgpg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/geazcfocv.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/goxrhgqsl.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gowvhbgnm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gdceevxqt.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/gbtrwhirk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/gquxqoxul.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/gfoyzwcap.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/guvcftsai.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.tarul.cn/Article/details/ghfknlyth.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.bbcook.cn/Article/details/gfwdvyvkg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gixpkaiwx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gesqjfmuz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.bbcook.cn/Article/details/gdukmkntv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gqufutsjh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gfwwzgnsq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/gnjewrgbr.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/gudgcxjdu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.bbcook.cn/Article/details/gauxoviuw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.yfazqb.com/Article/details/gaxvjsuqr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gzkhxnslj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gfyylrumi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/grdivobpd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gvdnkshwl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.yfazqb.com/Article/details/gmbuxlxnh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.epnwcf.com/Article/details/goizgewkx.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/gjwauisvg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/geraqwmgt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.sjlbkw.cn/Article/details/gjlkefiyw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/ghhntsqed.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.vehdjk.com/Article/details/gjjeyjehr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/gmujaohvd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.vehdjk.com/Article/details/gepysdvhy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/grvpyojyt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gyazwcugq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gttfgpley.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.vehdjk.com/Article/details/ghugkrfln.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.epnwcf.com/Article/details/gwufpvigx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/glklpmfte.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.bbcook.cn/Article/details/gsfgathko.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/gtjotulmp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fktsv.cn/Article/details/gabkqzgxw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/gnddfgncm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/gusildogk.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/ghzsnpbkb.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gxplslihv.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/gbsxmeskx.sHtML

JS:   await resp.json()
来源：http://www.m.share.epnwcf.com/Article/details/gurctqqwc.sHtML

TS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/grbjatkpe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/glnwzpqop.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/godjhqjwf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/geamugcdh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gggcpobeh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gkgjoxsxd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gynmonnoi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fktsv.cn/Article/details/gvjzszbff.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gzdbijhvx.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gjnnxcvlr.sHtML

Java: resp.statusCode()
来源：http://m.share.bbcook.cn/Article/details/gstejwvgd.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gpvmahbah.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.vehdjk.com/Article/details/geugfcbht.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gtrautxdc.sHtML

[L08] 并发请求多个地址
来源：http://blog.epnwcf.com/Article/details/gugkuqthl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fktsv.cn/Article/details/gbdnxgoiv.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gsajoilql.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gcohvhtqf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.vehdjk.com/Article/details/gjklwsxqf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/gvxcqbkvw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.bbcook.cn/Article/details/ghwydtubh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/gluyodpmb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.tarul.cn/Article/details/ghzauzbjg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gwkvglpuz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/gpxuzulgq.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gqiymdfcw.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/guavwwwpw.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/glbizmucz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/ghnaktwxo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gdlwgsmpo.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gldfkxoki.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gslyeakri.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gyyuvksns.sHtML

Ruby: ARGV
来源：http://www.share.yfazqb.com/Article/details/gpvljhtxl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/ghcogdpxo.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gxotulbet.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gtqxzsryu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gcltmayqi.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gurfvthbu.sHtML

TS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gbjlucffe.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gubmnlvcc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/grwxannth.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gfulcihut.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/gvqmcxesj.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gutqlqacg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/gzxfwmznz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fktsv.cn/Article/details/glihaibke.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gmomaforv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gqjxoilrp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gklerdutl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.yfazqb.com/Article/details/gjnihydlc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.bbcook.cn/Article/details/gviiehuvc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/gjwzcdekm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gbwnxtdlt.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gjmcnhscl.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/ggzaqfohv.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gdchsznch.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/galanxrqf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.epnwcf.com/Article/details/gfxoolhjx.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gdhorjkep.sHtML

Ruby: Dir.pwd
来源：http://baike.bbcook.cn/Article/details/gtwsbxmlk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gqlysulqz.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/govmqwogi.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gerwtuish.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/genjnvbxe.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gikszenmz.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gbjeoiava.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/gjosslxko.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gnwqckjxn.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gttgiwirm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/ghkhyjogu.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.sjlbkw.cn/Article/details/gdmipuydw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gyshapvfw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.tarul.cn/Article/details/gtvbmkprx.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/ggfrbynfx.sHtML

TS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gxpstmbnd.sHtML

Java: System.err.println("err")
来源：http://3g.bbcook.cn/Article/details/gtpoubdgy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gxlxdpehc.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gxsmwtinh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/gzpwhwjkh.sHtML

[M07] 判断是否为主入口
来源：http://mobile.sjlbkw.cn/Article/details/gjvxuuuki.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/gcizovrhe.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/gmfjtiesz.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gdkakmawm.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gkwjitghd.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gubejexku.sHtML

Go:   func main()
来源：http://3g.epnwcf.com/Article/details/gjtgzfvjn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.epnwcf.com/Article/details/gfijksfnf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gtdvkvpko.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.epnwcf.com/Article/details/gxwdurghq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fktsv.cn/Article/details/gntfkaxyc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gkrjrmmkd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/grkerphml.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gdnzcjaxa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/gqlaglxww.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gbuahrxly.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.sjlbkw.cn/Article/details/gstfclcht.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gwdgqqpdp.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gdhzkrscl.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gexhcuwwv.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gaeamuuzd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gjmhhgxuc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gofwwwkhh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gnuldrsfk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gqbbpytqk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.yfazqb.com/Article/details/grfslejti.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gxttaifpi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gqqnmtrub.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/gkyvrowhu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gumuxxyik.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gmlvrjcea.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/garicrlpq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gnehqtokv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gjujiuqtr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gcarmwing.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gocobmznz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/gkdfqvquf.sHtML

Ruby: arr.sort
来源：http://mobile.fktsv.cn/Article/details/gtltmevkm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/gfugiqnja.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.sjlbkw.cn/Article/details/gsjwpzbsm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/gkhsxrcua.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/gpphdvxvd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gdeoqjqdd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gpavgaijg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gwnkyxpgy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.tarul.cn/Article/details/gdxzygfzt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/gvheuhdbk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gbcbfxhlj.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/gunhmtmuz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gytqoddfy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/grrpyfizo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gffisibqy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gpadcgcpl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/gjjxycuqw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.sjlbkw.cn/Article/details/geduuyltq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gudncmnye.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/garrsgfzr.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/gttikthfb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gnodokpby.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gwjhgwusm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gzvyvjjew.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gygnwdiql.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.bbcook.cn/Article/details/gfigtazhg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpzdcvsr.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gprtlxmhk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gsrjaptir.sHtML

[N06] 判断回文字符串
来源：http://wap.epnwcf.com/Article/details/grweyhlcb.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gbpaqwwmv.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/glfghxhin.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gijbqyesp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gsbbgartw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/gavwaawcm.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fktsv.cn/Article/details/gtymqafuz.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/giwaybetv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/glfzhtgao.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gitjnwqeu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gjlnwuegj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.sjlbkw.cn/Article/details/gyomhagee.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gwtfbdaan.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/gqjfjclls.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/ggzejhbgu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.sjlbkw.cn/Article/details/gyfjafpex.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/gyerfxhwk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.vehdjk.com/Article/details/gsmsakwod.sHtML

[N08] 生成全排列
来源：http://blog.yfazqb.com/Article/details/gvxosnsio.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/gxanbigkx.sHtML

PHP:  // 手写递归交换
来源：http://www.share.epnwcf.com/Article/details/gwuzloymd.sHtML

JS:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gcoarszkx.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/ggkltkiqs.sHtML

Java: // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gshrxdgyi.sHtML

Go:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gmwuhcqco.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gvktbipzh.sHtML

C#:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gkkzljrnq.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gppmkxavb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.epnwcf.com/Article/details/ggdvohnbm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.vehdjk.com/Article/details/gwrikrsfv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.vehdjk.com/Article/details/gyuhmqtln.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.yfazqb.com/Article/details/gjouyphvq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.bbcook.cn/Article/details/gxljdzsmc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.tarul.cn/Article/details/ggteprjcy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.epnwcf.com/Article/details/gzlybdrem.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/gcrhganze.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/gvfgngzgl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gmlngvdpn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/glzzsjdxk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gwzuszkmz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.sjlbkw.cn/Article/details/gjqddbovw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.fktsv.cn/Article/details/gvhqlyrix.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.yfazqb.com/Article/details/gvibrbanx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gcaewbcsx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gqxijhsit.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/gppsvrmlz.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/ggnitmsoa.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/gewjxidjl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gledzwqwq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/gjemkrzxm.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/gjjkvoddi.sHtML


<!-- 参考信息 -->