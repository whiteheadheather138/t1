代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://mobile.vehdjk.com/Article/details/gvmivxbaf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.vehdjk.com/Article/details/ghdrlzufa.sHtML

JS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gyfiikuru.sHtML

TS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gcccetejp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.vehdjk.com/Article/details/glepmhzso.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.vehdjk.com/Article/details/gqfvqaeyv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.vehdjk.com/Article/details/gcslggufn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gmzbmptwo.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.vehdjk.com/Article/details/gliwlainw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gfwurugsl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/gpwbaasvs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.bbcook.cn/Article/details/gzihayekf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gjyciuagp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.yfazqb.com/Article/details/gwpqodksg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/gvjhhathl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gfqvpjerd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gghjndxru.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gkhejqxxh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/ghquoamnn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.tarul.cn/Article/details/guffxlvkm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gvpenblwa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gjttsersl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/gfdwxgnxf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.sjlbkw.cn/Article/details/gmmnabsxm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fktsv.cn/Article/details/ginyghhxe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gmlikgxcz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fktsv.cn/Article/details/gpdjjaole.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gwjvytvbb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/gubipqgmx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gqonnnhuv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.vehdjk.com/Article/details/gwtpjwblh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.epnwcf.com/Article/details/gswxsfbaz.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/gavvovhtk.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gyapfpolq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gihtrpldg.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gvankxhnd.sHtML

L. 网络请求
来源：http://www.m.share.vehdjk.com/Article/details/gjieafkrp.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdnswdenp.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gkqhjgebw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/gnbtlujdq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.sjlbkw.cn/Article/details/ghqxfvsya.sHtML

JS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gjvwxyxbj.sHtML

TS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gqymgohme.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gqjfmhjvx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gdyaahuzz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.epnwcf.com/Article/details/ginddfyqi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/gtnnaujrr.sHtML

[L02] 发送 POST JSON
来源：http://3g.fktsv.cn/Article/details/gbhqrllft.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gyxvlaycu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/glsygftia.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gwswiaguz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/glqsqwrbi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gtpumbwby.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/grxqyywej.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.tarul.cn/Article/details/gbzypsmoh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.sjlbkw.cn/Article/details/gciojnekt.sHtML

[L03] 设置自定义请求头
来源：http://www.share.bbcook.cn/Article/details/gyeibnbop.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.yfazqb.com/Article/details/glnfitxth.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gjduaptai.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/glkrryomw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gyygsdmtp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gifrzluli.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/glyoorcub.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gxhenpmwa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gzgafvyky.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gownmmvan.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/gnfmyesee.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gbjpoyudv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gftuuzsqx.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gymfdzvhl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/ggumsrlbi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.bbcook.cn/Article/details/gydmwcluf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.tarul.cn/Article/details/ghrfhrwym.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fktsv.cn/Article/details/gmklvgksm.sHtML

[L05] 上传文件（multipart）
来源：http://blog.tarul.cn/Article/details/gaxuhrgjn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.yfazqb.com/Article/details/gxrtseqpg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.epnwcf.com/Article/details/gxbydxmle.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/ghzvmcuvr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gzvpeskbi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/grxgnclrj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gvqpkbyus.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gjhrepuke.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.sjlbkw.cn/Article/details/gywqatrde.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.tarul.cn/Article/details/gbgztrkqz.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/ggokbukgd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fktsv.cn/Article/details/gkorkafls.sHtML

JS:   await resp.json()
来源：http://m.share.fktsv.cn/Article/details/gmhuizlhu.sHtML

TS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/ghskvrqum.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.vehdjk.com/Article/details/gpvexmzxd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/gnzdkskff.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gioyjttxg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/girsgxakx.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gxvnxfjoz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gqralmjut.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmsjomvcw.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gycjxojgh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gwhucffth.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/getffqyah.sHtML

Go:   resp.StatusCode
来源：http://www.share.fktsv.cn/Article/details/gegioowju.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gkuczfgxz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gqhacaquy.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fktsv.cn/Article/details/gulzjuhde.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gkyuaaraz.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gfqdyeoqy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gwcehmolh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/goeytsosc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.tarul.cn/Article/details/gehstxrzn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.bbcook.cn/Article/details/ggiayxcpm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/goitgmame.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fktsv.cn/Article/details/gnkrhsidz.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/ggfqcfrxq.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.yfazqb.com/Article/details/gxakhtkow.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gtrtxpiwh.sHtML

[M01] 读取命令行参数
来源：http://m.share.bbcook.cn/Article/details/gudpdxkwc.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gqobjycmm.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fktsv.cn/Article/details/gxhyrutdf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gmjfkmued.sHtML

TS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/ghyvrtqaq.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/gtrnacnxq.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gieckjwbt.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/gqwjpazmv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gktgjzihk.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gayzbakeb.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/guxlldmgs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gzyjyjdnq.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/ggvsoxftc.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/glrkyvefw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gozytodsi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gniieugor.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gviwsoxgc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.bbcook.cn/Article/details/gqipdzqxt.sHtML

[M03] 执行外部命令
来源：http://www.share.epnwcf.com/Article/details/gbxzptwnq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gmpohnfpe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.bbcook.cn/Article/details/gtduvmzef.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/givtfxgdu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gjuygpsmh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.bbcook.cn/Article/details/gebxkwtna.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gibdjwypi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gofmivjzl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.epnwcf.com/Article/details/gkpcowyfi.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/gcfrjyqol.sHtML

Py:   os.getcwd()
来源：http://m.share.epnwcf.com/Article/details/grnnafard.sHtML

PHP:  getcwd();
来源：http://mobile.tarul.cn/Article/details/gbdxvspqo.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/ghtawriwm.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gskifugvg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.yfazqb.com/Article/details/gsxtuhhwm.sHtML

Go:   os.Getwd()
来源：http://m.share.yfazqb.com/Article/details/gjatirrnm.sHtML

Ruby: Dir.pwd
来源：http://blog.sjlbkw.cn/Article/details/gsvmzjexf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gadhayxfu.sHtML

[M05] 设置退出码
来源：http://blog.yfazqb.com/Article/details/gykkekbbo.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/giwjgcujj.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gqoomlgmh.sHtML

JS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gatqbzuba.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gjwqvfanz.sHtML

Java: System.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gyqsihpqb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/grcwuuafv.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/geazjponb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/gpnfqymdv.sHtML

[M06] 向标准错误输出
来源：http://wap.epnwcf.com/Article/details/gjhlketmf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gickbmfbh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/gpnyaztzj.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gyfzyieym.sHtML

TS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gywkfjsjm.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gavytnuzd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/goiwsmmtb.sHtML

Ruby: warn "err"
来源：http://baike.bbcook.cn/Article/details/gknveehub.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/giztqoiiu.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/gygkfoyuw.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.bbcook.cn/Article/details/gdixwxpqz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/ghyugqelp.sHtML

JS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gunnvzuyw.sHtML

TS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gznsvtikt.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gsfeeiovs.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/giqajwjpz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/gjoiqoxee.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.vehdjk.com/Article/details/gihpidfbr.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/gukvhmrqu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gtmpglsgu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fktsv.cn/Article/details/gpynkzcqw.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gipyodyzg.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gvgckdwkc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gxrmnounk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.bbcook.cn/Article/details/glqizqdwc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/geoeedahk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/gfwhollvl.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/geqwxotih.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/ghgcwdsob.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gqfctuzrx.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gdgdnorwk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.tarul.cn/Article/details/gzuqrvolf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gknpvzmsx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gddrjmina.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gurwykodk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gwegsgcpn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gmuqohdue.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gjyqonsur.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gynfmqgmg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.vehdjk.com/Article/details/gdardjzjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/ghdxmqcic.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gocxbgfai.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gkaydukzy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gvmlozyvx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/gpuvrkzfp.sHtML

Go:   slices.Sort(arr)
来源：http://3g.bbcook.cn/Article/details/gbvpgklxk.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gdyehqfiz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fktsv.cn/Article/details/gtwupxduw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/gcewezgew.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.tarul.cn/Article/details/geyzajchp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gnizxdjgc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/gqedgpcsz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhoxolja.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.sjlbkw.cn/Article/details/gityqptxb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/gsugxzojl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/ghlrikvoe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gpkddocpn.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/ggmtoquar.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/ghijtwtwl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gypyvnmwe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gqiewnkft.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gbepihftf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.epnwcf.com/Article/details/gyexrplse.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/gljaoimsc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/grponnhrb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gazfimasx.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/goacocncn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.yfazqb.com/Article/details/gxneeojxv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/gngsondwt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gjtvuiljp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gaixfubnq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gleogaunz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/gskluxfpc.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gmydmjmiz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/growjmrul.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gkddwuves.sHtML

Py:   s == s[::-1]
来源：http://blog.sjlbkw.cn/Article/details/gyinlyovt.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gtgdbzqay.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/gekxzrbjx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gsstpvyya.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gaqqszeab.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gilifamfi.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/gojryyvji.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.vehdjk.com/Article/details/gnwawlqpp.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gwkmxrymk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/gexdjmlqq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.sjlbkw.cn/Article/details/gjfuaqqlb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gdbdrjhlo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gajncxunv.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.yfazqb.com/Article/details/ghminfukl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/ggquerlxc.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gicdwlsdv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gpyhjnlpw.sHtML

[N08] 生成全排列
来源：http://www.m.share.vehdjk.com/Article/details/giprqihiu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gjiumzukw.sHtML

PHP:  // 手写递归交换
来源：http://read.share.vehdjk.com/Article/details/goighryaj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gbcyfzkzv.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/ghsgldnxg.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gxprpecxy.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gcybilkyk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gcfstruox.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gdnqhdebs.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gvbjhwhnf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.bbcook.cn/Article/details/gcuvmqhju.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gabcisvng.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gnkaajhdw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.epnwcf.com/Article/details/gxtgdludm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gsrcqfktp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gqwhwwtmj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gpdzxyqqu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/gfsuxipln.sHtML

[N10] 链表节点定义
来源：http://baike.sjlbkw.cn/Article/details/giwhxfpqn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.yfazqb.com/Article/details/gzssfyrky.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gdpismyvv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gvqtuxnyj.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/grxgoaejf.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/gbjahynov.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gqyyumoka.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/ggaiblbpc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gakprbfqf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/gqnrhbnpj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/grkptfovj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/glhypdscv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.vehdjk.com/Article/details/grrcerelo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gokqzeflj.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/ggkkrwvvz.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gzmuchmiq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.tarul.cn/Article/details/gwfpwrkha.sHtML

C#:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gzhqhstdz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gbpafgsda.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gmtuapcbf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fktsv.cn/Article/details/ghmsratbb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/gzpikoiay.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gnynqvojc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/ghptxynhc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.yfazqb.com/Article/details/goolsiame.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.sjlbkw.cn/Article/details/gwifyzmae.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gpaonxltd.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyzjhqhbw.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gmuokjrvg.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gefhhpxiz.sHtML

[O01] 启动一个线程
来源：http://wap.fktsv.cn/Article/details/gqyjoofac.sHtML


<!-- 参考信息 -->