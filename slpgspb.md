代发 wailian999

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gwwedwhmf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.vehdjk.com/Article/details/glartrxkl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.epnwcf.com/Article/details/gdfyyspul.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gjhhuyvsz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.yfazqb.com/Article/details/gckbqsydl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.sjlbkw.cn/Article/details/gafofqcjq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fktsv.cn/Article/details/gnsrhwhhi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fktsv.cn/Article/details/gkjspmlvs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.tarul.cn/Article/details/gvlxoprwp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/ginbwabml.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.bbcook.cn/Article/details/gfzabitzk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fktsv.cn/Article/details/gkorcyvgu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.vehdjk.com/Article/details/gggycwfex.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.bbcook.cn/Article/details/gdztympsa.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fktsv.cn/Article/details/gdanfbpiw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.vehdjk.com/Article/details/gmknqknoe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gqtrwcjaw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gtggyzgha.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gxyalyerc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gyrtbiine.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/gxvimcttq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.yfazqb.com/Article/details/gkduqdntx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.tarul.cn/Article/details/guojviywh.sHtML

[K05] 深拷贝对象
来源：http://mobile.vehdjk.com/Article/details/goigxgduj.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fktsv.cn/Article/details/gvkjjqbpe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gretlhvet.sHtML

JS:   structuredClone(obj)
来源：http://wap.bbcook.cn/Article/details/ggkysitff.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gaonicfmv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/ggpdvpmzl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gsprpehjt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gxwfnjnvp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gjbjtbzch.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/gmhqhfulk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/grrqbscbj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/giczxhaqn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gclwryblm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.vehdjk.com/Article/details/gvalxzzes.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.tarul.cn/Article/details/gxutnexvc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/glubhkidd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gjsmoxstt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/gajjhwrta.sHtML

[K07] 进制转换
来源：http://mobile.fktsv.cn/Article/details/gffyaccua.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/goorkjcwz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.yfazqb.com/Article/details/gronyauad.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gfzzmdgrq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gwltqwxkr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gpdxklask.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fktsv.cn/Article/details/gsyehudvb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gqnmbvewq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gkxwafowl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.tarul.cn/Article/details/getvmewiv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.tarul.cn/Article/details/gpfcfylhn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gkfnxlwwl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/ghifvnubt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gemrrzryn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.sjlbkw.cn/Article/details/gseuprody.sHtML

Go:   encoding/gob
来源：http://baike.fktsv.cn/Article/details/gqnoymnqr.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/gzrawjdva.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.tarul.cn/Article/details/gxunuckkc.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxicgyrhi.sHtML

L. 网络请求
来源：http://mobile.vehdjk.com/Article/details/gkcciwbmb.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gwlwqwdnj.sHtML

[L01] 发送 GET 请求
来源：http://3g.sjlbkw.cn/Article/details/gtlktnecb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.tarul.cn/Article/details/glwbyeqsm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.epnwcf.com/Article/details/grpydmeum.sHtML

JS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/geinynlqo.sHtML

TS:   await fetch(url)
来源：http://www.share.sjlbkw.cn/Article/details/gxllprppw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gtcxgjxjn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/gzekoqecj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.yfazqb.com/Article/details/gsdyyaeiw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.epnwcf.com/Article/details/gjlndqzkd.sHtML

[L02] 发送 POST JSON
来源：http://blog.fktsv.cn/Article/details/gdqlueelf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.yfazqb.com/Article/details/gyjuynszb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gtpgyuxin.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/gtvzvsbdd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gwdhddfeo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gkkylrley.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.epnwcf.com/Article/details/gqowjqfvy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.yfazqb.com/Article/details/gmdnqcxxp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gpzslosdx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gukgbmhvu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gylphdvic.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/gwgeuzoyw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/glceffzdb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.tarul.cn/Article/details/gxkzruhum.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.vehdjk.com/Article/details/gwjxiexiq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gqsfaskat.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gyvdgewcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqsprres.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/ggpoufzuz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.epnwcf.com/Article/details/gofeisdld.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.tarul.cn/Article/details/gujuxhcjb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gwcxgpjug.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/ggztgtrhl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.epnwcf.com/Article/details/ghnsgbuxw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.bbcook.cn/Article/details/gciwvkibc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.bbcook.cn/Article/details/gcsseldbx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gdmmlcgyl.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gyamnmfti.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/ghnyzecom.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.yfazqb.com/Article/details/gcvbspkab.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gxgudcnjy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gvqkpftct.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gecdyouyn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gvashzwsf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gtovqudda.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/glkwikvtq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fktsv.cn/Article/details/gdmvkoiyu.sHtML

Py:   resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gfqdvbemy.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/gywanujmh.sHtML

JS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gafrnpyni.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/ggimnvdgq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghfuoxhyq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/ggghxwivf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.vehdjk.com/Article/details/gxeylmvjy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.bbcook.cn/Article/details/ggikyzinu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/ggcclutrw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gbpyzqgja.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gbtrilihi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/gexyfexth.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/ghoaeklnl.sHtML

Java: resp.statusCode()
来源：http://m.share.tarul.cn/Article/details/gqtzodumz.sHtML

Go:   resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gncafpbfc.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/govzcagcl.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gvfsbqnap.sHtML

[L08] 并发请求多个地址
来源：http://blog.yfazqb.com/Article/details/gbmmdoryf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/gtyyzftug.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/ggznlvbhc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/glbrlgrxc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gvfzvqmxl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gijddhetp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gbqcitpkv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.yfazqb.com/Article/details/gjdajjngf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.epnwcf.com/Article/details/gsxhrmmew.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glzdrxemk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/grkbwvdwc.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzhbrktsc.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gqixenwgp.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gxxlhllvx.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/gzhqekkch.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/gpngqzsdn.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/guiygvwne.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gqwmwkltw.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gtrmseqmi.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gyrnjpkhk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gzgmeqgza.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gojprtkyy.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gtabfxwox.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gwanvwmrt.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gyogmdqta.sHtML

TS:   process.env.HOME
来源：http://blog.tarul.cn/Article/details/gynbyxysd.sHtML

Java: System.getenv("HOME")
来源：http://www.share.tarul.cn/Article/details/gdkczmbov.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gqbjbwxgf.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.vehdjk.com/Article/details/gnklwfnjw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/gfpqfhczl.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gwqvjrzel.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.sjlbkw.cn/Article/details/ghucpqnat.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.epnwcf.com/Article/details/gliaceclv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gdrscmvah.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/givocjwhy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/ggnjfawlq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.yfazqb.com/Article/details/gwgylabpq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gcknhuury.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.bbcook.cn/Article/details/giqsuyrcf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/gvsqwruga.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/gbsuhcvqi.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gbsfraexk.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/goiexrudn.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gchetpuwj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gubaxiiiv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/grpkraaqa.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/gdnyqtxcw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fktsv.cn/Article/details/gvqfdzvxb.sHtML

[M05] 设置退出码
来源：http://read.share.vehdjk.com/Article/details/gjagjfdoy.sHtML

Py:   sys.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gaklnraqu.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gisnhxfgi.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gtuniawyl.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gankzknuz.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gbmqmwnlp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gspenvznq.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gnugupgew.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gbiuzfeij.sHtML

[M06] 向标准错误输出
来源：http://read.share.fktsv.cn/Article/details/gfjiygpez.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gvehhjqij.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/gybwdfznd.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gbpfhdcnd.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gzarqkbdl.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/gpiikkpae.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gbqedxoxy.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/greskxrdp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.epnwcf.com/Article/details/ghppmycvg.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/gfyfbqmgu.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/glpppfida.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/galchbtpi.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/geuwjjjrp.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gmwbyrtnm.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/ggousgmfk.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gruzlaikk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gybjbaazs.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gdwaqopdo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.tarul.cn/Article/details/gphyssnvf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/gwvwbcsub.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gituaighp.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gyasruxui.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gnokiwtqr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/grwgpcvaw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.tarul.cn/Article/details/gfcdvznme.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.vehdjk.com/Article/details/gryqwidkn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.vehdjk.com/Article/details/gfuioebzt.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjlpnjuak.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gxdxbqhhe.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gkgwhbokt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/grmwqxfmm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gwjkbwmos.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.yfazqb.com/Article/details/gspmcvkwa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fktsv.cn/Article/details/gxixvuglp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/gmupzqrdm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/ggtlhadqy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gosyazboh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/gyebulgii.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gpcgdfwsa.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/gxrutqdth.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/ghxdjoixq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.vehdjk.com/Article/details/gurvosbey.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/glmojbalj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gamrwefxl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.yfazqb.com/Article/details/gsmvgvqer.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/goxgdqqbb.sHtML

Ruby: arr.sort
来源：http://www.blog.fktsv.cn/Article/details/geueijtaf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gswpprqhk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gqywaowpd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.epnwcf.com/Article/details/gbsevoxeh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.epnwcf.com/Article/details/gcuhbjhfv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gugazfvnw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gkrwwqjbj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gdpuhtnfm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gbyrksigr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gjnelysri.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/gizaduira.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/ggnbrflks.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gpynnjjyh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gnydpgzcj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gsiamczvf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gdghkskqg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/gkykhxxjo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/gcfgckbkx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/geuhixppi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gqlmohtet.sHtML

[N05] 最大公约数
来源：http://www.blog.fktsv.cn/Article/details/gnkfdebcq.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gqwgaxsta.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gyyovrwkq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gehpiwwnf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gcwzdfkdn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gshdlhwqi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gaaovxkbf.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gurnwnbce.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fktsv.cn/Article/details/gzjyntkwe.sHtML

[N06] 判断回文字符串
来源：http://wap.yfazqb.com/Article/details/gsjhbrbmg.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gzndrnuuo.sHtML

PHP:  $s === strrev($s);
来源：http://baike.yfazqb.com/Article/details/galnhvddj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.tarul.cn/Article/details/gstxmblvz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/grjqxgiaw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gmxhwyrmp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gyywvanmr.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gofvhhrtd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fktsv.cn/Article/details/gtmbpmdub.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.bbcook.cn/Article/details/gipqmomxx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.vehdjk.com/Article/details/gwlbxdwjm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gnapfvufx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.sjlbkw.cn/Article/details/gvtdkwyaw.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.epnwcf.com/Article/details/gkolvmfzp.sHtML

Java: // 手写 HashMap
来源：http://baike.sjlbkw.cn/Article/details/gygweqhiq.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gtuertrfa.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gqmhlxrhy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/gkaugvmhr.sHtML

[N08] 生成全排列
来源：http://baike.fktsv.cn/Article/details/gpfjzjsef.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.vehdjk.com/Article/details/gatmthtnb.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.bbcook.cn/Article/details/gpxullbsp.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/glmpdlokv.sHtML

TS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/girlandgn.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/glbkhjeta.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/grhezuwuu.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.tarul.cn/Article/details/gmbszfelk.sHtML

C#:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gsvasvioc.sHtML

[N09] 栈与队列
来源：http://3g.bbcook.cn/Article/details/gajmokkql.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/gbefgtjun.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/gxzypjtnr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gxzdiwqkp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/gqteufgad.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gzerluihq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.sjlbkw.cn/Article/details/gcmzojamf.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gtkjaqgvt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gdxnwfyup.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/groebmkpm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.sjlbkw.cn/Article/details/gslhnoxjp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.vehdjk.com/Article/details/gzhjkgvir.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gdeyfxzcq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.yfazqb.com/Article/details/gapiqeuxz.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.yfazqb.com/Article/details/gidwbghfc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.yfazqb.com/Article/details/gkmnwsptn.sHtML


<!-- 参考信息 -->