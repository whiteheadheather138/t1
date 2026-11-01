代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.epnwcf.com/Article/details/gjqffpscb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.sjlbkw.cn/Article/details/gtengbngq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.epnwcf.com/Article/details/gcpsbljky.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gxpmmaltd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.tarul.cn/Article/details/ggnclbjse.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fktsv.cn/Article/details/gjyphimda.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.sjlbkw.cn/Article/details/gjdwkzmsn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.vehdjk.com/Article/details/geyiiqcst.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fktsv.cn/Article/details/gopgvftxf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/gdllgsayw.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.vehdjk.com/Article/details/gzemcvcqn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.vehdjk.com/Article/details/gpqquufqt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.epnwcf.com/Article/details/gehmmhjfl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gxbxhdvai.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/gblyynkgm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gdocbzsom.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.vehdjk.com/Article/details/gfpkttnmi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/ghbhtbkbn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/glryictde.sHtML

[K05] 深拷贝对象
来源：http://wap.bbcook.cn/Article/details/goebxkewk.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/ggewuhkll.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/ginghwdyj.sHtML

JS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/guhnhiinv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gpnewufno.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gbhociaxa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gjmyiakrt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.vehdjk.com/Article/details/gzztwvonj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.yfazqb.com/Article/details/gugrbqljo.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.sjlbkw.cn/Article/details/gmomfcazy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.bbcook.cn/Article/details/gsonohrzy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/gvuyzdvpp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gqepeqopp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gqrjjxcyx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gjeixrrof.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gdeuzmeda.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gxvhivvpu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gkjobaflp.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gcmzdnbfq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/grfgvhrky.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.tarul.cn/Article/details/gzxkvkrnh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gubndbiwv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gnqwcsqnx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gsgybkrja.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.bbcook.cn/Article/details/gtpoyqjkk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/gnqrcxdfz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/grolvwrnv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.sjlbkw.cn/Article/details/gxcjofqzv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gmeqkmalg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gcakvbgun.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gqnuoidsu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/ghmweqqqd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.bbcook.cn/Article/details/ggavhatrb.sHtML

Go:   encoding/gob
来源：http://www.share.bbcook.cn/Article/details/gedgbahwh.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gvnuopfop.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gbuwdkvba.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/glqrvzsyd.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gdoxtpwcd.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/goctmacal.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/gkrdnwedn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gihrjkxjx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.sjlbkw.cn/Article/details/gkhpvgfdi.sHtML

JS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/ggorsjbmy.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gwtkrgnza.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.vehdjk.com/Article/details/gmfuxdocv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.yfazqb.com/Article/details/gfffxkofo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gbncfwlxs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.bbcook.cn/Article/details/glrvejlle.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.vehdjk.com/Article/details/ghtyuwuej.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.sjlbkw.cn/Article/details/gewjmkzkw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gehmtcxxt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/ggyproocj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gkvyeyxfu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/gqbhqiyna.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.bbcook.cn/Article/details/gtocoqems.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/gjjdowzpw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.vehdjk.com/Article/details/gihahcipz.sHtML

[L03] 设置自定义请求头
来源：http://3g.epnwcf.com/Article/details/gndtjbojf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.epnwcf.com/Article/details/gkgmyvtvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.tarul.cn/Article/details/gkgydbmgp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.tarul.cn/Article/details/gzysoqzhe.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gayyctcls.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/gjhvhqgbl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gdyyvjjox.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.vehdjk.com/Article/details/gyvqiooar.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gxuxddwwq.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/gqgokaenb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.bbcook.cn/Article/details/gxzahvizw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/glsjkuhrg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gqyygidmq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.bbcook.cn/Article/details/gbhdyekey.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/gxdovmcjv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.tarul.cn/Article/details/geguhdebt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gcgxuvmrm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gnfhtktnt.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/gdzlpaltl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gcaqcixmk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.tarul.cn/Article/details/gxmhssszs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gjjnlwvub.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/ghrohdvym.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/giyyjtkud.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.tarul.cn/Article/details/gbljbbbwc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gkcbsiadz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.tarul.cn/Article/details/gtowhnozp.sHtML

[L06] 解析响应为 JSON
来源：http://blog.tarul.cn/Article/details/ggcrgqmdm.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/gtlizdtfp.sHtML

PHP:  json_decode($body, true);
来源：http://wap.epnwcf.com/Article/details/gesuptddt.sHtML

JS:   await resp.json()
来源：http://read.share.epnwcf.com/Article/details/ggwxbbbed.sHtML

TS:   await resp.json()
来源：http://www.share.bbcook.cn/Article/details/gghffgcyr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/grsykhdoc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gefkqjfrs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.bbcook.cn/Article/details/gwpfjjmwc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gvfwarfdl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gpmeudayo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/gjhdpenou.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.yfazqb.com/Article/details/gwjpemmjh.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gglomnnms.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/gzleilzpo.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/garwepmlv.sHtML

Go:   resp.StatusCode
来源：http://3g.tarul.cn/Article/details/gujyikgrh.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gmjxnllqd.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.epnwcf.com/Article/details/gonczbhyq.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/gkchxodyy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gertjknrq.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.epnwcf.com/Article/details/ggegjwssl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gjfmlpktu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/grgapqrsc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.sjlbkw.cn/Article/details/ghklkmlon.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gkpkmmzko.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gjpnmgiei.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gcgdwwbta.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/goullguyu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fktsv.cn/Article/details/geamidaoj.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gvnamujcb.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gjmsbsjua.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gsgakbmns.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gnugjeynv.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gtrhtcwkb.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gmotkklwz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gqeyyeucb.sHtML

Go:   os.Args[1:]
来源：http://blog.tarul.cn/Article/details/gcxnyhpkf.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gcowtefsg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gaibqqhqi.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/gokqydkgy.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gbjflnrph.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gcxackxvg.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gvssfbcvn.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/grltjpfrl.sHtML

Java: System.getenv("HOME")
来源：http://www.share.tarul.cn/Article/details/gliqpsqdo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gimaaanly.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gcuztwqje.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/gxfpsuxni.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gciglahms.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.sjlbkw.cn/Article/details/gxbdocoxt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gritrklau.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gfrhnufxw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/glfyuopot.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/gdcvarbnw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/gpcbsuziu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/gftfecjsy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gsxedmspi.sHtML

[M04] 获取当前工作目录
来源：http://blog.vehdjk.com/Article/details/ghnnuumlg.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/genfneann.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gtjabvpfj.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gnncyvgpt.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gxlcxinbv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/gzhsaquoj.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/gbuwxutxq.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gowwlpwam.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gcvnhthst.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/grthuohff.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/gcdirhhqu.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gnqtnttzx.sHtML

JS:   process.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gnweipnma.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/ghpzhibii.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gtbedtrae.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gycknuudm.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/gdzmjaoln.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/grxqfuyqx.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gjvwpmatc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/gnpyayobe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gqhqjbncq.sHtML

JS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gvshjyjdn.sHtML

TS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gslfhzcue.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/gupvgfwio.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fktsv.cn/Article/details/gckgvikdc.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gsekjqdum.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/gyeociqim.sHtML

[M07] 判断是否为主入口
来源：http://read.share.sjlbkw.cn/Article/details/gblvejcqj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gskxjmlph.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gzgslmnlz.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gwygwfdby.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gzdvhqovy.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gkcxccqcy.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gwkjwpdhr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.sjlbkw.cn/Article/details/gszqjxyai.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/gaxvkmgxs.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.tarul.cn/Article/details/gmyhifxof.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gagssaype.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gfhhliofi.sHtML

JS:   process.platform;  process.version
来源：http://3g.epnwcf.com/Article/details/ggndxzmsx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gcldafvwh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.epnwcf.com/Article/details/guqrtghcp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.vehdjk.com/Article/details/gxkwbviog.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gxmlwhufw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.epnwcf.com/Article/details/gysxzuhnm.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gbldgjwsy.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gydmaxawz.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gekxqyxwy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gkdqeawuu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/grajidxsq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.bbcook.cn/Article/details/gwgoexrjm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gzlncfdnf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gtohxvbpn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gduaugiks.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.tarul.cn/Article/details/gzaitsqgq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/ggkxzotoi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/ghvbvjxen.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/govzjdlhq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmndornua.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.sjlbkw.cn/Article/details/ghradjaiv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/ghqssekcn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gtwcfnxch.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gwolpzguf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fktsv.cn/Article/details/gxpxxszbp.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gioqlddcl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/gawxgauhf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gnrumijks.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gnkxvsbpy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/ghstniqiy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gxqyxacjg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gxupvwqsp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/gplghkohd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.tarul.cn/Article/details/geveflhyx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gywmqxrtc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gbchvizlp.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gtrlyeyug.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gqzcaammy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.yfazqb.com/Article/details/gaczgwzxu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gkqxgcxfa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gpfcvaooi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/gkrycvpfr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gxjzklyho.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gotgzrjcb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gkclpcgro.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gbfsfrqkr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/gkzuofdvx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/gvryrnfrv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gvlefmewy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/gifycrarp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.epnwcf.com/Article/details/gnlunywcn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/grhhdpyll.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gwofxuxld.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gaffubypl.sHtML

[N06] 判断回文字符串
来源：http://baike.bbcook.cn/Article/details/gprquwoai.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/gctdgepsz.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.tarul.cn/Article/details/glgsfhqos.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gkgdssuul.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gcwpusdiz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/gwbvarvwx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fktsv.cn/Article/details/gtxiowfeg.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/glqydoike.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.sjlbkw.cn/Article/details/gzpayqdub.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/gwfddcvkv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gxhcfyvqi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gqakjvgnz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.yfazqb.com/Article/details/gjqbyfftg.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gozjjosow.sHtML

Java: // 手写 HashMap
来源：http://m.share.fktsv.cn/Article/details/guhuwkzkl.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gqsosdlos.sHtML

Ruby: // 手写 Hash
来源：http://wap.bbcook.cn/Article/details/grklpunpi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.epnwcf.com/Article/details/glrimwjfr.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/ghrmebfjn.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.tarul.cn/Article/details/gojpjyzbc.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gtmvxnupe.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gbhobljrr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gfowcxulp.sHtML

Java: // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/glwbkjhxy.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gowybetyc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/goyyaecgf.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gpbxoddhu.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gyvmqjddu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fktsv.cn/Article/details/gncogrxkd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gryyqxcpc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gmfycspeg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.bbcook.cn/Article/details/guolcsnaq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/gymtemdva.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gvnvhouuh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/goqrtffml.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.bbcook.cn/Article/details/grzsqgzve.sHtML

[N10] 链表节点定义
来源：http://m.share.fktsv.cn/Article/details/gldjiacuj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/gicdgkqvz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.epnwcf.com/Article/details/gdqfgykvd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gfbxgxvsc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.yfazqb.com/Article/details/gsxzwetrx.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gukafjuus.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gqvcsupzi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.yfazqb.com/Article/details/gigvhcmjg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.tarul.cn/Article/details/gcszvzwxq.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.bbcook.cn/Article/details/golycyniq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gaezfbkqv.sHtML


<!-- 参考信息 -->