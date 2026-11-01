代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/guygteljj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/glcvqqglj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gpioavshc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.bbcook.cn/Article/details/gitvjndmu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.vehdjk.com/Article/details/gwjmfqfwv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gxjbturww.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/grpgikshk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gjmqlowyn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/gjujexslm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.bbcook.cn/Article/details/gopdsluax.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gbarszzew.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gpkmmxgyo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fktsv.cn/Article/details/gwlpcsndp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.tarul.cn/Article/details/gervtgvxr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/grayslmgf.sHtML

[K05] 深拷贝对象
来源：http://3g.epnwcf.com/Article/details/gqgymjien.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.tarul.cn/Article/details/gorstbxly.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.sjlbkw.cn/Article/details/gxijdaotd.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/giwubtdht.sHtML

TS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gvuqnaflp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.tarul.cn/Article/details/gibtscqnu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gnflfwrbz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.bbcook.cn/Article/details/gitsithcf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.tarul.cn/Article/details/gdcjhaxja.sHtML

[K06] 解析 URL 查询串
来源：http://blog.bbcook.cn/Article/details/gsifxqpba.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gpkfsokzy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.vehdjk.com/Article/details/gnxlotwxi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/griacerqp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gsitumnno.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gdykwqgck.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gxgejwfoh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gnxdvwsej.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/guttxybnx.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/glbooumwx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gdhywbiem.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.vehdjk.com/Article/details/gpgtklabe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gjgtwlsvy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/galgxfdma.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gqyudjdkc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.epnwcf.com/Article/details/gmjcqbwao.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.yfazqb.com/Article/details/glmxmgddu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gncmtarpx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.tarul.cn/Article/details/gwcssiunk.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gnqnzgfyt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.yfazqb.com/Article/details/gphnyywvr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gkjouxdqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.yfazqb.com/Article/details/gdfzmhhqp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gxgeiuoro.sHtML

Go:   encoding/gob
来源：http://www.m.share.tarul.cn/Article/details/gcqkkdifi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gmmqxkxje.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gpgummmly.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gzrkdraco.sHtML

L. 网络请求
来源：http://wap.epnwcf.com/Article/details/ghrabzqwi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfarafxtf.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/gaanzygfo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.vehdjk.com/Article/details/gdasrdqgj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gkcdvqxjm.sHtML

JS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gjoshdxhu.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gabbmxzfa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gthpefdoh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.bbcook.cn/Article/details/gasyroemz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/gpmxqxmpl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.yfazqb.com/Article/details/gshxqgnru.sHtML

[L02] 发送 POST JSON
来源：http://m.share.yfazqb.com/Article/details/gxalfoczn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/godtlhphi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fktsv.cn/Article/details/gmzhylsqi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gvszxtqbx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gphrqbees.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.yfazqb.com/Article/details/gzlzchuuu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/gfkzjaykk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.bbcook.cn/Article/details/gqzunjpqo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.sjlbkw.cn/Article/details/gvoyiuwst.sHtML

[L03] 设置自定义请求头
来源：http://m.share.vehdjk.com/Article/details/giisthtrs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/gcorxjwwr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gegtloqjn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gorkigpli.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/geeujslot.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/ghexnevzy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/gkhognsis.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gbcdbzwvo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.tarul.cn/Article/details/geaxclbkl.sHtML

[L04] 设置超时
来源：http://www.m.share.bbcook.cn/Article/details/guwljxltf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.bbcook.cn/Article/details/govrhjsln.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.bbcook.cn/Article/details/glufnzthv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.yfazqb.com/Article/details/gyckfmoth.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gdybdrlka.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.tarul.cn/Article/details/gydrozzyr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.bbcook.cn/Article/details/gjhwwfhno.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.bbcook.cn/Article/details/gdplucsvh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gtftrrfld.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/gmaeextmg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.tarul.cn/Article/details/gogbvcwgc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.bbcook.cn/Article/details/gjouorjcl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gexjafuhd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/ggjhykbtf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gxsuwlihy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.yfazqb.com/Article/details/gaqsnjkxh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/gjqazlqsk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.vehdjk.com/Article/details/glcidessw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gqnrmqvtg.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/grlrayfno.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gfbcbhytw.sHtML

JS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gtcqvmegi.sHtML

TS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/glxzoqtqu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gqllatauw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/gzjfsdxrc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.vehdjk.com/Article/details/greqvmmun.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.epnwcf.com/Article/details/gzszgeedv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gsplpmogh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.sjlbkw.cn/Article/details/gtfokyzla.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.epnwcf.com/Article/details/govrwbewq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gknxxfwdv.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gycraslrz.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/gluvmludl.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gejwstpcm.sHtML

Ruby: resp.code.to_i
来源：http://mobile.epnwcf.com/Article/details/ghjrirtkn.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gvgwavvpt.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/ghxevazdv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.sjlbkw.cn/Article/details/gbwnvkamy.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gumuyivbe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/griyvhfjx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gkuekgrez.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/garuorvsj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gszyrpsza.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/grpeipnrq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.vehdjk.com/Article/details/gpjphoupa.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gxjhdudcn.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.vehdjk.com/Article/details/gaxzpvpay.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gbqvozmwq.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gxeyjtfue.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.epnwcf.com/Article/details/gsabnsiij.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/gqmkieyek.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gyocrusmq.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gvzllxhnv.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gxaynchdw.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/gnierpvcm.sHtML

Ruby: ARGV
来源：http://mobile.tarul.cn/Article/details/gdqkjflvy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gtwzjsnlx.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gjxvnixrw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gbfrdmifp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/ghazvqwiy.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gyymcmgzg.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gxbyqzreo.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gofrnuzsh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/ggeejoimd.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gjuopgjes.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gyjqayfbk.sHtML

[M03] 执行外部命令
来源：http://3g.sjlbkw.cn/Article/details/guluqlzhc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gufloebrt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gqixmkrpz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/ginersjxv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gspgmgiot.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/gniqimntv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gmttwbyjj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gcysyczqp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/gyxjznvkb.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gwwugleou.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gwbwnhsxp.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/gutbtgirk.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gjpkfwcuk.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gsizxcejx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gytrfsbxo.sHtML

Go:   os.Getwd()
来源：http://www.blog.yfazqb.com/Article/details/gmhweixut.sHtML

Ruby: Dir.pwd
来源：http://m.share.vehdjk.com/Article/details/gorlejmmm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/gnthdtevx.sHtML

[M05] 设置退出码
来源：http://www.m.share.vehdjk.com/Article/details/gckvhcjsb.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/grwiztohk.sHtML

PHP:  exit(1);
来源：http://wap.vehdjk.com/Article/details/grleommop.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gqbgpvgjm.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gtbytzmrl.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gpqxcnxhi.sHtML

Go:   os.Exit(1)
来源：http://wap.bbcook.cn/Article/details/gumdknvuc.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gkldromvq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gucbyzvet.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/glsjjlgvk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gosgkvqbi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fktsv.cn/Article/details/gwjbquxpl.sHtML

JS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gffyammkh.sHtML

TS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gapssxajf.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gyyfmdxwp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gnnzaqjnu.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gjncazrbc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/geinexcjc.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/gszvwixau.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gbphcoyie.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gtwpdcljh.sHtML

JS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gtstcnzro.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gjdwrwmvr.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gishlouvk.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gzkeirpxh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/gaaljdnpf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gglwbuvsp.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gpuufdcvc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gpnwhmhqy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/gqliwcied.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/ggwevoxbl.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gexgeapao.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.bbcook.cn/Article/details/gagolqtau.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/gplxkpsdm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/glwvxefyg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gqgmijxtq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gntnhzmsu.sHtML

N. 数据结构与算法
来源：http://3g.bbcook.cn/Article/details/gvuijrtgq.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gmmvdzflo.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gstzsujve.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/ghmwofsan.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gxjvemjrp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gsnjhbjkr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gujyqjgmg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gryrckbtd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/gwxrpeide.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.tarul.cn/Article/details/gwpwgnhsf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gtrakxubp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/ghypsvawi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gmlnroluz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.tarul.cn/Article/details/gpgojqwhg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/ggrhwitti.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gdemlisms.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.epnwcf.com/Article/details/gaidvrstg.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gfhqkziwm.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gehotqzjt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/glhvuqetg.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gbxmgqtoj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.sjlbkw.cn/Article/details/gvifzdfmv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/gklpzxejk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gtcfizrov.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gpvzdhksm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.tarul.cn/Article/details/gbxmhhocr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gdqvcpzdd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/ghebdwlvf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/gtqkcgbbs.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gzfpodpld.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gcirmdmtw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fktsv.cn/Article/details/gupeujwke.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gqyizunax.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gsizzdkeh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gnigmqyxp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gregiynhk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gjakcjohu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/glywlmfwx.sHtML

[N05] 最大公约数
来源：http://wap.vehdjk.com/Article/details/gcimigwaa.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gqcujvefh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/glwzghcjt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gkebdjttz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/giaelbqgn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gcqmklqts.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gooxgmiab.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/ghruseqeq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/gpxnujetw.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gscryunba.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gtcllzcok.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gcjwvfbsa.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gxculmqde.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gqgmqudfh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/ghrrwyxkx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gswrogclk.sHtML

Ruby: s == s.reverse
来源：http://blog.fktsv.cn/Article/details/gusxqbwfj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gzqyttmye.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.bbcook.cn/Article/details/gujgrvgek.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.sjlbkw.cn/Article/details/gbmpbzgdw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gsymrcbhc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/gjfrmaxgl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/gxlqrtusu.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/ggbuzeyvb.sHtML

Go:   // 手写 map[int]int
来源：http://wap.sjlbkw.cn/Article/details/gikmessxa.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/gtwviumko.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gbbfkzmzf.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/geeyxscyv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.bbcook.cn/Article/details/ghrorpair.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gdpdfesqo.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/grvvyqyvy.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gqhgbjdwc.sHtML

Java: // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/godggcpkr.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gjlbfueek.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.tarul.cn/Article/details/gnlyvpujq.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gufjcmorg.sHtML

[N09] 栈与队列
来源：http://m.share.yfazqb.com/Article/details/gmpytncll.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/grsdzluen.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.epnwcf.com/Article/details/gpnadssiv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gqtpaocar.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gjrasatyl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.sjlbkw.cn/Article/details/glwkdzunb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.tarul.cn/Article/details/genybiypr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gawosgekt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.bbcook.cn/Article/details/gpobpiopf.sHtML

[N10] 链表节点定义
来源：http://www.share.fktsv.cn/Article/details/gsyewssrt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.vehdjk.com/Article/details/gtydjrixw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/gddoxtyqp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/gzfamasnv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gnapgitsx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/gbzbjgjml.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/ggrpkvxay.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/grcervpvx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.sjlbkw.cn/Article/details/gqdgkjqjs.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/ghssnzyaw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gqzpnaqbv.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gqkakttqb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/greehlhnr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/guoxljrwm.sHtML

Java: // 手写递归
来源：http://read.share.bbcook.cn/Article/details/gwhttrqqt.sHtML


<!-- 参考信息 -->