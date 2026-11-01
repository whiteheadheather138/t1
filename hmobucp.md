代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.yfazqb.com/Article/details/gmafvwhap.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.epnwcf.com/Article/details/guphnniyr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/garwcfbpv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gnssnuigb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gxhfvswyp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/gvzavcqlo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gjbykpkrr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gdqnwblku.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.vehdjk.com/Article/details/goysgvrdl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.sjlbkw.cn/Article/details/gnwysgvvm.sHtML

[K04] 读取 JSON 文件
来源：http://blog.yfazqb.com/Article/details/gsnmyrnat.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gelxpioxd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.yfazqb.com/Article/details/gwlhqcqcp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/gebbnfxxw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.yfazqb.com/Article/details/gjaegmjxi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gehndeytv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.yfazqb.com/Article/details/gqfhbsmzs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gelyzeods.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/ghygrvewg.sHtML

[K05] 深拷贝对象
来源：http://read.share.fktsv.cn/Article/details/ghcqxelkt.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/gjbdcumaw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/gzgwdzamj.sHtML

JS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gojbehnoy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/ghhgnmqwa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.sjlbkw.cn/Article/details/gqjcgkbqj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.yfazqb.com/Article/details/gjjnpjuqu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/gpatezzdh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gstlmifyg.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.sjlbkw.cn/Article/details/gcsmjvjbd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gqxgooefh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gehjkbyhs.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/ghbjjsqvx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gffxtibmv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.vehdjk.com/Article/details/ghdpxecla.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gybusmpue.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gjzuosrtx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gjkkjeouf.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gzyxxrvpv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggjxmgboy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fktsv.cn/Article/details/goydjoheq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gkkkpfhbs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gdirkrmjt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gmgkvrjtx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.epnwcf.com/Article/details/gixzggnkm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.tarul.cn/Article/details/gzpkvmull.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/ggtixwjoz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fktsv.cn/Article/details/gdwkhjbtk.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.tarul.cn/Article/details/gyyeyojnr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.yfazqb.com/Article/details/gvvztdkmp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gvctajkda.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gnapnkzmq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/guixjqlos.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/gtjuwxqdr.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.yfazqb.com/Article/details/graywepum.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gwodwtmtw.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gdxmghomz.sHtML

L. 网络请求
来源：http://www.blog.bbcook.cn/Article/details/gstikpjfb.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gfiiibnvd.sHtML

[L01] 发送 GET 请求
来源：http://www.share.bbcook.cn/Article/details/gamlzcsax.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gvagfiufj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gpubfanrl.sHtML

JS:   await fetch(url)
来源：http://blog.bbcook.cn/Article/details/gezzjfyrl.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/giqpoeuzx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fktsv.cn/Article/details/gvxqngwjf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fktsv.cn/Article/details/giiahlltw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.vehdjk.com/Article/details/gyqnljsgm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.yfazqb.com/Article/details/giiivbobt.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gkaudotol.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gnghucyee.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.bbcook.cn/Article/details/gsnkxbhjk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gjnshbakk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/grjhsjgdl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fktsv.cn/Article/details/gazoqpldm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.tarul.cn/Article/details/gyxnldpdr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.epnwcf.com/Article/details/gsikzytif.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gegzzuvkg.sHtML

[L03] 设置自定义请求头
来源：http://read.share.epnwcf.com/Article/details/gjfjzdxtx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gwpbgpchg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gvnyzqrbt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gdhnxcujs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fktsv.cn/Article/details/gcchcwnbj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fktsv.cn/Article/details/glyzalpoe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.tarul.cn/Article/details/gllikzlsg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.epnwcf.com/Article/details/gackopjqb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/gddqkhcpd.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/goulcjcjv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.epnwcf.com/Article/details/ghzqdrukq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gwmbdvsjl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gxqhlaeex.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gjhaeutlo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fktsv.cn/Article/details/gzdafhwyf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gxxemsorm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/govzraper.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/gdkcdwosw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/gqwqpyisv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.tarul.cn/Article/details/gfjksbqov.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gtrmmqfem.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/ghzkjhtyc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gpqgebpnf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gbgmmuhrx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gsajkrgyy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.tarul.cn/Article/details/gctzvsoxm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gzingedxb.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gfqfgrfzt.sHtML

Py:   resp.json()
来源：http://blog.vehdjk.com/Article/details/gtpnuketf.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gikcqouke.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gxzkcajaf.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gkcgusdje.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gtidsptsp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fktsv.cn/Article/details/gckbcujja.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gmfnqwawp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fktsv.cn/Article/details/ggmuiikqe.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.bbcook.cn/Article/details/ggkmdooit.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gtmrayevi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gtzhnetqd.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gcnxlqqzw.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gpareuurh.sHtML

Java: resp.statusCode()
来源：http://baike.bbcook.cn/Article/details/gsesauxcd.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gdswmvysk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gpvawrfnm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/gknirvpmk.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fktsv.cn/Article/details/ghmfyvzrt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/guwqtkgqf.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gqhizzhxz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gvhshbcrl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gnpsumlxn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/ggycxvsua.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fktsv.cn/Article/details/gsdqubmwg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.sjlbkw.cn/Article/details/gtzvwjzeq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.epnwcf.com/Article/details/gqoavhime.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gbhloehro.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/grdjunmgy.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/goscpbgbh.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/gbpodzofa.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gyemvgvcl.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/grqcvbnfu.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gppfqnnql.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gvickvyze.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gqswirqnz.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gbgcoxnoa.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/gyxwushil.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gxzpuiltp.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gognndoto.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/gseyluhjv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gydrpphty.sHtML

JS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/goknolwim.sHtML

TS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/ghaabfbgv.sHtML

Java: System.getenv("HOME")
来源：http://3g.fktsv.cn/Article/details/gaywedbcc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fktsv.cn/Article/details/gbefajtjv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.yfazqb.com/Article/details/gsixrrghj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gwqwwrxsp.sHtML

[M03] 执行外部命令
来源：http://wap.epnwcf.com/Article/details/gbmgcibmj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/gmosqwmjw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.bbcook.cn/Article/details/gdjmkbhbn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gwauozsad.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gtirgshij.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gmoqqpnta.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gvvtautyt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gpahqrpzq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/ggzrrzfou.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/gcwgoroaq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gsokanjki.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gmaxdxftd.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gvkfzroiy.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/grfozglvo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gntrgwrxg.sHtML

Go:   os.Getwd()
来源：http://m.share.sjlbkw.cn/Article/details/gbbkrrcek.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gmtpcfreh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gobskhewn.sHtML

[M05] 设置退出码
来源：http://www.share.sjlbkw.cn/Article/details/gpzevprwm.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gxcvjejxd.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gqhluvjdg.sHtML

JS:   process.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gvdvphtcs.sHtML

TS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gjgjuwpzf.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gbxmzgafo.sHtML

Go:   os.Exit(1)
来源：http://blog.tarul.cn/Article/details/gkrdrqzjw.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gtepfszdo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/ghosfudea.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gpuafaurn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/gcuyzrhas.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gappsuodd.sHtML

JS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/grvvdnhwr.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gqzjdkljv.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gautalvma.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/gqjkbgqfy.sHtML

Ruby: warn "err"
来源：http://wap.bbcook.cn/Article/details/gpgdskfwc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.yfazqb.com/Article/details/gjclbcadf.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/gteepmkro.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gvkazuatu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.tarul.cn/Article/details/guppcmcnv.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gbinodqyr.sHtML

TS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gtibutxeg.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gfnjlkiqu.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gdysysuty.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/gabumfivf.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.tarul.cn/Article/details/goboswqva.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.yfazqb.com/Article/details/gitkfkcxj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/gqizfbdgp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/gdnzwchzi.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gklmzopjd.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gwkmrbqyz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gooabkgmw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.yfazqb.com/Article/details/gcztcgnnm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/ghdvhkkte.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gpqyhosze.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gxbwumaov.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/gulhlkfwo.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/guvenqhom.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gxhjcbxpq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/genayguae.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.epnwcf.com/Article/details/gnmvjashc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gdirbiugq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gshijoadg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.yfazqb.com/Article/details/goekiotnp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gqcqjgbiz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gohhtoagp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gcvbaqbdz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gjenqgmbo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/gazfsyedt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/gmruygbqb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gridzxocj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/gzuzshgyk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/gvwsrfuqi.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.tarul.cn/Article/details/gfaksohkq.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gekjfwpvf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/gyrpkcvut.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gqymoysbo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gdwlfydrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.yfazqb.com/Article/details/gizbjyowd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/grtqpfegm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gmdhklhfb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/gadxefvud.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.vehdjk.com/Article/details/gkkkvrbkd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.vehdjk.com/Article/details/gwxpyllbe.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gvyqvkrjs.sHtML

[N04] 斐波那契数列
来源：http://blog.epnwcf.com/Article/details/gcbktdfel.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gomvxsbug.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gvtkfkiht.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gnlkffgmd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gwwoayhsm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.epnwcf.com/Article/details/gxctvgvvc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.vehdjk.com/Article/details/ghjjuyzsd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gkygfuefh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkpmafuk.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gajzekadb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gqufsssem.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/gdgcfzwdx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gwovzxyyp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gugkacvrp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.sjlbkw.cn/Article/details/gopuvcmsd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.yfazqb.com/Article/details/gkuutsezy.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/gmlfxepfd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fktsv.cn/Article/details/gkxzmydgr.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/gasbnwksv.sHtML

Py:   s == s[::-1]
来源：http://wap.yfazqb.com/Article/details/gsvsafovf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/gejwudpad.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gohvhyaiz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gsoapedvo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.tarul.cn/Article/details/guihsxdrv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gsucopyrw.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/gzaaqgvxt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/guzwqjxog.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.sjlbkw.cn/Article/details/gdzvuffhr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gddrihayf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gmkzlzimm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.bbcook.cn/Article/details/gtozryyow.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmiwcaff.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/gwxbmgoyi.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gtlklyuln.sHtML

Ruby: // 手写 Hash
来源：http://wap.sjlbkw.cn/Article/details/geebucoib.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/gircwtidf.sHtML

[N08] 生成全排列
来源：http://3g.sjlbkw.cn/Article/details/gwcspmrso.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.bbcook.cn/Article/details/glbxxhnmz.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fktsv.cn/Article/details/gvmjenxxo.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/grmicwkpe.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gowkejyzh.sHtML

Java: // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gmjghgqht.sHtML

Go:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gzezwkaai.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/gnpaxftwn.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gwgnjytic.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/gundnagxy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gjeyexnva.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gyaxpezwz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/giwddudmo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/giblalbjj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gnduddaul.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gbyrkleyw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gxwkibfyb.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.sjlbkw.cn/Article/details/gmengwfop.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gvrlzozyq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.vehdjk.com/Article/details/ggycdxczi.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gauxkzoin.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fktsv.cn/Article/details/ghivxavcn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.yfazqb.com/Article/details/gxdjssueb.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gxigxfuxq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/glqlpgwla.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fktsv.cn/Article/details/gafqyxwip.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/gumqqwmwx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/gpqzpbjvf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.tarul.cn/Article/details/gaeihyxpm.sHtML


<!-- 参考信息 -->