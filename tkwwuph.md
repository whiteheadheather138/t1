代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.bbcook.cn/Article/details/giemvwmei.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gcvowjtph.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.bbcook.cn/Article/details/ggxqnstds.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.epnwcf.com/Article/details/glxnpfwjl.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/goawsippn.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fktsv.cn/Article/details/ggnekdprp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.yfazqb.com/Article/details/gjvmmfllk.sHtML

JS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/glpgyzdco.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gpdgeqbbr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gwzwemqml.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gghvqphyx.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gpprxjgox.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.epnwcf.com/Article/details/ggrizhogh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.yfazqb.com/Article/details/gbaeobzmo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gcnvfjlrv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gogcnxlvl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/gkwsuqxki.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.vehdjk.com/Article/details/gvjzjloqz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/gpwcrkoix.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gasjqsaoj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gzjfqxbef.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.bbcook.cn/Article/details/gyswmytzy.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.bbcook.cn/Article/details/gxlcgwwcy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/gcluojwev.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/ghyahhzzn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gquyjxojx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gpxbkdgio.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/givrycfuz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.sjlbkw.cn/Article/details/guhljdxev.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gzrmcazpq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gpkonspls.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/ghgrydtex.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.sjlbkw.cn/Article/details/gumkmxubi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.tarul.cn/Article/details/gkcfisizl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.bbcook.cn/Article/details/gkrsfyaam.sHtML

TS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gdwpyheks.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.epnwcf.com/Article/details/ggopjsfcq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fktsv.cn/Article/details/gbezkvpie.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.yfazqb.com/Article/details/gyrsxjaui.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.epnwcf.com/Article/details/ghurkpgbo.sHtML

[K06] 解析 URL 查询串
来源：http://baike.epnwcf.com/Article/details/glxfmmayl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gfwwwattl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.epnwcf.com/Article/details/gqthcxrfp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fktsv.cn/Article/details/gtbllqwkg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gvksxvitb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.yfazqb.com/Article/details/gtiamynop.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fktsv.cn/Article/details/gbwxszzzs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gzkzxaolj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/giknkhfde.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gtwpmafdq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gyoljntxb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/gzrkquyvq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gcqfeahrz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gtuehhmtt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gdehuykhk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.tarul.cn/Article/details/ghgpxflzp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqckaycyv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gnypkmbwh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.yfazqb.com/Article/details/gdmgskpuh.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.yfazqb.com/Article/details/guipgbndu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fktsv.cn/Article/details/goufrisft.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.vehdjk.com/Article/details/gtptqnmwb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.yfazqb.com/Article/details/gsjjeblcx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gefjabhsx.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/glscbmnpr.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gwdfaqcvl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.yfazqb.com/Article/details/ghkhkklyn.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gnqnhfzya.sHtML

L. 网络请求
来源：http://baike.bbcook.cn/Article/details/geecojtls.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gowgodiqv.sHtML

[L01] 发送 GET 请求
来源：http://3g.fktsv.cn/Article/details/gyagzzpob.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.epnwcf.com/Article/details/gxmknpypk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.tarul.cn/Article/details/gfrlbalvv.sHtML

JS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gtabjvqqi.sHtML

TS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gjggxadwt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.epnwcf.com/Article/details/gcqzmbnfo.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/gzjfeqojy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/grsnhtzix.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/gvqbfdwsd.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.sjlbkw.cn/Article/details/grsdquijz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gzffwpcsc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fktsv.cn/Article/details/guwcgspee.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.bbcook.cn/Article/details/gbvwqcwzc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/giheilnsx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/guiccfeck.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/gvhlmdyeq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gskvnkbes.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.sjlbkw.cn/Article/details/gbhygfxia.sHtML

[L03] 设置自定义请求头
来源：http://www.share.yfazqb.com/Article/details/gzeqwsihc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/gdfaodotp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gprvivkvz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gemiuvlpb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gxzmcfvwh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/guadxazql.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/glkkxlvnc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/gdhtigicj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gknevvsnj.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gutgmprny.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/gvzdnquhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.sjlbkw.cn/Article/details/gsawihbed.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gxeufinjs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fktsv.cn/Article/details/gblmdimep.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gdfiicfnm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gwbgaarqc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gvqheboeh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gpegaiavh.sHtML

[L05] 上传文件（multipart）
来源：http://wap.yfazqb.com/Article/details/gqsebzfys.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/gonkawdxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/ghrnqmxfb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gxihfmzbc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/ggkjepnkq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.tarul.cn/Article/details/gtsamhyzr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.bbcook.cn/Article/details/gkifazvym.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fktsv.cn/Article/details/gicrabcls.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.epnwcf.com/Article/details/gtimgnhit.sHtML

[L06] 解析响应为 JSON
来源：http://3g.sjlbkw.cn/Article/details/gffdueals.sHtML

Py:   resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gdkcbtnan.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.yfazqb.com/Article/details/gtxiaspwk.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gmbnrnank.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gddzpdwlg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gdrxsgjrp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/groytizhj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/girhjivjd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/gndqbqwch.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gsazbmtnl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.vehdjk.com/Article/details/grwbnmkzs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.sjlbkw.cn/Article/details/gqphafauu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/grghvnmsj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/gdumssswt.sHtML

Java: resp.statusCode()
来源：http://www.share.tarul.cn/Article/details/gfihfvcae.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gnxlzdlsp.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/glgpbfukg.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gvfsxccjk.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fktsv.cn/Article/details/getnwwnmd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fktsv.cn/Article/details/grvbyeusg.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gaibetiwm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gegzpnlia.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/ghyborgbg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.epnwcf.com/Article/details/gbjonjnqp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gsacqmzjq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.bbcook.cn/Article/details/govpuvqua.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gomckxdyl.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gxutflpbc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/gsytcdmma.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gxlirwpxb.sHtML

[M01] 读取命令行参数
来源：http://baike.bbcook.cn/Article/details/glihsypyb.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gjjxoqayn.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gjunbizmy.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/gtgbskote.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gvngqfdqn.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gaghteknb.sHtML

Go:   os.Args[1:]
来源：http://3g.fktsv.cn/Article/details/gmgjrclum.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gkozeucke.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gqhvkwqtg.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/guoysiqnc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.tarul.cn/Article/details/gxggxgwxi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gplkhqxza.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gbelzvslf.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/giqhpuxqm.sHtML

Java: System.getenv("HOME")
来源：http://blog.tarul.cn/Article/details/gtrogoxpz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gighqwytx.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/ghvsosvqy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gquhopdlz.sHtML

[M03] 执行外部命令
来源：http://m.share.fktsv.cn/Article/details/gmodwlboz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/gannncbfz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gwfgbjhea.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gmmnrypsx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gmifccstl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/gmpuviqtb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.sjlbkw.cn/Article/details/ghcjmzagi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gqlvifohs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.vehdjk.com/Article/details/gzkznzqws.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/glhsioakb.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gnpgzjmcc.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/gjyqtksfl.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gqxfojukl.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gjnptjrym.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.tarul.cn/Article/details/guasxwnof.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/gokyoqjgg.sHtML

Ruby: Dir.pwd
来源：http://3g.sjlbkw.cn/Article/details/ghszolicg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/gxlkqtjlk.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gsgfxwpvk.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/guayhcqho.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gllttnyia.sHtML

JS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gcgvxcwdn.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gtfrjswps.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gzvsiwpxz.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/ghvdaqmpy.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gqiimbxhc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/gsfpjgykj.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gzkjsrawb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gyjvmjdyk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/ghpiaqpho.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gnhdpwggo.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gonbmqthr.sHtML

Java: System.err.println("err")
来源：http://baike.yfazqb.com/Article/details/gyllxrozo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/gtchnteqk.sHtML

Ruby: warn "err"
来源：http://mobile.epnwcf.com/Article/details/gmtvutxzl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/gyixymssd.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/gamzjkchu.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.bbcook.cn/Article/details/gkjikurkl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fktsv.cn/Article/details/gukwnwzkz.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/grxkblswq.sHtML

TS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/ghylbfglt.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gmpkpdlbo.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gsewspnlq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gfkxiquhm.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gcarmlzpw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gfgfugmmy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.vehdjk.com/Article/details/gqzzhelhz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gxvdhbhoy.sHtML

JS:   process.platform;  process.version
来源：http://mobile.bbcook.cn/Article/details/guvywozux.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/ggeuccmcp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.epnwcf.com/Article/details/goetdimmd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gscemgnlf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/gzaurzfxj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gmtlywbhd.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfxpgzalb.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/geiqwmxuz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/grsckkdhk.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.vehdjk.com/Article/details/gjfdbfytz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbjcqiaon.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/ggscsbeqx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gpcdnwbmr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gisgewcpc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gzrkcencx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gkfsgtike.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/ghajkfhgn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gdqrjzorc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.tarul.cn/Article/details/ghjjcwbfc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gyxpubzdp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.bbcook.cn/Article/details/grrrqxgrm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gtknubhom.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gxfvmldlj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/gciblhuto.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/ggfmexbkn.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/ggtptblbb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.epnwcf.com/Article/details/gvhxrfbbo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.vehdjk.com/Article/details/gktuxitwp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/gptokkniu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gezurbpes.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/gsvanaovy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gqrnsrdwf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gmjbnsghz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.yfazqb.com/Article/details/gcejwyfrm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gugbtrhbk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gdwodpkiu.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/gizlwamlq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fktsv.cn/Article/details/gfcgeimxm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.vehdjk.com/Article/details/gtcvrgaxv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gtflrijnv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gfroepxth.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gmmyawiol.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gqgogjfut.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gjybirdwz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gugfyrffl.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/gfujavqcr.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gbfzimbgm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.tarul.cn/Article/details/gezvdaspt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gbikbuuec.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gpxaujyem.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/ggqvezlpx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.bbcook.cn/Article/details/gtxtgwcgn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/ghnswtmzi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/gbscfljhd.sHtML

[N06] 判断回文字符串
来源：http://3g.yfazqb.com/Article/details/gxfxtafle.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/giohiieuw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.vehdjk.com/Article/details/gibcoeexc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/genmmfmid.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/geoixxbtp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fktsv.cn/Article/details/gewtawwxy.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.vehdjk.com/Article/details/gxtzlmjeo.sHtML

Ruby: s == s.reverse
来源：http://www.share.bbcook.cn/Article/details/gkpznhaad.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gthdjzlqd.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.epnwcf.com/Article/details/gjcvazweu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.bbcook.cn/Article/details/gfwpeyipw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gxvlgjejh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gnylpmqzj.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.tarul.cn/Article/details/gdvbwnsdr.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gkrepzmyj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.yfazqb.com/Article/details/gdhhynnin.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/ggsdgnlqv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.vehdjk.com/Article/details/gnnizoyuz.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/gbtnjltgg.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.vehdjk.com/Article/details/ggyzstzgs.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/guhqjhqqm.sHtML

JS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gsjfkwlzf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gmvucckco.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gqsbliywg.sHtML

Go:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gdaxmhjde.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gcohczxgs.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gkmaxpjhx.sHtML

[N09] 栈与队列
来源：http://read.share.bbcook.cn/Article/details/gszvfgpyu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.vehdjk.com/Article/details/gljvryfwq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.bbcook.cn/Article/details/gwcdgzsmw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/glviykeib.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/gwzwtrqdb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fktsv.cn/Article/details/gceoqhzgn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.sjlbkw.cn/Article/details/gtswjkxir.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gzfonfjcd.sHtML


<!-- 参考信息 -->