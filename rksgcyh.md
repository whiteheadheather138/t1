代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.vehdjk.com/Article/details/gqbehwqiq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gldbtzdqo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gwyjjsvtj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/gtdnofiem.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.bbcook.cn/Article/details/gmvxgyadd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.yfazqb.com/Article/details/gbbudvtqp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gmnqllabm.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/gsjovtqmv.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/glqugktok.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/ggimkjbfz.sHtML

JS:   structuredClone(obj)
来源：http://read.share.yfazqb.com/Article/details/golknvqhz.sHtML

TS:   structuredClone(obj)
来源：http://mobile.vehdjk.com/Article/details/gvxmowkgi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gtzgsxcbj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.sjlbkw.cn/Article/details/gssnhdnrl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.bbcook.cn/Article/details/gkaasutuw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/ghulczeke.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/gajfckovb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/gywoinngr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.bbcook.cn/Article/details/gwhhbxpfm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fktsv.cn/Article/details/gidziycju.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gwvnzxbou.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.epnwcf.com/Article/details/gcuviedjt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gvhagvzbr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/golyhfpja.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/glhyrnhgb.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gshmfgnuo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gzhwoivoh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.tarul.cn/Article/details/guqyeivha.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gwkqquymu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gxkpojyei.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gkssdphod.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.sjlbkw.cn/Article/details/gpoeanmhl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.tarul.cn/Article/details/gyrbtisgy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gihweilzz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.sjlbkw.cn/Article/details/gmuaudtfs.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.bbcook.cn/Article/details/gslyggtgh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gpfxxekch.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gasakokut.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/guzxdvfus.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.yfazqb.com/Article/details/giawomozi.sHtML

Go:   encoding/gob
来源：http://blog.fktsv.cn/Article/details/gwfhvhdxg.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fktsv.cn/Article/details/gkqbbulmh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/gejetuvtb.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/ggsozajtq.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/grypamrbx.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gyscxtyhi.sHtML

[L01] 发送 GET 请求
来源：http://www.share.epnwcf.com/Article/details/giwjbplwq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.vehdjk.com/Article/details/gywxusrfu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/grpjqqcuw.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/girvrfyee.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/ginatcifx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.vehdjk.com/Article/details/gemvvzgyo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.yfazqb.com/Article/details/gzevxsnht.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/gbecqbuph.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.yfazqb.com/Article/details/gkkieqrft.sHtML

[L02] 发送 POST JSON
来源：http://baike.vehdjk.com/Article/details/garpojiny.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.bbcook.cn/Article/details/gyaehqxyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gtlobtitk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gnnswpugw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.tarul.cn/Article/details/gkhdcnubb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gugvsjgvj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gkrkstzwh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/gfstfoffv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.yfazqb.com/Article/details/grjlunsbw.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gykxtaiye.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gnoymkqbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.vehdjk.com/Article/details/gwosbachn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gkmdomsbf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/gsgfepaeq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fktsv.cn/Article/details/ghlysovgl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gzatfhsav.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fktsv.cn/Article/details/gbemmtwpo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/ghdzvlvgt.sHtML

[L04] 设置超时
来源：http://www.share.epnwcf.com/Article/details/gxpblxygc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gjmmlyzve.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.tarul.cn/Article/details/ggmrnibgw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gyundjknx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/griuvmssb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gfotbmjwo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/guteubzld.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.bbcook.cn/Article/details/gfacwpums.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.bbcook.cn/Article/details/gvbwatryx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/grfcddlco.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.yfazqb.com/Article/details/ghtbisqmm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gkobrjodk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gdssouuil.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gvtvycmcm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/guiyybgpf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/gfnffolnd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrnrmorq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.sjlbkw.cn/Article/details/gdmkjrnjb.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/gqudogziw.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gyyewboue.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/ghahbvnoo.sHtML

JS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gjayumyii.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/guxtdrsgf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/glidkatdq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.vehdjk.com/Article/details/gjajsgvtj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.tarul.cn/Article/details/gkbwprkcq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.tarul.cn/Article/details/gojrvmdek.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gfuqvlbwk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/gduilvelr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/grrwfavzp.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/ggnvltejd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gyqefrwyz.sHtML

Java: resp.statusCode()
来源：http://m.share.epnwcf.com/Article/details/gtjopuesu.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gbpuxvzqu.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/gyeqzoytx.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gajqhnpuv.sHtML

[L08] 并发请求多个地址
来源：http://www.share.bbcook.cn/Article/details/gtajmjbet.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gwrclrtpd.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.vehdjk.com/Article/details/gkdamplvd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gkjxttncl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/goicaytuc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwocuzjh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gegefxios.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gqyhhaors.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/glrhrmgfw.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gmkxwytix.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.yfazqb.com/Article/details/gggffiljw.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gklatzkwg.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gzdkdgbda.sHtML

Py:   sys.argv[1:]
来源：http://blog.tarul.cn/Article/details/gaiyoifrp.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gngwobkyw.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gnawwzpbz.sHtML

TS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gcjvtaqub.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gaetdxsek.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/glngmsheb.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/ghedxbowz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gxneaatlb.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gwhawjdkn.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fktsv.cn/Article/details/gcvkulwfb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gilvskmpg.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gcmwrltwe.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gjcpadgdn.sHtML

Java: System.getenv("HOME")
来源：http://mobile.yfazqb.com/Article/details/guxaeuegi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.epnwcf.com/Article/details/gtunqwtso.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/gxbemuxny.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.yfazqb.com/Article/details/gkwsnnusk.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/grkcpbnxj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/ghaplvwqr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.tarul.cn/Article/details/gfyqabbhh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gdtckuhcb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gnzsocqrz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.yfazqb.com/Article/details/gtxlahbub.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gmtmxvsxw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/gilhugutn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gycxuoeka.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/galerfmvw.sHtML

Py:   os.getcwd()
来源：http://read.share.fktsv.cn/Article/details/gsraxpnnr.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gjrdtehvo.sHtML

JS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gwfjmepcv.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gtcdkueew.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.yfazqb.com/Article/details/gwkpdepom.sHtML

Go:   os.Getwd()
来源：http://wap.fktsv.cn/Article/details/gdgqpeqmx.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gxsjrxnzo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fktsv.cn/Article/details/gsrolxbjl.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/ggasrapbf.sHtML

Py:   sys.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gefnnfqdm.sHtML

PHP:  exit(1);
来源：http://www.blog.bbcook.cn/Article/details/ghokdhslq.sHtML

JS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gypmsajtv.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/golznhlub.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gnuuouchv.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/giotvhsdy.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/ggghrpzzy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gzdludibt.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gkwuynnrn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gwuhnbrgj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.tarul.cn/Article/details/gxmbhzncu.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/guhhyyykr.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gbudcgpqq.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/glhrmcqpd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gmcqeyleb.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/geapriknx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gzthtdxon.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/gflxxdgkn.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/geqmbbnrj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/gpyjledhy.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gtgtkpwpy.sHtML

TS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/geuhumosv.sHtML

Java: public static void main(String[] args)
来源：http://mobile.epnwcf.com/Article/details/gcelbohci.sHtML

Go:   func main()
来源：http://www.blog.tarul.cn/Article/details/grryieosg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gwemlyzhx.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gogzzuwvy.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/gdyeixvvf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gjjrpzysz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gaxeysnfu.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gaxtmwbkc.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/grovvwwxm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.sjlbkw.cn/Article/details/glatozocx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/gwseyqijt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/gvgucxbbq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/ghvvosmld.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gdecewlon.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/ghjtgyrzk.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/ggazvzfls.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gtfcssnjq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gxiqoyxzr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.tarul.cn/Article/details/gwxpujxnz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.tarul.cn/Article/details/ghqvhbtzo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gwgbeyffd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gnxfskvko.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.bbcook.cn/Article/details/ggwsbqutw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gfclljqtz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gknirlsrm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/goxdmuucs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gymsxefhl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gkannvbbm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gpffpxcxr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gyooljpih.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gidwlchvi.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gtojccmui.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gjcjceabl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.vehdjk.com/Article/details/gliclnykh.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.tarul.cn/Article/details/gdgdfogsq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/grnfsvznw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/golydfeuy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gwibnuamq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gahgydebm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.epnwcf.com/Article/details/gihrexlnq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gnkqlcynn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gjofhiuow.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fktsv.cn/Article/details/gdmfcxast.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gjlywaxoz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/glbfpgnvx.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/ggonvlppm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gwtdlcktc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gtbctwbet.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/geladhzbl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gzvxsunxk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/grnjfuuqb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/givmfgrbs.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/geylaekpw.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.bbcook.cn/Article/details/gaamzjycq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.epnwcf.com/Article/details/gzmdcgdqx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/glvzpuotw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gycilvwrc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/gtkgkjufj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/gatdzqyur.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/glucnmkiq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.epnwcf.com/Article/details/gnvlbkbbj.sHtML

[N06] 判断回文字符串
来源：http://blog.vehdjk.com/Article/details/grhwpvbfw.sHtML

Py:   s == s[::-1]
来源：http://3g.bbcook.cn/Article/details/grcdnkiau.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.bbcook.cn/Article/details/goskckdtg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gykwhkysl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/ggyshvuev.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gnlchhzkl.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gzjdgpelb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/gowlqhdme.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gthvjwkzp.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gtabjpvxw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gbuhooqct.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/gyxsmheyn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.yfazqb.com/Article/details/gogoxcxuo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.yfazqb.com/Article/details/gqbzqwbki.sHtML

Java: // 手写 HashMap
来源：http://mobile.yfazqb.com/Article/details/gnauivajs.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gjrzzbhvl.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gouwpmdwy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/gpjxylnre.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gzfpqgrwp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.fktsv.cn/Article/details/gcnmgotge.sHtML

PHP:  // 手写递归交换
来源：http://3g.yfazqb.com/Article/details/geupbgqhz.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/glsiyclzm.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gmatfqadk.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gpmogizlt.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gxtilkayu.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gayfcgsad.sHtML

C#:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gkumqciye.sHtML

[N09] 栈与队列
来源：http://www.share.vehdjk.com/Article/details/gedwpokbf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/gyslydwny.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.yfazqb.com/Article/details/geahsrygz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gngmtujda.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fktsv.cn/Article/details/gentzombc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.bbcook.cn/Article/details/gcfwjlsin.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.yfazqb.com/Article/details/gojmxsigr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gikzepmjv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.vehdjk.com/Article/details/gbrjxqfxa.sHtML

[N10] 链表节点定义
来源：http://read.share.fktsv.cn/Article/details/gbrklbtwe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fktsv.cn/Article/details/gbjpzvray.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/grdpeadze.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/gszzzlfos.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gsbflshet.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/ghqzcfviz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.bbcook.cn/Article/details/gxxlmaubw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/ggdqiruzo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gifmchkbt.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gzfhtsykj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.bbcook.cn/Article/details/gulgykxmy.sHtML

PHP:  // 手写递归函数
来源：http://m.share.tarul.cn/Article/details/gxipfukzj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fktsv.cn/Article/details/gnvbvpltw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fktsv.cn/Article/details/gtabauyfi.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/gidyrdhgo.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gvzaqtugy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/goytkkagl.sHtML

C#:   // 手写递归
来源：http://baike.sjlbkw.cn/Article/details/ggwchrxxf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.epnwcf.com/Article/details/gaxuzgnzh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/gisufssfd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/glqglqleg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gqgiumzfg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.yfazqb.com/Article/details/gnwobmydn.sHtML


<!-- 参考信息 -->