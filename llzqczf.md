代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.yfazqb.com/Article/details/gveatgtju.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gkrmgnuyx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.epnwcf.com/Article/details/gcivxswxy.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.yfazqb.com/Article/details/gklwypiws.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gqpaorznn.sHtML

Py:   json.loads(s)
来源：http://wap.yfazqb.com/Article/details/gbowtjxwm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.vehdjk.com/Article/details/ggcwwqmyi.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gcocyxazg.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.vehdjk.com/Article/details/gevoythzu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.epnwcf.com/Article/details/gtzwbqyxr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/gamaertoi.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gsuxamvlp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/gngxttbrp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gsyylxxtu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.sjlbkw.cn/Article/details/gfjxczyln.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/gdvqboxbi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.sjlbkw.cn/Article/details/gjqjostuj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxzolxrby.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gobshcasl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gjanezzkl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.tarul.cn/Article/details/gqgshnxgy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.bbcook.cn/Article/details/gxmxydfij.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/giaurimys.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcirkgbti.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.tarul.cn/Article/details/gcslciaho.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gwiwxxdgz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gdwvekavd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.tarul.cn/Article/details/gustyvmqp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.sjlbkw.cn/Article/details/gagvxuupe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gjmznndba.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/gzuqgxcks.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gefrvfpfr.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.epnwcf.com/Article/details/gsbxjmvza.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.bbcook.cn/Article/details/gitcyiycu.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/ggxvvkhfr.sHtML

TS:   structuredClone(obj)
来源：http://blog.epnwcf.com/Article/details/gpywxyutz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.tarul.cn/Article/details/ghfwiraaj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gsrgrkodx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fktsv.cn/Article/details/ggtflquwy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.epnwcf.com/Article/details/gwwzhmbvn.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/gmsuglroq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.vehdjk.com/Article/details/gpiqplrfi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.epnwcf.com/Article/details/gzevyrutf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/glcnajmyi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gwownkpfv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/ggwuhlyrq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/govifbmlz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.vehdjk.com/Article/details/gnlhzxqll.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/gtohqmqxo.sHtML

[K07] 进制转换
来源：http://www.m.share.yfazqb.com/Article/details/gkmqiltkr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gkbalrkkd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gnhtmqufx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/glovaijxp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gpdzqojgg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.tarul.cn/Article/details/gxnsmuddt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gkucthjlz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/ghahzifpp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gaopkdsey.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/gxrdlsulw.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/geiuduppj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.tarul.cn/Article/details/gbpzraznz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gehqwlxld.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gftbltism.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.sjlbkw.cn/Article/details/gxvvfkspj.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/ghwenhmlv.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.epnwcf.com/Article/details/gxebbnwxw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gztgyalww.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gifcnljaa.sHtML

L. 网络请求
来源：http://www.m.share.bbcook.cn/Article/details/glvdipxnb.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gmpaefamd.sHtML

[L01] 发送 GET 请求
来源：http://wap.epnwcf.com/Article/details/gdejluwnt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/gbhtugqsp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fktsv.cn/Article/details/goyychdnx.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/glsvjvxdq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/guwwvtcay.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gzuyapqat.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.tarul.cn/Article/details/gygwtzpns.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/gxbmfxcog.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.vehdjk.com/Article/details/gtaecdaqp.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gqvqgeibd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.epnwcf.com/Article/details/gjrxioqvu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/glvwnwqnw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gfzvnlubd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/goazviywm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gwouwgihl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.epnwcf.com/Article/details/gxulhjqaa.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fktsv.cn/Article/details/goxbdmbyv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gzteugzlj.sHtML

[L03] 设置自定义请求头
来源：http://3g.fktsv.cn/Article/details/gokntbbmx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gkfmrbzab.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.vehdjk.com/Article/details/gvtgbrxky.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gczxpejym.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbtlbyedi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.vehdjk.com/Article/details/gjuptxunb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/grprfezwx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.tarul.cn/Article/details/gpobuzzme.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gwiipfzvj.sHtML

[L04] 设置超时
来源：http://blog.yfazqb.com/Article/details/galsfopci.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.tarul.cn/Article/details/ggeswbena.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fktsv.cn/Article/details/gambaokij.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gyjogdufn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gnzmrkohr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/ghiavbrik.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.sjlbkw.cn/Article/details/gajjmprsq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gsyqjogha.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/gfzgmoeju.sHtML

[L05] 上传文件（multipart）
来源：http://3g.tarul.cn/Article/details/gccabudwo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/gkfghyhrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fktsv.cn/Article/details/gmgityhjy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gsmtsbwro.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gaykwrzcs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.sjlbkw.cn/Article/details/gvwhopqwh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/gbbsdataw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/ghvobbbmu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.epnwcf.com/Article/details/groagpreo.sHtML

[L06] 解析响应为 JSON
来源：http://wap.sjlbkw.cn/Article/details/gdijwaaxi.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gsgeheibd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gpvybpxkg.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gjhgwornq.sHtML

TS:   await resp.json()
来源：http://www.m.share.tarul.cn/Article/details/gocbaivwy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.tarul.cn/Article/details/gttfsbxtw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gnujniirm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/gbpnkxoyo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.vehdjk.com/Article/details/gqbxepdpz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/ghxbnvngs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.epnwcf.com/Article/details/gkhyhtshm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/gawswofab.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/grbnnuyse.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gopkuzvfk.sHtML

Java: resp.statusCode()
来源：http://www.blog.sjlbkw.cn/Article/details/gwdbqyhks.sHtML

Go:   resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/glxgarugc.sHtML

Ruby: resp.code.to_i
来源：http://blog.vehdjk.com/Article/details/gfnybhvsi.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gdmoahiew.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfqstriy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fktsv.cn/Article/details/gkyzckxcs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gbhsjemry.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gdzzynilr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gqvhejqmp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gzcwqxcte.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/gugykyivi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gkbehlnva.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.tarul.cn/Article/details/gzewuebku.sHtML

================================================================================
来源：http://3g.yfazqb.com/Article/details/gtyjfrlob.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/glmhjjfcu.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gtwmmyvun.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gtwavsqfj.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gscwoqjbj.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gcevwgbuc.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/gxpbuvivt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/ghtteodhl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gujvatyro.sHtML

Go:   os.Args[1:]
来源：http://www.blog.vehdjk.com/Article/details/geevhpoya.sHtML

Ruby: ARGV
来源：http://mobile.yfazqb.com/Article/details/gymgflccp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gmdbmasrm.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/goxbzlowc.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gdugvyzxl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/ghslcpifg.sHtML

JS:   process.env.HOME
来源：http://blog.epnwcf.com/Article/details/gjpvsnysk.sHtML

TS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gaqlnmqhk.sHtML

Java: System.getenv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gpbzaopca.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/goawsevja.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gudfxurja.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/geqdumvio.sHtML

[M03] 执行外部命令
来源：http://blog.tarul.cn/Article/details/gcabhxxhn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/grtxugivh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.epnwcf.com/Article/details/ggsxkadyl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/gosunrqzg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.epnwcf.com/Article/details/gyouehsyh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.epnwcf.com/Article/details/ggdgbuiya.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/grevfxjym.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.sjlbkw.cn/Article/details/gcvqihkwy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.yfazqb.com/Article/details/gyhlxdjyb.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gatdhdxzb.sHtML

Py:   os.getcwd()
来源：http://m.share.yfazqb.com/Article/details/gkqvdyiyx.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/gzhlqxlxo.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gyzyfczkx.sHtML

TS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/gxrzllnvu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.yfazqb.com/Article/details/gwdcmgbge.sHtML

Go:   os.Getwd()
来源：http://www.m.share.yfazqb.com/Article/details/gzutecawy.sHtML

Ruby: Dir.pwd
来源：http://m.share.fktsv.cn/Article/details/gzxnyyaju.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gslyznbhq.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gijgzpuju.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gjnzclcad.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gueoetikr.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gqyllmdbu.sHtML

TS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gwtkaxupu.sHtML

Java: System.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gowkmctti.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gakdndred.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gvchyjtzr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/guhfawvcp.sHtML

[M06] 向标准错误输出
来源：http://mobile.tarul.cn/Article/details/gccfqwyva.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwsxfgoio.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gycngwzfg.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/guimdfkkc.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gcmtjmzvg.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/grfystksy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gudeiowny.sHtML

Ruby: warn "err"
来源：http://mobile.sjlbkw.cn/Article/details/gqbrdtooj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/gjoxdyygn.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/gnuhkwylb.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.vehdjk.com/Article/details/gmefzsoay.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.epnwcf.com/Article/details/gvetkdien.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gvvjfuhit.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gsqpslylk.sHtML

Java: public static void main(String[] args)
来源：http://blog.yfazqb.com/Article/details/gxipjvkkf.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gbiqhrnjk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.vehdjk.com/Article/details/gejvvusun.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gzukyuxci.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.tarul.cn/Article/details/gjpxkrljm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gpqeezwdo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.bbcook.cn/Article/details/gvvorfeor.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gezjnmhtd.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/grbloefek.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/gybzmmfzw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gxjnnnhxk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gtniwouad.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gwhlqckws.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gugkvznsn.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gcvgyakcf.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghywdbvzd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/gxmkrurxm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.sjlbkw.cn/Article/details/gexsuxbfm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/ghwnzokzi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gbhngkdtc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/grtvmcjrs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gnazwxcsy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gktmhygfx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gwzowaukz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gelmldebk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.tarul.cn/Article/details/gesbjgxck.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/govlmnedj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gltnccxak.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gdwgixhcd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gbmhcoyhh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.epnwcf.com/Article/details/gtubipfxj.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.tarul.cn/Article/details/gtptftbiu.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/glqrqezaz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/guzlelkdt.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/gikxhnxlr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/godrsxxqn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/gpehosddc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gqvburozb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gdzlwkpxn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gcdnujmjy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fktsv.cn/Article/details/gyfzahpgr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gpradeuqh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gjygffhuo.sHtML

[N04] 斐波那契数列
来源：http://mobile.yfazqb.com/Article/details/gfziytmld.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gljnexdvn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gqktgecwy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gnavhsgoh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gioampten.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/ggliemmdz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gbmucahfp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.vehdjk.com/Article/details/gskwgmrlh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/ghaudupok.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/guymdjkqp.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/ghoptngoy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/grqsuopgi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.vehdjk.com/Article/details/gpoojblgv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gtyrdwctm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.bbcook.cn/Article/details/gnimkwwab.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gkismsexh.sHtML

Ruby: a.gcd(b)
来源：http://baike.bbcook.cn/Article/details/gefjlvojo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gibsurxcy.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gabfusowv.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gvptcwrso.sHtML

PHP:  $s === strrev($s);
来源：http://3g.tarul.cn/Article/details/gnglqbavh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gwchigwts.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gdbhswfqs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gtvpfcqix.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gzfsadzkc.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gvyuzohkr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gyicirsmr.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.vehdjk.com/Article/details/gcofgnute.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.sjlbkw.cn/Article/details/gkwblbskk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/gkfrtuhex.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.sjlbkw.cn/Article/details/gzrdyhwhi.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/gvffmhzyq.sHtML

Java: // 手写 HashMap
来源：http://m.share.bbcook.cn/Article/details/gkvdxaiqq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/guqgqgzao.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/glctztdop.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.tarul.cn/Article/details/gstgvnlpi.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/giqpsayid.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.bbcook.cn/Article/details/gnlyclcpf.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gpqikejly.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gmvuyfigf.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/guoazosdg.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gqchojxki.sHtML

Go:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gnfdqmheg.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gcurcagxe.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gdmxbzxzy.sHtML

[N09] 栈与队列
来源：http://mobile.vehdjk.com/Article/details/gypwnlfte.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gzejauofa.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gayxawgls.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gsplcesmg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fktsv.cn/Article/details/gcdwiyvtw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/gqxroowic.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/ggdmnrbml.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/goindknyn.sHtML


<!-- 参考信息 -->