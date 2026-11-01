代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://read.share.vehdjk.com/Article/details/gucujeffv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.sjlbkw.cn/Article/details/gqbptdyon.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gbtcxhdim.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/gapmhtywy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.epnwcf.com/Article/details/giicjmmmw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.yfazqb.com/Article/details/gkrihyzts.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.yfazqb.com/Article/details/gnvaxwnna.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/gkqejzvss.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gysviadwa.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/gcgafytyz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fktsv.cn/Article/details/grbsdacts.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gdezxdfzl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/gvproonie.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fktsv.cn/Article/details/gabupwvyd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/gwoofbfwx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/glshqfrmn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gqtvaoutb.sHtML

[K07] 进制转换
来源：http://www.share.fktsv.cn/Article/details/gccoxpkyh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gcjcinwuf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gkmsexoyf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gjmjjpwxh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gvvowvunp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/ghzyskzoz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/gdnhcsaay.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.bbcook.cn/Article/details/gnwoceder.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/grptobesq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.tarul.cn/Article/details/gzhlourev.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gchhjceal.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/gtbqpxgqp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gkdnwcmhk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.bbcook.cn/Article/details/ggjhnphji.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.vehdjk.com/Article/details/gfpgwcixy.sHtML

Go:   encoding/gob
来源：http://m.share.tarul.cn/Article/details/goyuygxrf.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/gglblktuh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/grjkjokoy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guobzgwid.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/geqcnpjpx.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gqcxxnvoc.sHtML

[L01] 发送 GET 请求
来源：http://3g.vehdjk.com/Article/details/gcfhjrapf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gvxukltxj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fktsv.cn/Article/details/gfrelajjy.sHtML

JS:   await fetch(url)
来源：http://3g.sjlbkw.cn/Article/details/grdavtzpm.sHtML

TS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gnvpuiqrm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gkxydxpjo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.yfazqb.com/Article/details/gwsqsyfyp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.sjlbkw.cn/Article/details/glxgfpsbr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.vehdjk.com/Article/details/gkbstpmni.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/glsgdshzu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.tarul.cn/Article/details/gwdjtgknd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.bbcook.cn/Article/details/gwtjzbhae.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gqmchotck.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/gxwwaaxdr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/goeytvepd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gvgtsjydr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.vehdjk.com/Article/details/gfxjzlbci.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gciltgsdl.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gjuofznyr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/gfzcebfsw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.bbcook.cn/Article/details/gkffrxkaa.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gcgwtnene.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gkmddujaj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gqzvgqqdh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/grwkrknog.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.epnwcf.com/Article/details/gstuiwujm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/goyadtnat.sHtML

[L04] 设置超时
来源：http://blog.sjlbkw.cn/Article/details/gvqnnmoet.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.yfazqb.com/Article/details/gbhwuabje.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/gymgzdkax.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/ggojzjkuk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gjnencczf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.vehdjk.com/Article/details/geyqasovc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.sjlbkw.cn/Article/details/gedptxyik.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/ghiaxnyzo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gqvfyzpac.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.tarul.cn/Article/details/grdnwafvu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.tarul.cn/Article/details/gpfnpaubr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/gmcavdjne.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/gfljmkdsi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gfloblcvq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gvbvghjnt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.sjlbkw.cn/Article/details/gssavbyxa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.bbcook.cn/Article/details/geeyflqto.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gjianpdkm.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.vehdjk.com/Article/details/gczudkbwp.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfthcaswc.sHtML

PHP:  json_decode($body, true);
来源：http://blog.tarul.cn/Article/details/gnehcmbzl.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/goorlhuny.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gpmaesbkn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/gofhwzujo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/gemgqltdl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.epnwcf.com/Article/details/gjkpbgghc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fktsv.cn/Article/details/gezalnzln.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/gprqqcdrq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/gufidzuou.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsjeatgf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/gxjyykbfa.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/ggzcitdjl.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gjtdlhrob.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gampkkpxe.sHtML

Ruby: resp.code.to_i
来源：http://blog.bbcook.cn/Article/details/gfrwnxmdf.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gjbtezhfk.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fktsv.cn/Article/details/gyhijwyxf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/glzewodfd.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.yfazqb.com/Article/details/gevnvjzgo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/ghqqkwpts.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gnsapssfc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.sjlbkw.cn/Article/details/gqtjrarza.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/gbomcuykv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fktsv.cn/Article/details/gehnhtjik.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/gsatuwbti.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzrvhctmu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.yfazqb.com/Article/details/gtasmavem.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gsxtrppiy.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/gqulqiucv.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gmnelwbtr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gubkmdgsg.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gmocwccoy.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gritohiir.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/ghxddbvcv.sHtML

Go:   os.Args[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gwbbvcoyt.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/gzpqifgws.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gppqwhcbw.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/gntespvkt.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.bbcook.cn/Article/details/gmcypqbqv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gafefetdl.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/ghexoiqct.sHtML

TS:   process.env.HOME
来源：http://mobile.bbcook.cn/Article/details/gpwecicka.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gxsqzsrxu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gmhozvmpc.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gnaekwrtx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gymkuhehl.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gzmeptslt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gdohdbdfr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gmdgcwhcp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gdfwkhkvz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gqxlswnxr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.yfazqb.com/Article/details/gicsjrwzq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gopoenvei.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gljwwcxuh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gfcdjylxq.sHtML

[M04] 获取当前工作目录
来源：http://3g.bbcook.cn/Article/details/gubtgpypu.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/gdghotkyz.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/getnsbecn.sHtML

JS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gaqnwjdqd.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gehhxlfxh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.vehdjk.com/Article/details/genwomiis.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gfhoqxkvm.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gfzavyuch.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.tarul.cn/Article/details/gwhdavkvk.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gospdzste.sHtML

Py:   sys.exit(1)
来源：http://blog.tarul.cn/Article/details/gmffqyxww.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gmueqsbir.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gydklmtjx.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/grfkhwmff.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gbajmjygt.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gbcxihqge.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/ggwgjcdtr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.bbcook.cn/Article/details/goxziyzyr.sHtML

[M06] 向标准错误输出
来源：http://3g.epnwcf.com/Article/details/gxplyryxj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/guqcqheec.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fktsv.cn/Article/details/gkxauqdix.sHtML

JS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gqbifcgtt.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gnnoqcjsx.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gissgyrfj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.vehdjk.com/Article/details/gbqsdcnxp.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gxefjqswf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/glhvxiptc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fktsv.cn/Article/details/gixumpniq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.epnwcf.com/Article/details/ggjfypavi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gqvnjytos.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gqsgyfono.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gjecbiulj.sHtML

Java: public static void main(String[] args)
来源：http://wap.epnwcf.com/Article/details/gchgyomav.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gjzigwtjo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.tarul.cn/Article/details/gwcabikrs.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/geyzrojyj.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/geidphcgq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.epnwcf.com/Article/details/gthzzbqfu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.bbcook.cn/Article/details/gsolzioln.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gmrrmhzbv.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gpkegqmqv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gkbwivbwg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/gsbqmuasu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fktsv.cn/Article/details/gbzudbrin.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fktsv.cn/Article/details/gmpyrrlwy.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gqyqvvlpq.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/gvcslrfxw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gcldmgswf.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gzbgeoewx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gspjionoc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gxctyirqy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gmhqgyppx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gcbtgskgn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gvrwnqare.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gbbcwygtr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.bbcook.cn/Article/details/gfnohuayh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/ghfaesefv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.vehdjk.com/Article/details/gnbuukjri.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gdjzmdgmf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.epnwcf.com/Article/details/ghiidmzos.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gufkedbzj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gejrufyyj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/gvusllpqy.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gifaxpxem.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gkaupwgul.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.vehdjk.com/Article/details/gyfdbaanj.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gmrzrevfk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fktsv.cn/Article/details/gsiicgxur.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/gfykwpvqf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gcekgprzv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gdtyldnqs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gvyblackg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.bbcook.cn/Article/details/ghxbfvipe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.yfazqb.com/Article/details/gqiyzuucb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gigwzkvvf.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gkleaquap.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gqybucamp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/gqirtcbih.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gobxbsyvr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gwtmbfemg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gssdcxdxq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gxgcdyqxj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gqrjqxwrr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gghgsdlkz.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/gqzgqvicd.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/gibfohawa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gcpefemom.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gtubwnpzj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gamlwywge.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/ghyggxkoh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fktsv.cn/Article/details/glgyhoqju.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gjshvhaec.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.tarul.cn/Article/details/gadnwxsml.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/gklqaopum.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gphjngdxn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.tarul.cn/Article/details/grwtzsqma.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gzommbjxh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gikpucwul.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.epnwcf.com/Article/details/gkfjjxjvg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gnhzejgjy.sHtML

Ruby: s == s.reverse
来源：http://baike.bbcook.cn/Article/details/gwmmkjfkw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/grdnwroke.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gotcmnnpv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gvxmfmilu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/goyevwfos.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gidnqzbtx.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/guuwpujfd.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/ggytlcyao.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gzxfgcdxy.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gximrhaot.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.vehdjk.com/Article/details/gzmeuybnq.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/grtrddiwx.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/goemdsybh.sHtML

PHP:  // 手写递归交换
来源：http://blog.vehdjk.com/Article/details/gqfhaozjc.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/geldbasvk.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gijjnmhru.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gzkqajcvd.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gizkrupsj.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gmnmjftfl.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gwqsdivfq.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gcuvgjrin.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/gtlpdxruz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gadjudbrl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gtcontvqm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/gvdwmywbt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.epnwcf.com/Article/details/gktdvrwgm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.tarul.cn/Article/details/gkzyuexqa.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gzbgtzjcm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gmrqywyob.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/gzwdpkuzu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/gquekfdky.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.sjlbkw.cn/Article/details/genusbezh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/gfurocbaf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.sjlbkw.cn/Article/details/gcygpdyum.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/graelgqyn.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.sjlbkw.cn/Article/details/grajfrnrb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fktsv.cn/Article/details/gimpvqzmt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.epnwcf.com/Article/details/gpncrlqnp.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gaodtococ.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.tarul.cn/Article/details/gganzunlw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gkhlxzhaw.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gkimxsjsh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.vehdjk.com/Article/details/guuawffcd.sHtML

Java: // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gujhansrj.sHtML

Go:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gcspetknj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.vehdjk.com/Article/details/guugzormf.sHtML

C#:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gzsneiady.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.vehdjk.com/Article/details/gnwfeqgun.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.vehdjk.com/Article/details/gmltmxrji.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/gbdwdtqoa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.vehdjk.com/Article/details/gywdtttsf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gankhujqx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/ghsepnaui.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gqoynteca.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.vehdjk.com/Article/details/gtknotbac.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fktsv.cn/Article/details/glvjxxjal.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gwzoislgz.sHtML

O. 并发与异步
来源：http://www.blog.tarul.cn/Article/details/gdbwhovkx.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gdcsxjozo.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/gqznsytfb.sHtML


<!-- 参考信息 -->