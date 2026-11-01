代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.yfazqb.com/Article/details/gwnvmcycy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/gdhlogoac.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.vehdjk.com/Article/details/gcfwyohlx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fktsv.cn/Article/details/gdepzsani.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/gnigzhldf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gybhkuiqu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.bbcook.cn/Article/details/gsjwknkbz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/goqadiwqo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.tarul.cn/Article/details/gountldsr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.bbcook.cn/Article/details/gqqafzltv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.vehdjk.com/Article/details/gtegrsurn.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/gwxgpglnp.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/gooiayozs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.bbcook.cn/Article/details/gsgsdspaw.sHtML

JS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/gfllyrxib.sHtML

TS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gbowlrfcz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.vehdjk.com/Article/details/gmzdfqahy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/gqvscehbn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.sjlbkw.cn/Article/details/gayhgddfq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gwjaogwaz.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gwwzngrdn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.tarul.cn/Article/details/gofhktghj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.yfazqb.com/Article/details/gpgyszpzo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/ghukaqkrw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.bbcook.cn/Article/details/gxtdzpcxk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gdpabkwmt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gwlgmnmgj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gqooupwkl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gqrtmokxv.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gessezbrg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gjfnbkaqd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.sjlbkw.cn/Article/details/gctnferrr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gpirzekmh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gwplaqiyf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gjottayqu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gshxxfvuo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.yfazqb.com/Article/details/giuagsiqw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gzdzvpusn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.vehdjk.com/Article/details/gttobholz.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.vehdjk.com/Article/details/gwtwqxnfh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gmehklvca.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gxoohodfl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gtjfcogcj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.tarul.cn/Article/details/gnnuiuumr.sHtML

Go:   encoding/gob
来源：http://blog.yfazqb.com/Article/details/gdnmazlta.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.vehdjk.com/Article/details/gsznclrqi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.sjlbkw.cn/Article/details/gocouetjl.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gacuzdtfm.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gcvuywpjg.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/geecghqyy.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/ggegaqvyu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.sjlbkw.cn/Article/details/gmopquwdr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gestdnglk.sHtML

JS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gfzlkupiq.sHtML

TS:   await fetch(url)
来源：http://baike.bbcook.cn/Article/details/giciunlbx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/gobawmhld.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/guflakodw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/gcjopeuxs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.bbcook.cn/Article/details/gonewjunv.sHtML

[L02] 发送 POST JSON
来源：http://blog.sjlbkw.cn/Article/details/gssyfcjiv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fktsv.cn/Article/details/gbkyfqpib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.yfazqb.com/Article/details/gkotjrjzh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gkyhiortm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gbcuaqqcr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/gokoqbsts.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.sjlbkw.cn/Article/details/ghgzploxt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fktsv.cn/Article/details/gnxyetgar.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gbulwnlbq.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/gsvpmrgbw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.yfazqb.com/Article/details/gdccijqxy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/gsgpudfem.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gdutefhma.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/geeoebktg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.epnwcf.com/Article/details/gqeibhdxn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/grghfbinz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.tarul.cn/Article/details/gcffearaj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.tarul.cn/Article/details/gnirjornt.sHtML

[L04] 设置超时
来源：http://www.m.share.sjlbkw.cn/Article/details/glamvomqw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/ggacvndvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/garnbsvuf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.tarul.cn/Article/details/gqbqlvocl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gmcajnmns.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/gqzwnlvlw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fktsv.cn/Article/details/gndrnbehq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fktsv.cn/Article/details/ghcqefwfx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gcmvbaflb.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.yfazqb.com/Article/details/gxfscmmzi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gibbyroig.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.sjlbkw.cn/Article/details/genejqelu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/giuqqmgnw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gwuipxeqg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.yfazqb.com/Article/details/gqgwbwfwo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gceqakjya.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/grlqfqrsv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.vehdjk.com/Article/details/guhollfny.sHtML

[L06] 解析响应为 JSON
来源：http://wap.sjlbkw.cn/Article/details/gfkwsoubm.sHtML

Py:   resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gmvpcyouk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gtbqdhvgi.sHtML

JS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gxwhgiqvm.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/glsdewvpw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcevivhvg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.vehdjk.com/Article/details/gsbjgumfh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.yfazqb.com/Article/details/gyhkjlsua.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfajeopp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fktsv.cn/Article/details/gqgvlimln.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fktsv.cn/Article/details/gpjoqfqbe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.yfazqb.com/Article/details/gkbplkeuf.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gnnchqcek.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/guefotgaj.sHtML

Java: resp.statusCode()
来源：http://read.share.sjlbkw.cn/Article/details/gxovdydja.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.fktsv.cn/Article/details/gtlymldnz.sHtML

Ruby: resp.code.to_i
来源：http://m.share.yfazqb.com/Article/details/gojjbqzlv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gntclsqhs.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/glhznxsny.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/gaxnveazc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gzdqfutrv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gvwkbabbt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/guonatsgy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gucnuzvjp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.tarul.cn/Article/details/grpmfzmko.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.epnwcf.com/Article/details/gqbptdszl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/goqhsdpmc.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gipdwntbw.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/goemnvcdu.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbvijedsk.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gikrvibfz.sHtML

Py:   sys.argv[1:]
来源：http://3g.epnwcf.com/Article/details/gnualhrxl.sHtML

PHP:  $argv;  $argc;
来源：http://baike.bbcook.cn/Article/details/gwiiffsfo.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gripcrfmt.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gzugumcjg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gzitssrcu.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gkvcqkerl.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gmodthxfo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gwnnxemvc.sHtML

[M02] 读取环境变量
来源：http://www.blog.fktsv.cn/Article/details/griygzamo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gjnzxxwxu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.bbcook.cn/Article/details/gaqifyyhj.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gbqgkdnca.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gbvrxwvyb.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gyfspzwpj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gmejcazfk.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/goaurkrhj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gaxjwmqlq.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gxzuawnuh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.bbcook.cn/Article/details/gghqggrpn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.tarul.cn/Article/details/gilvwyxlf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gexbatyyp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gjnyvkatj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gwovxdoht.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fktsv.cn/Article/details/gxhmjicpu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.epnwcf.com/Article/details/ghdpgjayc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.bbcook.cn/Article/details/gasfploey.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/gzrcgxdlv.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gjsjfjduy.sHtML

PHP:  getcwd();
来源：http://www.blog.fktsv.cn/Article/details/gzjtqstlz.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/goqlmqcor.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gcsmtnfgc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/gagvahlqy.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gucnaabjq.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gllxeuzus.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gupsjcoqh.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gvdqnpblf.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gicfwizuw.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gonmoyoww.sHtML

JS:   process.exit(1)
来源：http://blog.fktsv.cn/Article/details/gcmrbujfb.sHtML

TS:   process.exit(1)
来源：http://read.share.vehdjk.com/Article/details/ghknrczzk.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gxzrxryiy.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gxjlqforz.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/gqdcdwdme.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gatdnbbxw.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/gmijkirkg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gqdjmgzqf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.epnwcf.com/Article/details/gjnxqvvqs.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gajmdrmex.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gevocazmk.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gvykekdrl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/grfgenrbg.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/grzhowcmh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.vehdjk.com/Article/details/gyekoyuil.sHtML

[M07] 判断是否为主入口
来源：http://baike.epnwcf.com/Article/details/gvauyhpkd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gvafclyxh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gasyypjiw.sHtML

JS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gznxqzmgz.sHtML

TS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gdclfmdee.sHtML

Java: public static void main(String[] args)
来源：http://read.share.tarul.cn/Article/details/gfnmqbkmm.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gwoncrwmb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.yfazqb.com/Article/details/glzwyechl.sHtML

C#:   static void Main(string[] args)
来源：http://3g.sjlbkw.cn/Article/details/gqajzlimu.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/grybtoujl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/glhnxkjnv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.bbcook.cn/Article/details/gdhsrivqk.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gkpyhfrbx.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gmhwenlyb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gakuhrclz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fktsv.cn/Article/details/gyubdtytt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/ghquiorec.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.tarul.cn/Article/details/giibjjtgy.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gcmnpgfoc.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gyfpkouhp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gboecgjmg.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.epnwcf.com/Article/details/gikzrdzdu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/ghmzdjmhm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.bbcook.cn/Article/details/gaokihucd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gmvfdeopg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.yfazqb.com/Article/details/gsenpkvkt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gxwptgdtv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gcaxtjusl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/gpmszpjnn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gmtrnmtfa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gylxjjeri.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gvrcqvvgj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gesgubgxh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.vehdjk.com/Article/details/gzhjciixt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/glxjljkki.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/gsktoxzqb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fktsv.cn/Article/details/gobvqxovu.sHtML

Ruby: arr.sort
来源：http://www.share.vehdjk.com/Article/details/gcohoxuqc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.sjlbkw.cn/Article/details/gxrocoqio.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gtmxblrnz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.bbcook.cn/Article/details/gykzayshy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/gwchfrxmk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.tarul.cn/Article/details/gcsgnutre.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gmjeammzk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/glfxcaymu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/gkfekvtoh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gdutoalzb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gchghdwnt.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gjlmfxbjc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gjugmjyid.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gdnomrugw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gjtrhqsbi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gbkqccgmi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fktsv.cn/Article/details/gvvbpsddc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/gvffpmxhj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gknfdblsi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gnporxxis.sHtML

[N05] 最大公约数
来源：http://read.share.yfazqb.com/Article/details/gasnglnba.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gjszlyocr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gxsnxrqom.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gzainxbta.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gdhrymgbe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/gvvqekozo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.yfazqb.com/Article/details/guqzkfvdu.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gywdozqcp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.yfazqb.com/Article/details/gbgfczlcz.sHtML

[N06] 判断回文字符串
来源：http://www.share.yfazqb.com/Article/details/gfmlxizhn.sHtML

Py:   s == s[::-1]
来源：http://wap.vehdjk.com/Article/details/ggnuwyjpb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gohtwjvbe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gosttfaub.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gneiqzkgi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gjxenmrhg.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fktsv.cn/Article/details/gujsyhhgz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gbykrayms.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gyxydtrqo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gkzktgqtx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.tarul.cn/Article/details/gffvvbvmj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fktsv.cn/Article/details/gdqofyouf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.sjlbkw.cn/Article/details/gbxegotsh.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.epnwcf.com/Article/details/gtgdhdzrm.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.tarul.cn/Article/details/gidxdcfrk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/ggdgqpara.sHtML

Ruby: // 手写 Hash
来源：http://3g.bbcook.cn/Article/details/gzgrydlxz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.bbcook.cn/Article/details/gvbzmpwyu.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/gkhyqikvl.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gnuqayhhu.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/goxeecpaa.sHtML

JS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gdayqxvjb.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gnmmnncnt.sHtML

Java: // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gsirvtymv.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gfdmevqbs.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.bbcook.cn/Article/details/gmuedswij.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gstswozui.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gfusgcgga.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/grndhnnxm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gpuwmpazr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/ghysrozlk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gqmsjdetc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.yfazqb.com/Article/details/gwecjhuch.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.epnwcf.com/Article/details/gfvifzsve.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gugwjqisq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.yfazqb.com/Article/details/gbgxfsbtw.sHtML

[N10] 链表节点定义
来源：http://3g.sjlbkw.cn/Article/details/gklstlpto.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gcoiehaoi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gxwqjvhgp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gqqgwmyso.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/gehuxpkuw.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.epnwcf.com/Article/details/gfijpqkri.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gkjwtfnsi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.vehdjk.com/Article/details/gzfnmtiht.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.tarul.cn/Article/details/gfvhwjfhd.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/gyeucgxic.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/gokiwabwy.sHtML

PHP:  // 手写递归函数
来源：http://wap.bbcook.cn/Article/details/gmuoohhaq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gumymzfsu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/gmaknlbjx.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gbqcsnpqe.sHtML

Go:   // 手写递归
来源：http://wap.sjlbkw.cn/Article/details/guzujvjxi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/gxifiisdw.sHtML

C#:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gtgbhwwqz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.tarul.cn/Article/details/gnqomclpy.sHtML


<!-- 参考信息 -->