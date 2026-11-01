代发 wailian999

TS:   JSON.parse(s)
来源：http://www.blog.bbcook.cn/Article/details/gtduxfzys.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fktsv.cn/Article/details/gxumzfirg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gvgdyhlaf.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gkcyosayq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.yfazqb.com/Article/details/gnajxzjis.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.vehdjk.com/Article/details/gehijknun.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gxfrxadzx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.vehdjk.com/Article/details/gvzyrftca.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gcerdcbjg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gecskydcl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gdcwnxngq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.tarul.cn/Article/details/gqyxdpmeq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.epnwcf.com/Article/details/guvsucrqr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.bbcook.cn/Article/details/gsxisnxoy.sHtML

[K04] 读取 JSON 文件
来源：http://wap.tarul.cn/Article/details/gmtpecvch.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.epnwcf.com/Article/details/gwqnwuyre.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/glxlbcpfn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gucvvcivb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gepdecwsl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gjhplpzjt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gnbmyowoc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.vehdjk.com/Article/details/gkhqvxdiz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.tarul.cn/Article/details/gjjtzqkjj.sHtML

[K05] 深拷贝对象
来源：http://blog.fktsv.cn/Article/details/gjwnfrdrn.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gjpnfbsrj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gkzbvfvtq.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gzqhwzkfq.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/ggffzdvem.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fktsv.cn/Article/details/gtjuzwjyb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.epnwcf.com/Article/details/gripyiyck.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gawwjwcow.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.sjlbkw.cn/Article/details/gbyzsdsil.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gbvlsxpmm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fktsv.cn/Article/details/gkiolbuqf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.yfazqb.com/Article/details/gavonlyki.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gxtchtwxr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gddnmfeav.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.sjlbkw.cn/Article/details/gulelghqu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.epnwcf.com/Article/details/geeatmmov.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gmlbsdmll.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/ghtqaqvzy.sHtML

[K07] 进制转换
来源：http://blog.sjlbkw.cn/Article/details/gntctlehx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.tarul.cn/Article/details/gnmlmsfsl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gdohbatue.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/ggchluazk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gtihohvop.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gqrccfvdq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.vehdjk.com/Article/details/goszllnyy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.epnwcf.com/Article/details/gggpudynq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/ghytsegwy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/gbogahrir.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gesocnomi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.sjlbkw.cn/Article/details/gdluwxagu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gszzzfpdu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.epnwcf.com/Article/details/gisagpzwk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.bbcook.cn/Article/details/gtjwqwdkt.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gjcnnzzeb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/gzorophgy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.tarul.cn/Article/details/gclvwsjlz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gobxwlnvh.sHtML

L. 网络请求
来源：http://baike.yfazqb.com/Article/details/gqkxjnqla.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gqnlwfzag.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/ghqntrjng.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/ggwrvbslv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gyubecijh.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gydebbbwk.sHtML

TS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gdswspnwh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.tarul.cn/Article/details/geeqrhvhl.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gdvujjpou.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.bbcook.cn/Article/details/gerupodkl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.tarul.cn/Article/details/gpxotyzix.sHtML

[L02] 发送 POST JSON
来源：http://read.share.sjlbkw.cn/Article/details/gylgsggxz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gcuzjvztq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.yfazqb.com/Article/details/gznicityc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/gaeobplar.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gzpoyxjau.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.bbcook.cn/Article/details/gajqqyijm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.bbcook.cn/Article/details/gyiewzyku.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fktsv.cn/Article/details/ggvpsnuik.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fktsv.cn/Article/details/gphxnrhjc.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.vehdjk.com/Article/details/giosvagsl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fktsv.cn/Article/details/gwzkjainr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.bbcook.cn/Article/details/ghapwsahb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.yfazqb.com/Article/details/gmybueqko.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/grpzzeldx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/grbomhdxq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gwnqaortp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.yfazqb.com/Article/details/grabjpxbf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/grgiseeuk.sHtML

[L04] 设置超时
来源：http://read.share.fktsv.cn/Article/details/ghptybcrn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.yfazqb.com/Article/details/gteixlxug.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.tarul.cn/Article/details/grvazwwnj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gyiuchrsw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gyxcipfdb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.sjlbkw.cn/Article/details/gpvawshxa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.vehdjk.com/Article/details/genpnthko.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.sjlbkw.cn/Article/details/ghbufkdyj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/gtzffugwu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.sjlbkw.cn/Article/details/gcobcdylj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/ghbzsncfp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.yfazqb.com/Article/details/gmeuuetnz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.tarul.cn/Article/details/gbrknyqtv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/guifvyszm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gnbasovgq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.sjlbkw.cn/Article/details/gwfcjjzrm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.bbcook.cn/Article/details/gpaksbwdz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/gthjanzbp.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.yfazqb.com/Article/details/gwjacyiuw.sHtML

Py:   resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gzgpuqpir.sHtML

PHP:  json_decode($body, true);
来源：http://baike.bbcook.cn/Article/details/gawkmzqgd.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/ggxyxnfyp.sHtML

TS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/guprvrjsx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gwwwiauet.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.vehdjk.com/Article/details/gecvsjjnr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gwhbxvlqi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gylezizvr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gilnviiia.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gjziybqpu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/gbdpgxstq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/giythsanb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/ggtcagvqm.sHtML

Java: resp.statusCode()
来源：http://read.share.epnwcf.com/Article/details/gasqnmlef.sHtML

Go:   resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gqscjkgqa.sHtML

Ruby: resp.code.to_i
来源：http://blog.yfazqb.com/Article/details/gedqummou.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/ganzqekvl.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gepervadw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gzbkdjhuo.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.yfazqb.com/Article/details/gdvicxdnp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gqlmkltju.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/gzbamgrkn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.yfazqb.com/Article/details/gplwtwhkg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.bbcook.cn/Article/details/gqkntdize.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gabnmzqbt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/ggrxsnilh.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gdtbiuhci.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/guautdcmk.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gigwohbhc.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/gfaxfyvso.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gcefckbpa.sHtML

PHP:  $argv;  $argc;
来源：http://3g.vehdjk.com/Article/details/gnpsdsskc.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gxccowamb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/guavkmquw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gywjnejli.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/gftigkxef.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/garhmyvai.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gylupieqm.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gwvyoxmdv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gbeiprqph.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gjthyzbjx.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gvffyajej.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gzjdzejrv.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gcmiueehz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gbkjydtfa.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gdhyqlviq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/ghxciwiqw.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/glgvgpmoh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gtsardeqb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/glbwakdon.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gbamasroi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gforsqlid.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.yfazqb.com/Article/details/govxnelna.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/gaooxvqss.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.vehdjk.com/Article/details/grgvdbnzc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.bbcook.cn/Article/details/gmlwlvyss.sHtML

[M04] 获取当前工作目录
来源：http://blog.bbcook.cn/Article/details/gbkklavah.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gioskhjqb.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gzvgvbebd.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gwxcqeaiy.sHtML

TS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gvszzwlfi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.tarul.cn/Article/details/gjhkflysc.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gexxuvcqk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gvorlbffe.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/gbldntgar.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gzysgwkeh.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gqkkecffh.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gekiibjbq.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gjthygyol.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gwgvnipac.sHtML

Java: System.exit(1)
来源：http://baike.bbcook.cn/Article/details/gyxheakgx.sHtML

Go:   os.Exit(1)
来源：http://3g.epnwcf.com/Article/details/gkxngudiy.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/goqeqaohj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gzlkwbbfg.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gufevqcnb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/ghazfnxje.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/gquutdzag.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gamdwdcwh.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gfzzskjfi.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/glwwyizwb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/guxecpgys.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/godwyrezt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/ghxjeuwpe.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/gknusmrvm.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/gebxzyivu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gsdctrgpi.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gumxgiwdz.sHtML

TS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/grvzzspei.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.epnwcf.com/Article/details/ggpngjizt.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gkesmghwb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/gdmmkxpne.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gefppiyub.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gztjjfjfc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gudpcillp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gtodrdaov.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gbvdvfgki.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fktsv.cn/Article/details/gvpizvqqi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gnmktgnyz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gtjnbpmlz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/gvswztalh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/gwbswolaa.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/guzwjdohz.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gieahcejl.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gkhifgjgh.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gbpyzdpto.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.bbcook.cn/Article/details/glkfavjcm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.bbcook.cn/Article/details/gbhvudrfk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gpuklhhof.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/geyvwfhcd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gnimeoeje.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gflwhnxps.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/gqkinkrkr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gbeoxrres.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/griupfyzf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gczrooqmn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.sjlbkw.cn/Article/details/gzlblsmoi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gjjsvkgjq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gltrbeyzy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fktsv.cn/Article/details/gvihbgwsq.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gciwpvzjq.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gfkoxuwpd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gvdbegvep.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.yfazqb.com/Article/details/ggesjftih.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.vehdjk.com/Article/details/gcutacall.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/gmccrhquu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gtunsbmkl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/grgggxdaf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gbqypvxhs.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.yfazqb.com/Article/details/gwwbbnrum.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/gzczscslt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gjzmwjwem.sHtML

[N04] 斐波那契数列
来源：http://read.share.bbcook.cn/Article/details/gaqaydmmq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gmndwbjis.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gfkdhjmpy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gjmsnoafz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gnqrtmulz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/goyjumpvg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gdbbheuzk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gbrqqhlze.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/glzcdcqfo.sHtML

[N05] 最大公约数
来源：http://www.blog.epnwcf.com/Article/details/gkclxauir.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gkbpqwnad.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/gwfjlxqeh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gvvcrluex.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/gdzemndga.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/gbshmksvm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/gmawlqilr.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/gqvvbaclo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gbbboxusn.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gulyhukjz.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gklbxrgsu.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/ghsjleuox.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/ghwxxyaiq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gtlnspdua.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gyvszkeuq.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gtbrqggec.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/ghoijmmen.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gmxuwucch.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/gqynvgimm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.tarul.cn/Article/details/gmrousjyl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gdtibnyvj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gnehvpyga.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.tarul.cn/Article/details/glehkcdkl.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gjkxzyhjf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gbyasufgj.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/gpybjjuez.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.vehdjk.com/Article/details/gubenmvxw.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/gsfegvmen.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/gaoougzkv.sHtML

PHP:  // 手写递归交换
来源：http://baike.yfazqb.com/Article/details/ghufzkvnb.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gmrjeqimr.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gxzbrktby.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gdlsnnltp.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gwpkfekef.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/gprdmfjoh.sHtML

C#:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gvxrhpoil.sHtML

[N09] 栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gnbbhsrrp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.vehdjk.com/Article/details/gpsovppul.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gazlumvvv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gsjrgaghf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gmfkioqcr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gamjhaktw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fktsv.cn/Article/details/gjqfbnczg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gevmvdtvd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/gdszitymd.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/gfmlljrvc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/gnpaikgje.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.vehdjk.com/Article/details/gfywklvqz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gjwctqxto.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.sjlbkw.cn/Article/details/gdqfnmyjj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.sjlbkw.cn/Article/details/glizopufh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.epnwcf.com/Article/details/gzziyevak.sHtML


<!-- 参考信息 -->