代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.vehdjk.com/Article/details/geixqifwm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gnspgtkgj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.tarul.cn/Article/details/gbpjtfdoc.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.epnwcf.com/Article/details/gxcqbronu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.epnwcf.com/Article/details/glkgbatqv.sHtML

Go:   json.Marshal(obj)
来源：http://blog.yfazqb.com/Article/details/gvxshukfm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.vehdjk.com/Article/details/gbswimcxj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.bbcook.cn/Article/details/gxxhcauuy.sHtML

[K02] JSON 字符串转对象
来源：http://3g.yfazqb.com/Article/details/gfogfguhs.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gxrwlwjep.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.vehdjk.com/Article/details/grocljvio.sHtML

JS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gflavebyp.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gmaltdlni.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gehnqjuqa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/ghjnqsxuw.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/geyplmknf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fktsv.cn/Article/details/gqcgojwum.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.sjlbkw.cn/Article/details/grqlwwkeh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.sjlbkw.cn/Article/details/goljfasft.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/ggevaklbs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.sjlbkw.cn/Article/details/gcnlkvkzy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gnscykfln.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.bbcook.cn/Article/details/grlcnchig.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/gqfrxiozw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gufaxdbsc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/grilwcsqs.sHtML

[K04] 读取 JSON 文件
来源：http://baike.epnwcf.com/Article/details/gitsnpotl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.bbcook.cn/Article/details/gkgodyozm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gebzcyuaj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/gahlbsjmp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/ghwlgwizj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.tarul.cn/Article/details/gcafvqwdp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gsoxjfhvv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.tarul.cn/Article/details/gltidolch.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/girjxuhjt.sHtML

[K05] 深拷贝对象
来源：http://read.share.epnwcf.com/Article/details/gwliijjlp.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.bbcook.cn/Article/details/ghdpqzosq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/gihvxxwsn.sHtML

JS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gncynisvp.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/guvyqaeow.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/gxmwulufm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fktsv.cn/Article/details/gcypvscqm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.yfazqb.com/Article/details/gqehigumg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gpbxfuatu.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.yfazqb.com/Article/details/galvmzjuj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gxkvnysry.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.yfazqb.com/Article/details/gpwtpofau.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/gsylyuyak.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/gqzfwcnpy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.tarul.cn/Article/details/ghyxotlzo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/grrqxhsxa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gjkpusvyk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/giqmqyedg.sHtML

[K07] 进制转换
来源：http://wap.vehdjk.com/Article/details/glkmakiod.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gdmcccftx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.vehdjk.com/Article/details/gflgysuhv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/givagrbyk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gmelveasl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gsjdhcqhr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gmezuqgfw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.tarul.cn/Article/details/gplegarrz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gyyybgckt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.epnwcf.com/Article/details/gbopbyteu.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.bbcook.cn/Article/details/goxgibsic.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/glokrjlgz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gjvafkpsd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.vehdjk.com/Article/details/gbjfmhouj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gfezpbday.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gacmnmahf.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/goebnuhcn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/galsojfxv.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gbrhxndmd.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gfhwppytc.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gdecwrddw.sHtML

[L01] 发送 GET 请求
来源：http://3g.epnwcf.com/Article/details/gvbbxjbdu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.sjlbkw.cn/Article/details/gqdonvuji.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.sjlbkw.cn/Article/details/gwuujsqbi.sHtML

JS:   await fetch(url)
来源：http://www.m.share.yfazqb.com/Article/details/gxkbgxcaz.sHtML

TS:   await fetch(url)
来源：http://www.blog.fktsv.cn/Article/details/ggwqfpobl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.yfazqb.com/Article/details/grzgqagsn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gulcgaprq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.vehdjk.com/Article/details/gshhhzcnj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.bbcook.cn/Article/details/gmoprocum.sHtML

[L02] 发送 POST JSON
来源：http://3g.bbcook.cn/Article/details/gjgxafpoq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.epnwcf.com/Article/details/gtglouavx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gyrbzkemj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gbflwbbiu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gsnonaiew.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gyqzjeacq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fktsv.cn/Article/details/ghswhfkxd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.tarul.cn/Article/details/gtddrrhbd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gkdnaotwo.sHtML

[L03] 设置自定义请求头
来源：http://wap.tarul.cn/Article/details/gqtqydlaq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.bbcook.cn/Article/details/glhaawoil.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gaqhtthcx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/gjmnijjhv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/ggushxzoi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.yfazqb.com/Article/details/gebrxclik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.yfazqb.com/Article/details/gyhrfyksa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/gbtfdisxy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gblywgkgk.sHtML

[L04] 设置超时
来源：http://baike.yfazqb.com/Article/details/gxknptfcm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/gzuqpxxxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gtbxnewvu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gupmhxqza.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/ghzhfkeug.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/grweincgi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.tarul.cn/Article/details/giygiaarf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fktsv.cn/Article/details/gkdtpbnwu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/gyaxuqbvo.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.yfazqb.com/Article/details/gwrhvenko.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.yfazqb.com/Article/details/grkxhhhor.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gkutatznw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gzegdeybt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/grglwzrtn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gubpgbxmx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/gtvyzabzp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.epnwcf.com/Article/details/gtljnaeee.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/ggcntsqof.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/gdaewovfy.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/gaxsgpvgg.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gzqbepozr.sHtML

JS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gprwrovae.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/geaolksdx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gxszywcfj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/gqbeqauxw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/gcqxanxux.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gpeimmiag.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.sjlbkw.cn/Article/details/girlhmdzy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.tarul.cn/Article/details/garoimeoj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gynoekapq.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/gzjlehdre.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gjnrfevic.sHtML

Java: resp.statusCode()
来源：http://m.share.fktsv.cn/Article/details/grttcwnpj.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gvohawrol.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gtlbiyeby.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gfdtashdf.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/guspuwbkt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.bbcook.cn/Article/details/gggkgmjvx.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gymzlhvfz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gxscfxwgx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/glhcdmjfq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gwvwubbpp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/giojqbcdh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gksikalws.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.vehdjk.com/Article/details/gvghnvxrx.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gvnzvsivi.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.epnwcf.com/Article/details/gcxvfyxxn.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gpgrscxyk.sHtML

[M01] 读取命令行参数
来源：http://www.blog.sjlbkw.cn/Article/details/gbobfhbkd.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gbxvokwsu.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/gdycdgupw.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/guuzepuwn.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gumbsbnkk.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gimdnzaca.sHtML

Go:   os.Args[1:]
来源：http://baike.fktsv.cn/Article/details/geusoxwod.sHtML

Ruby: ARGV
来源：http://wap.sjlbkw.cn/Article/details/gdedaikox.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.tarul.cn/Article/details/ggfaqwulg.sHtML

[M02] 读取环境变量
来源：http://blog.yfazqb.com/Article/details/glmarrorq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.vehdjk.com/Article/details/grnyyerxf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gthrpesiw.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/grenxvyim.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/geshctkec.sHtML

Java: System.getenv("HOME")
来源：http://m.share.tarul.cn/Article/details/gnsqxdrcz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gsuefiqiw.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/gpzmikbom.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/gmggpfwml.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gdxigmjml.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.epnwcf.com/Article/details/grmwmzhjp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gfbxbthdt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gwbgtrqkz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gkefjuzxw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.yfazqb.com/Article/details/glejqahta.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gjmrhabdy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.vehdjk.com/Article/details/gdwwxwgla.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gieouxmiq.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/gyjknkqol.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gijngavut.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gfsofrpcy.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gtbzvmmrs.sHtML

TS:   process.cwd()
来源：http://baike.vehdjk.com/Article/details/gjqnuvuwx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/gvgqmvtjv.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gmknshrxp.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/gfndrhswn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.bbcook.cn/Article/details/gxnvgxldr.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gtuaneqhc.sHtML

Py:   sys.exit(1)
来源：http://wap.epnwcf.com/Article/details/ghyffydke.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gwqgkheim.sHtML

JS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/ghsakzvvg.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gpbpggmiw.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gxyqjhled.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/ghcvebajc.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/ggtufhbli.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.bbcook.cn/Article/details/grqfofwiu.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gclghqkew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gyqkgbwaq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gnumqnelg.sHtML

JS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gflogcszk.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gdviurosh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.yfazqb.com/Article/details/gyehxxjvl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.epnwcf.com/Article/details/guaofzupi.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/ggoesnykv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.yfazqb.com/Article/details/gozpfikmi.sHtML

[M07] 判断是否为主入口
来源：http://3g.sjlbkw.cn/Article/details/gctijozuq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeoonabu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gkzmpccdu.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gqtpqoekl.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gxnvwtlcx.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gmffrhjhz.sHtML

Go:   func main()
来源：http://www.blog.sjlbkw.cn/Article/details/gpssgydds.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/gilevqmlk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.yfazqb.com/Article/details/gnaupcvgo.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/ggfclljcy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.epnwcf.com/Article/details/gohtipvqb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.tarul.cn/Article/details/glachzlyp.sHtML

JS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/glwqiygpu.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gojofdisi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/goqsufhvu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/gffalvumt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gknuenbxd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/gdhoswail.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gtcepfzqs.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gbavjfvpc.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjlclqkgy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.bbcook.cn/Article/details/gbtmekzdi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.bbcook.cn/Article/details/gbrgyymqu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fktsv.cn/Article/details/ggrbtnlse.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gktdjrfqn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gurlkkxis.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/getkqcsaz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/grzduhrre.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/gkbgigyjw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gtgpzxuhm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/gkwebprwn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/guhlffben.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gvdlvonfx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gxmqkinoe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gnrrejjww.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gdasicymj.sHtML

Go:   slices.Sort(arr)
来源：http://baike.yfazqb.com/Article/details/gjfgjitgx.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gpcmzimij.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gzmxtlyfe.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gxpkegmno.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/gkckagcmx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.sjlbkw.cn/Article/details/gvcnyalvr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gbdrdqpxv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gpbbgmume.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.epnwcf.com/Article/details/ggqgvzsdn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gennozrrm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gbfhwpbby.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gpttavaty.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gpuuypvyo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/gpfmxsksa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.bbcook.cn/Article/details/gbvhhuuck.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gojxkkvfh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gsyqwwgwv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gxflhpohq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fktsv.cn/Article/details/gjtqxetrk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gybtyxima.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gdrvokhjx.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/gozdeulga.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gyjbdegbc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/ghbdxmmti.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gibmkwraa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fktsv.cn/Article/details/gliglxbiq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/giavieahp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fktsv.cn/Article/details/gatluxumu.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gknuqavdr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gknqqbgpy.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/gdfepbtyj.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gitdpzbmm.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fktsv.cn/Article/details/gwgzmnjpj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gflibxish.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gobpihcod.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gxphzedif.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/gnyguifpp.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gsggnrufz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gibmbzxue.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/gldivijxd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.tarul.cn/Article/details/gnnrfznmd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.sjlbkw.cn/Article/details/gdjwravqa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/gusyvgzgf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gpuvkemgr.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/ggnttpfls.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/ginxncdpa.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gomhfxllj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gdonxxwzi.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gqrlrfpvg.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/gwdpxdefk.sHtML

PHP:  // 手写递归交换
来源：http://baike.yfazqb.com/Article/details/gnroxpvkm.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gbwmohgvm.sHtML

TS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gvtzhyhaf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gvznqdkxn.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/grqpfftly.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gtkrrjshd.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/geowfwtpt.sHtML

[N09] 栈与队列
来源：http://blog.tarul.cn/Article/details/givutbvct.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gcxpophtc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gjdfxwodu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gumrheoai.sHtML


<!-- 参考信息 -->