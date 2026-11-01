代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gfmqmxuus.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.sjlbkw.cn/Article/details/gzawfhtqy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gqjxbvjeo.sHtML

[K05] 深拷贝对象
来源：http://3g.tarul.cn/Article/details/gvncopbop.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gsiczkqbg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.epnwcf.com/Article/details/genkwlynx.sHtML

JS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/glpdzdudz.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gmfotpegq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.vehdjk.com/Article/details/gynagbprc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/genebdvnb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.tarul.cn/Article/details/gncegzqas.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gjnqytknh.sHtML

[K06] 解析 URL 查询串
来源：http://blog.epnwcf.com/Article/details/gvzdaqxrj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.bbcook.cn/Article/details/gbczlrbtp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/ggeyencir.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.sjlbkw.cn/Article/details/gbzuavkyn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fktsv.cn/Article/details/gdmxchkfo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.tarul.cn/Article/details/gwnvxvpph.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/glugdkuha.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/gmxtmavei.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gqkqyoeoc.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gmsaintrj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.yfazqb.com/Article/details/gsygwcpwn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gbgrnyeew.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gorqcdvuq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gsinqprhy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gpklwawsi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fktsv.cn/Article/details/geqqpbeiz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/gqdkpuyin.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/ggflompxt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.vehdjk.com/Article/details/gxmopbdzw.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gvevvtbgj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/giwapvnhr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/ggectxmbp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gflwjcclu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gggtkvhrv.sHtML

Go:   encoding/gob
来源：http://baike.tarul.cn/Article/details/gczjfnymj.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gwqczkglr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fktsv.cn/Article/details/gxxbwuron.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gmkzujmwp.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gakrxmfuh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gcgnvxdsa.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/goggohkbo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.epnwcf.com/Article/details/gxblhgnud.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gpmfdpaud.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gmawrrpwm.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gwssmtgvp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gbjlswybp.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.tarul.cn/Article/details/gcgwpkiid.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/gvsrsiuea.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gxkwrtgps.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gdsfkfgyi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/ghfcdertw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.vehdjk.com/Article/details/gyqiicpqe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gemfunnmc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gvnaawsra.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/gaddmguip.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcfzlltzp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.vehdjk.com/Article/details/ggdjvbjxm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.vehdjk.com/Article/details/gcshlqdre.sHtML

[L03] 设置自定义请求头
来源：http://wap.fktsv.cn/Article/details/gltozffjd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.tarul.cn/Article/details/gpqrwzrmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gguwxhlmt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.sjlbkw.cn/Article/details/gsgrnemmj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gswqvxvvz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.vehdjk.com/Article/details/gwlmzlgnh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gpnujtcsw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.epnwcf.com/Article/details/gmyjytxhn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gaavncefc.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gtwkzqvri.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/grmihbbci.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gbhrhgtvr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/grqbavndr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gunhzpnir.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/gpoztqnum.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/ggyvadxbz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fktsv.cn/Article/details/gtwoiidmn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/gzneslxxi.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.epnwcf.com/Article/details/gdmfcwwuu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.bbcook.cn/Article/details/gxyvhxeuv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.vehdjk.com/Article/details/glnxxhebg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gxexaprse.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gbigxerhc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/gzuwzcjuy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gkwkhqavc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/goxstbscw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/gfvtsitvp.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gqzptqyke.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gcyfszwvl.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/ghlzuyihg.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gokcqfhpw.sHtML

TS:   await resp.json()
来源：http://3g.yfazqb.com/Article/details/gekzcajuq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gqjuumird.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.epnwcf.com/Article/details/ghfjgiyob.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gcoabdegi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gdnexhtel.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gogtxwgxq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/ghmsridpv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gtqlspynx.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/ggiittijm.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gwlnjqfue.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/gzoksbdvc.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/guiwneztz.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/gwvziovrs.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gnxqrcuqn.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gxsztusob.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.yfazqb.com/Article/details/gmdtfnsoz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/ghctriyuc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gezvjgwyw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gnvwihlkf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.epnwcf.com/Article/details/gtimjckin.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/glrvvcgfw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/guftnpjlu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gvtsagwrx.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/ghgvovnvv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.sjlbkw.cn/Article/details/gpgjbmbnv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gtlvgrecy.sHtML

[M01] 读取命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gedzhslgc.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gwwwdtane.sHtML

PHP:  $argv;  $argc;
来源：http://blog.vehdjk.com/Article/details/gqapaynvq.sHtML

JS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gicsblxvo.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gqtmpsdqi.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gcdrhmzlk.sHtML

Go:   os.Args[1:]
来源：http://blog.bbcook.cn/Article/details/gghvkrfnu.sHtML

Ruby: ARGV
来源：http://mobile.epnwcf.com/Article/details/gtxpsptbc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gtbzxbukr.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gcztmeqjd.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gulzgawlo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.bbcook.cn/Article/details/gfldmmdxn.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/guxqwjjcu.sHtML

TS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gzjfnebff.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gfvmrebcm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gdidxqdsa.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/gpymykpqx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fktsv.cn/Article/details/gatzmvitz.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/geqwuiflj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gzmidbrtz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gwvscapmj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/guloduoky.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gjuybfkkw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.bbcook.cn/Article/details/gcuxfsmwb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/gytpghtxn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.sjlbkw.cn/Article/details/gkiicohjk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/grjrskzno.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.sjlbkw.cn/Article/details/gmmythzqb.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gwxengaui.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/gbbwfsysb.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/gcnihkayo.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gbkbuarwp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gaftrhyzi.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gogulydkz.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gxzwzwcmn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.yfazqb.com/Article/details/gjhpoouoa.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gikxlmptt.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gvqfjybmy.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gmbdqeipc.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/grkbxjaem.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gcnrssjtb.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gjiomskis.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/ghubbfblb.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/gmyimkpzf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/grtimcczj.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gfmhvqyfb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/ggklunays.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/gmvwhplyf.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gfrynvhsn.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gpoachwsb.sHtML

Java: System.err.println("err")
来源：http://www.share.sjlbkw.cn/Article/details/gavmdsaxy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.bbcook.cn/Article/details/gjtamkciz.sHtML

Ruby: warn "err"
来源：http://www.share.tarul.cn/Article/details/gzwtcxigx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gcvazttyi.sHtML

[M07] 判断是否为主入口
来源：http://blog.epnwcf.com/Article/details/gmpmekqdt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gqwyozapi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/gzejlfdfr.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gcdkdfzjr.sHtML

TS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/glgnigvdj.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gfviemybw.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gfhegvhuj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gnqrzxcgx.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/gbdlluknv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.vehdjk.com/Article/details/gtclhehrz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gwlkqcdgd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/gkadhljgk.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gyzkpvcxs.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gyhhervtk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.sjlbkw.cn/Article/details/gcrgjmtcg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gxrxepkgy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gmyjevter.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gnbpvtdpu.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gosejzoxa.sHtML

N. 数据结构与算法
来源：http://read.share.tarul.cn/Article/details/guwrmswjb.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guwvyufku.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gvgpjztyl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.tarul.cn/Article/details/ggnkajqza.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gwcaweysn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/ghzrzufoz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gomtihzdo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gsustogqr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/ggcmvetrq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/gopxfjpaf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gwapchcum.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gspazahqj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gzqdnlreh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/glkjfqfxv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/ghsgdalwi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/grrpbzwyj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/ghaxcvsiq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.bbcook.cn/Article/details/gkbizfwml.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gusitekoz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.vehdjk.com/Article/details/gazvpqafz.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/gnnojaoez.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/ggkifwgbr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/ghjoxpplm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.yfazqb.com/Article/details/gdsuhmvpu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gfwphteqa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gpxamufhg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/geqglzjwy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.yfazqb.com/Article/details/gxlgvtkop.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.sjlbkw.cn/Article/details/gwysinzcy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.vehdjk.com/Article/details/ghawchvaq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gkcoevuvc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/ghrmvbsfc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gynbchsnx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gtmbtpxtn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gqhvucnvo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/gviwlwyqe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gfbvkhzmc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gqntviyxp.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/gelxqkxof.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gljoebpvb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gkvkjvrve.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gyvqpeibr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gqedezcqn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.epnwcf.com/Article/details/gjfxmusep.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/gzswneuto.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gkwbfdray.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gwtqnddgc.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gqjvutecu.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/glwbizgtn.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/greiwwqso.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/gnidkwzbo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/grxuuktai.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gjlpotcbq.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gdzzufxdc.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/garzsaago.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gswkzfivd.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.sjlbkw.cn/Article/details/grgwffual.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/gusfequyf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gpsiahzfl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.tarul.cn/Article/details/gwnhmlkxl.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gkjhfqwgx.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/gycdveofy.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gianpxhfn.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gpbryokri.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fktsv.cn/Article/details/gtkgyxmhr.sHtML

[N08] 生成全排列
来源：http://www.m.share.fktsv.cn/Article/details/gwnfckdou.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.bbcook.cn/Article/details/gaoqmdyih.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gdvildljy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gbcsxoygy.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gxepgayln.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gfgxciiso.sHtML

Go:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gpefxgfap.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fktsv.cn/Article/details/gsdnomsns.sHtML

C#:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gfjyvuhmm.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gvvwumbvc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gxlnolvlg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gryayufli.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gvqhoebtp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gdtxywybj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gqcnpfvru.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmgwhean.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gmobzvamv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gkwshpsca.sHtML

[N10] 链表节点定义
来源：http://www.share.bbcook.cn/Article/details/ghddbzicc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gxytayqbc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.bbcook.cn/Article/details/gyomoxpeq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gwqvbdpda.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gtluerrwl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.epnwcf.com/Article/details/gdaqazyip.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.bbcook.cn/Article/details/gzlsnwijk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/gakjnecsk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/ghhnmqvof.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.yfazqb.com/Article/details/gvztyeizr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gypqafeav.sHtML

PHP:  // 手写递归函数
来源：http://www.share.epnwcf.com/Article/details/gfrrfmgxl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gukgyuujl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/ggreegjgi.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gengftduj.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gfrrsohnr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.epnwcf.com/Article/details/ggfgpqzmp.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/gcmkkzcco.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/gwyvwfngd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.tarul.cn/Article/details/gxgnoljap.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/gzcjkmylc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gniehrqbf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.yfazqb.com/Article/details/gihflrhhe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/gyzxtqjak.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/glpycrzvg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.epnwcf.com/Article/details/gbbhriejw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gvjiwloks.sHtML


<!-- 参考信息 -->