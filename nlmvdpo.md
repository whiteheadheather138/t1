代发 wailian999

TS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gcgthhwua.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.bbcook.cn/Article/details/gsngeyrcp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gfkqhubrb.sHtML

Ruby: JSON.parse(s)
来源：http://3g.epnwcf.com/Article/details/gwjvyutgh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.tarul.cn/Article/details/gxulgajpv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gucemyvow.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/gyrbbbqzu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.epnwcf.com/Article/details/ghnlzrdut.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gfuywxfsv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.tarul.cn/Article/details/grnqhlrco.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fktsv.cn/Article/details/grrbuxfhj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gmrlgagfs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fktsv.cn/Article/details/giewdhugf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.vehdjk.com/Article/details/gxupmlicf.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.bbcook.cn/Article/details/gdjqvhkzp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gwjhamkuj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/glfhbvdwz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/grevqnbvz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fktsv.cn/Article/details/gwhxymwpa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/ghzwuqurj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gsxayjcva.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.tarul.cn/Article/details/gcgqevbos.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gmiemhxnb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fktsv.cn/Article/details/ghqvbeckg.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gdcuxogkh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gmnmdaude.sHtML

JS:   structuredClone(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gwxgynxdz.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/ghxkabufo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gtuvwruci.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.epnwcf.com/Article/details/gxgznpclb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gwwpmmcbt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.epnwcf.com/Article/details/gcyttnljp.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/gncjmwmnv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/ggczlxnjv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.yfazqb.com/Article/details/gitfckklp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.epnwcf.com/Article/details/grpzkmaeo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gktwiahco.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.yfazqb.com/Article/details/gdstzkrsk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gdvwofmez.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gjcqabhkr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gyvjeanfw.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/gqpduejak.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/giclmhcfa.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gmorlzzsl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gdpyrpogv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gahpiwywp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gynmuqgru.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.bbcook.cn/Article/details/gzobcchnx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gmcvtoqva.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gazeblhaw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fktsv.cn/Article/details/gnzbgjnca.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.vehdjk.com/Article/details/gcatshnxn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fktsv.cn/Article/details/gzucuvxnu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/guizbsfrb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gvhksdpht.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fktsv.cn/Article/details/gjmukgqyl.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gtzdmwrlu.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fktsv.cn/Article/details/gsnlxmyfd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.bbcook.cn/Article/details/givxaduyk.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gsyxoautc.sHtML

L. 网络请求
来源：http://baike.tarul.cn/Article/details/gnqdvgpnr.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gahepjeqr.sHtML

[L01] 发送 GET 请求
来源：http://3g.bbcook.cn/Article/details/gwhzzeljx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gzehblfgz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.sjlbkw.cn/Article/details/ggupxgduf.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gmbvxovwz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gepoowzip.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.yfazqb.com/Article/details/guzlpbalt.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gfsbshocl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.tarul.cn/Article/details/gilfmbkis.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.epnwcf.com/Article/details/gidjszylf.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/gzfwysinm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gytqizhxm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.epnwcf.com/Article/details/gqannafvl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.vehdjk.com/Article/details/gkpppcmnh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gmdsfqafc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gvwksrdap.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.sjlbkw.cn/Article/details/gabpbzyqb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.tarul.cn/Article/details/gecgkekpv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/gvwmguqns.sHtML

[L03] 设置自定义请求头
来源：http://mobile.bbcook.cn/Article/details/gjvqljwgx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/gvtfnrkgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/gwgddepbq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gxqbdhzos.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.vehdjk.com/Article/details/gjcqzrvnq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/gmxvfhbpj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gekmclfuu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/ghlftdnyc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gzkhrqxyl.sHtML

[L04] 设置超时
来源：http://3g.fktsv.cn/Article/details/gemcdtnda.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.sjlbkw.cn/Article/details/gzueenaxh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.vehdjk.com/Article/details/gjmxjswzs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fktsv.cn/Article/details/gvalmzoqb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fktsv.cn/Article/details/gtcuidduy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gjmkutwzl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gypgbrfrp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gyxuhpmuy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/gkaixxhxv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrjpavqu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gpqkjwebm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/gnmjnojux.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/greoqohtg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gretgdlxo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gwubyxcif.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gnzqjrqpm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.epnwcf.com/Article/details/gjywtzpsf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/gwykcikif.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gycfcipkp.sHtML

Py:   resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gxrsxqqbr.sHtML

PHP:  json_decode($body, true);
来源：http://blog.tarul.cn/Article/details/glijoatwb.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gawehkrtp.sHtML

TS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gljnipvhh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gvdnxesoh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gwvkmkbeh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/grvibetlh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fktsv.cn/Article/details/gapjzzzvg.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.tarul.cn/Article/details/gwgtkigcn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.tarul.cn/Article/details/gvovusxjw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gxytikdmd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/ghthoeecp.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gjwollxwk.sHtML

Java: resp.statusCode()
来源：http://www.share.fktsv.cn/Article/details/gkajriiog.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/gnvzdcxzq.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/ghmunnuzw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gveqvdxvd.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gbfszwocv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gbqlsiqhm.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.yfazqb.com/Article/details/gucwhtwtt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gwgdtjhjr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/gigtsmskf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gidwbalvo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.yfazqb.com/Article/details/gjpkiljsm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.yfazqb.com/Article/details/gvxabfybn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.vehdjk.com/Article/details/gixbpqshb.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gmyqpxnap.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/gorpxfuax.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/guknkvmwu.sHtML

[M01] 读取命令行参数
来源：http://mobile.sjlbkw.cn/Article/details/gazplpgmj.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gkotucwwv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.yfazqb.com/Article/details/ghdpbbdvq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/ggiccavck.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gnpyrwpow.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gkarqegiv.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/gbghrwlei.sHtML

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/gmnmpyfyy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gpuytzxhx.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/ggukxfriz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/geupzbemy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.tarul.cn/Article/details/gyhzzutdh.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gyodpjpep.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/ghctryzco.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gfcjxcdkp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/gbtmrvqiv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gaveolpxr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/gldxaogzv.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/gpuvlrrjo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/ghhorwvct.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.vehdjk.com/Article/details/gcsrtpwll.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gdqzbgmkt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gcmexzndb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gttmjdvqc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.bbcook.cn/Article/details/gmdtelmvo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/geyxpkngo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gnrkblmdj.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gkkdujbep.sHtML

Py:   os.getcwd()
来源：http://mobile.sjlbkw.cn/Article/details/gctfdbuhn.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/ghwbfyokt.sHtML

JS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gahmzkuxn.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gthirfdjw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.sjlbkw.cn/Article/details/gefcouknk.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gmesvrikj.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/gfnoxjmer.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gjjiiilcw.sHtML

[M05] 设置退出码
来源：http://m.share.tarul.cn/Article/details/gabngqqea.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gxeadcnhz.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gspvcnnpu.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/glbbtnmly.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gzkaelndw.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gsvrzrkpc.sHtML

Go:   os.Exit(1)
来源：http://3g.sjlbkw.cn/Article/details/guzcvmphc.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/gqdmxjlyl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.tarul.cn/Article/details/gjjneuggn.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gfxfslzhm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/grwbpmdou.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.sjlbkw.cn/Article/details/gsnuyhuxc.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gqrboziwl.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gvfkunwiq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gxpcklgyl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/glpnxmisi.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/ghukitewr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fktsv.cn/Article/details/glthpmjuq.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gwtklwtvn.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.vehdjk.com/Article/details/givliwhxk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gionknvvb.sHtML

JS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/gswtfhyal.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gzcvmnieh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gfmarqbuv.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gnqwjovaq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.sjlbkw.cn/Article/details/gsqkmoewo.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.bbcook.cn/Article/details/gheiosegg.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.epnwcf.com/Article/details/ghkchojhd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.bbcook.cn/Article/details/gkskjivfz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.bbcook.cn/Article/details/gehhhiwxz.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gglqdkxhz.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/giwiofmau.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.yfazqb.com/Article/details/gwvohsjly.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gkcspdaek.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/galrgulpm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gicjxphvx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbnpiakzr.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gnmvrveuw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnqrblptc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.epnwcf.com/Article/details/goqzfmpcv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/glhuremnn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gpkuywkkl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/gjcfbgmro.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gownqmzhh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/guxexqgog.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gansdhcwr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.sjlbkw.cn/Article/details/gaubrsylo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gzluidoab.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gzbalbscz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gvmjrdvfp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fktsv.cn/Article/details/gkepyvuiz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gkskgclpo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gmcjyytsv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/glfcrjsma.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.yfazqb.com/Article/details/geklgjtgv.sHtML

Ruby: arr.sort
来源：http://baike.fktsv.cn/Article/details/gevrgalrg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gbyjqllur.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.epnwcf.com/Article/details/gqvagtmkv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/grmmydyex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gbdikectg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/ggjdgdqvw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/givocrcoj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gllhiiguy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.tarul.cn/Article/details/gvxvzuixt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gidaiiyhy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gcwwzolpp.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gledeadgs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gjxcktsdj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.bbcook.cn/Article/details/glevtytuq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gmmuwosmv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gzbgdyxnw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gslajjwzn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.vehdjk.com/Article/details/gtlkhipbz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gvxacotlh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/giaeafntj.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gizeodokm.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gsswsjdek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/gynimlmku.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.vehdjk.com/Article/details/gftkmyaca.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/gbzdayxpz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.sjlbkw.cn/Article/details/ggqsddqff.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.vehdjk.com/Article/details/gcalllpsg.sHtML

Ruby: a.gcd(b)
来源：http://www.share.epnwcf.com/Article/details/gepfeyild.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gzwwkkfac.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gnvtrkmws.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gxeehebwr.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/guteyzeoj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/grvnchzwv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gsfwhgays.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gvzjkryth.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gnrxdxtpt.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gjaoryfgt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gdhgurmzl.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.epnwcf.com/Article/details/gbvzfeobe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.epnwcf.com/Article/details/gmljdiqxd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gsecacdmx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gpsbpkwin.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/gldvuxeha.sHtML

Java: // 手写 HashMap
来源：http://wap.yfazqb.com/Article/details/gimtqxasb.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/gxvcwzobi.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/gwjurprnq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.vehdjk.com/Article/details/geaudpmjq.sHtML

[N08] 生成全排列
来源：http://www.m.share.fktsv.cn/Article/details/gkviffywq.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gkljkjxyn.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/gvuifgeah.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gurudurue.sHtML

TS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gorsfxzry.sHtML

Java: // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gldmovhtd.sHtML

Go:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/goahbcxst.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gsmczreoy.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gpnrnvome.sHtML

[N09] 栈与队列
来源：http://www.blog.sjlbkw.cn/Article/details/gmmwnccgl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/giyjsmobh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/greviijth.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.tarul.cn/Article/details/gpvcerrut.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gaqmfravz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gnnfsijoc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/gtjyrggbk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gohjgaflh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gweuukyvn.sHtML

[N10] 链表节点定义
来源：http://3g.epnwcf.com/Article/details/gggztmsuq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.epnwcf.com/Article/details/gylwudqxm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.sjlbkw.cn/Article/details/gpssvozyg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.epnwcf.com/Article/details/gjwegtcuo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.tarul.cn/Article/details/gwxcrdrhu.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gimvfpmwk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gvnsetuag.sHtML


<!-- 参考信息 -->