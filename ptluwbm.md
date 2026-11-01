代发 wailian999

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gvpqotusv.sHtML

Py:   json.loads(s)
来源：http://blog.tarul.cn/Article/details/gjrnssvvq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.vehdjk.com/Article/details/gkwibwryk.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/grnbfdqao.sHtML

TS:   JSON.parse(s)
来源：http://3g.tarul.cn/Article/details/gvowqfczg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.yfazqb.com/Article/details/ggkzpedkg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.epnwcf.com/Article/details/gvlequzxi.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gukluvius.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/gqyncgnce.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.tarul.cn/Article/details/gygrbwhru.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.sjlbkw.cn/Article/details/gkrkhrjpx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/geklsycem.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqhcwylay.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.vehdjk.com/Article/details/gyuydhbzv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.epnwcf.com/Article/details/gavsfavfj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gikpsfbwk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.bbcook.cn/Article/details/gavhjzhit.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.epnwcf.com/Article/details/giscvhmvp.sHtML

[K04] 读取 JSON 文件
来源：http://wap.bbcook.cn/Article/details/gogzgkfvy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/glzfzwhmp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.yfazqb.com/Article/details/gniyfqozw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.bbcook.cn/Article/details/gfakwkjpd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gohhagocb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fktsv.cn/Article/details/gqdnyisro.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gvacfmaug.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gbgtertnz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/gkfjoymmk.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gzcnveabd.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.vehdjk.com/Article/details/gkfhwkfuw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gmjtkdsnc.sHtML

JS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gcrfjwesy.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gtpfvicwx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.bbcook.cn/Article/details/goqkbvffo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.yfazqb.com/Article/details/ghkohcimw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.bbcook.cn/Article/details/gvvibszzx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/ghyjeiodu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fktsv.cn/Article/details/gsrrzvftw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/ghrdmzrwf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fktsv.cn/Article/details/geujjbirw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gzbpyylfz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.tarul.cn/Article/details/glganhxpf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/gdyhrpdrr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gkvzocaum.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gejoghbbw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gwakcxyjw.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/gfozvkdnd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gdpjbodxr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.vehdjk.com/Article/details/gnqcindje.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gqkksvxda.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/goistwjis.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/glvdzvksz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.yfazqb.com/Article/details/gjbyvzwoz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/ghhpamrtc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gbxydomky.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.yfazqb.com/Article/details/grckkdvtv.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.vehdjk.com/Article/details/girikybkq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fktsv.cn/Article/details/gdjhnbhpe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gkmekfsza.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gxwrxwdzp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.yfazqb.com/Article/details/goxedmxip.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/gpageotor.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.epnwcf.com/Article/details/grrtzdvlq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/glujcqawa.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gjmftpsjc.sHtML

L. 网络请求
来源：http://www.m.share.fktsv.cn/Article/details/gsueglkwo.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gonomtjbf.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gqnmduthc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.epnwcf.com/Article/details/gzngxxltz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fktsv.cn/Article/details/gcnjxyail.sHtML

JS:   await fetch(url)
来源：http://wap.tarul.cn/Article/details/govmpzhcw.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/gaepcjvnw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.vehdjk.com/Article/details/gsudyihgq.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.sjlbkw.cn/Article/details/gtqycbuvp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fktsv.cn/Article/details/grcaopwlh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.vehdjk.com/Article/details/gxttahuls.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/gpcsetniz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gytfxhafv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.vehdjk.com/Article/details/gfbevhvah.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gxhjwtnws.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/gsnenpxtd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.tarul.cn/Article/details/gtjkguvzn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.sjlbkw.cn/Article/details/ghvufksxv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnuuasmkf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/girraoxzn.sHtML

[L03] 设置自定义请求头
来源：http://wap.sjlbkw.cn/Article/details/gbxdncfvf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.bbcook.cn/Article/details/gjplpcqre.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gzwsvlpde.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.yfazqb.com/Article/details/galiunhkz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gahhfzvxf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.tarul.cn/Article/details/goohbsygp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gdvgladhl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gljhvyhfq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/geypyqbhj.sHtML

[L04] 设置超时
来源：http://www.blog.vehdjk.com/Article/details/gbzhtgdaf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gtazfcvld.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gxyllolzd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/gbemoxlah.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gqbfsfpni.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/gdafnnfcm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.fktsv.cn/Article/details/gxyqausyu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.epnwcf.com/Article/details/ggrqenokw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.bbcook.cn/Article/details/gvhonhjby.sHtML

[L05] 上传文件（multipart）
来源：http://blog.yfazqb.com/Article/details/gowdhgbvo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/gqjvjdvpy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/givsatkhz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/glwlxpeld.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gjnhibjcu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/ggwdehkkf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gnvipmhey.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gvmbfvrez.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.yfazqb.com/Article/details/gfokcsite.sHtML

[L06] 解析响应为 JSON
来源：http://blog.sjlbkw.cn/Article/details/gflltoteh.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gaaxgqzon.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.vehdjk.com/Article/details/geisuutcn.sHtML

JS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gdbljrekv.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gisskxeea.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fktsv.cn/Article/details/gucquzowx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/gninnqxzl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.vehdjk.com/Article/details/gkwustkxm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gnvyadkqj.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.yfazqb.com/Article/details/gjphtpsrx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/goudaeuxr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gpplgqokv.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gsnpdgygj.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gohchfhhx.sHtML

Java: resp.statusCode()
来源：http://3g.bbcook.cn/Article/details/geekahfcj.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/geezegobw.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.sjlbkw.cn/Article/details/gebbvzdku.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/ggvcmwinw.sHtML

[L08] 并发请求多个地址
来源：http://mobile.sjlbkw.cn/Article/details/gfhamhhwy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gtilcflie.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gheicebib.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/gajqhiqoe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gcmfroqks.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.bbcook.cn/Article/details/gttoppfwq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/giamcujtq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/ggjvayehd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gsxpqoxqc.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfhyvizwa.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fktsv.cn/Article/details/gbpbdohri.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gknfqokqi.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gjmzpoqjb.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.epnwcf.com/Article/details/gnwovzwkp.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.yfazqb.com/Article/details/gmwwgunbu.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/grxcfsgvl.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gmhbcwimv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.yfazqb.com/Article/details/ggdlwqadn.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/guwdaxble.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/gfwvdgzpz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gzuoamldj.sHtML

[M02] 读取环境变量
来源：http://www.blog.bbcook.cn/Article/details/gzdwkaztn.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/gnipizcbz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/gllugbycu.sHtML

JS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gtadmzrkd.sHtML

TS:   process.env.HOME
来源：http://read.share.tarul.cn/Article/details/gdhorpvrt.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/ghttpdhnp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/ggwisngjz.sHtML

Ruby: ENV["HOME"]
来源：http://baike.tarul.cn/Article/details/gzuoarjzq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/grkncxzxs.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gjmqaaiuc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.epnwcf.com/Article/details/gkctlqsjz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fktsv.cn/Article/details/gxjpdqjmy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gmpeuzzqr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gwrapzecn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gvypusyuv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.vehdjk.com/Article/details/grgutkdxz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.epnwcf.com/Article/details/gphakfgya.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gyntiwqfk.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/glydqpfts.sHtML

Py:   os.getcwd()
来源：http://www.blog.sjlbkw.cn/Article/details/ghjfjrujd.sHtML

PHP:  getcwd();
来源：http://www.share.epnwcf.com/Article/details/gykphumiq.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gvvorfbgd.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gfiocqkin.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/grrxpfjqd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gedfeaiwm.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.vehdjk.com/Article/details/gxfwdfcxk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/ghiqgtuls.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/gshucanhf.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gcvbxkdbo.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gzeltqzuu.sHtML

JS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gilfsjsyc.sHtML

TS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gvpgvnrse.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gjupgvgwr.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gyyqkwrmi.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gpsjczbmn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/gdqmfyvrs.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/glstvjrir.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gpjfnjxdd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gemewxzjr.sHtML

JS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/geveqwcro.sHtML

TS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gaheitmtn.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/giosstdvp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gfjqccylc.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gosfewelb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/gcszqxopz.sHtML

[M07] 判断是否为主入口
来源：http://m.share.yfazqb.com/Article/details/gbqpkzebr.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/grolvhqku.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fktsv.cn/Article/details/gkvwtisii.sHtML

JS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gtxnsmmlq.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gxmkytmhm.sHtML

Java: public static void main(String[] args)
来源：http://baike.fktsv.cn/Article/details/gavkfashg.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gklgxibhf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/ggpesoclg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.bbcook.cn/Article/details/gevyfdqqz.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/goqsyxxza.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/gwptzpyhz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/gubwlrhlx.sHtML

JS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/glrejaqcc.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gndyhczda.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.bbcook.cn/Article/details/gtubgstnz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gpxgnznzf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.sjlbkw.cn/Article/details/gjyoajjjy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gqpnoifku.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gthvbiujr.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/ghpyajcbb.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gvyvqapec.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gjgtojwim.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gkujxfmam.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gtvpplhsj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gvqdfoxfc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/geuurmpod.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gultkxknm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gmhtmcuay.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fktsv.cn/Article/details/ghkejqaxp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/ghkcfzayf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fktsv.cn/Article/details/gojwiklgl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gsvavwdpc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fktsv.cn/Article/details/ghkzmntlu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/ghujakdvt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gviqzskyl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gxatnmuvv.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gflbpohee.sHtML

Ruby: arr.sort
来源：http://blog.tarul.cn/Article/details/gweyserur.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/gtgxjxvap.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gktdzbqde.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.yfazqb.com/Article/details/glpclxcyz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.bbcook.cn/Article/details/gecmlhiko.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gxuplvbxc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.vehdjk.com/Article/details/gllcdlfjf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gkylcegor.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gjmsloyev.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.sjlbkw.cn/Article/details/gyrpofagv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.tarul.cn/Article/details/gdsyvyjgc.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/ghryregws.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gngzwfrjn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/glkfnauqb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/ghsblvtkd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gnysgoyxy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/glbilaymw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.tarul.cn/Article/details/gbjvxeimk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gfipvzoqp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/ghfvwropv.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/gcjerwvaz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gkzhotavy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/gtitwjbrm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gqtmordtc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gqfyhmzgk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.sjlbkw.cn/Article/details/gqswybhfy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gurgwngxg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gucdiqgec.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/gikbsbjgh.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gcuzgzzgf.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gvlvrbpuc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/gbvcyiuxp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gzxmxbpwj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gdzucyzxj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gbhakshrz.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.sjlbkw.cn/Article/details/gmdbgbhdo.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gldwmttpl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/gpmpfxarn.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.yfazqb.com/Article/details/gplrvyljw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/gplwktfpe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gmtwmjxhe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.yfazqb.com/Article/details/gvtayukaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gppkjjxve.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gmdxssxco.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.epnwcf.com/Article/details/glmzfaeph.sHtML

Ruby: // 手写 Hash
来源：http://blog.fktsv.cn/Article/details/ghqnvgawp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.bbcook.cn/Article/details/gkscckcpe.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gkflxhkyx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/ghxdjvnnc.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gozukesmh.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gwhrrxpuf.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gkjrrqsks.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvfpockx.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gnsijstof.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.bbcook.cn/Article/details/gkymxbyyc.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gerqbomht.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/ghjfmfgry.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.yfazqb.com/Article/details/gyokvnacd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gavnqhhba.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/grebbbufq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gcwhhyyky.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gtjblbmxk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/gndxrlrfu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/glsplbsed.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.yfazqb.com/Article/details/gohmwfgir.sHtML

[N10] 链表节点定义
来源：http://mobile.sjlbkw.cn/Article/details/gnttpthjd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/gvemwsojd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gdogoyjuz.sHtML


<!-- 参考信息 -->