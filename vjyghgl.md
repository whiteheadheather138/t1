代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.sjlbkw.cn/Article/details/gpkleusyt.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.bbcook.cn/Article/details/gqtdcthdv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.yfazqb.com/Article/details/gcopjnwfe.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.epnwcf.com/Article/details/ginlncbvj.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.tarul.cn/Article/details/gmlelfjaf.sHtML

Py:   json.loads(s)
来源：http://m.share.yfazqb.com/Article/details/gvdxusssl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.sjlbkw.cn/Article/details/gwerqbnfb.sHtML

JS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gsjfiyvzb.sHtML

TS:   JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gynkeyfct.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/gjrhsfngz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/ggcomceou.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gwhtekkbh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.sjlbkw.cn/Article/details/gwxxzkbrh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gngpccxro.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gxghunqva.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gyxbkzsrr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gdiwpcxeq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.epnwcf.com/Article/details/ganiiteyt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwpospqog.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.bbcook.cn/Article/details/gwwwplvav.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.vehdjk.com/Article/details/gbmiwzyxy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.sjlbkw.cn/Article/details/gvsbxggpg.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.bbcook.cn/Article/details/goizszjey.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.sjlbkw.cn/Article/details/gkdgozsxo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.sjlbkw.cn/Article/details/giyxzsaeq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.bbcook.cn/Article/details/gphrppfqi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/ggyvyxqva.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/gjmgzkule.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/ghvvpvqlz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.tarul.cn/Article/details/gqeuywuqb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/giaphpvdf.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gbrelqomn.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gmexemwzd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fktsv.cn/Article/details/ghettynvw.sHtML

JS:   structuredClone(obj)
来源：http://wap.tarul.cn/Article/details/gaosrjayo.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gbfeltqeh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.bbcook.cn/Article/details/gewzhbdoz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gxpwnkxek.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/guavxzhwa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.tarul.cn/Article/details/gqetqfzth.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gimtatocb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/gvmcpeinx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.sjlbkw.cn/Article/details/gbcvthycc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fktsv.cn/Article/details/gnkhkruir.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.vehdjk.com/Article/details/gyshvhtxp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.epnwcf.com/Article/details/gpesixszn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/ghkijfzop.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/geauboxbm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gltlvbnrd.sHtML

[K07] 进制转换
来源：http://blog.tarul.cn/Article/details/ghddvbolt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/ghmnjelan.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gbglnulzv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gyrtuihpx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gfnolvjuw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gujesdcnf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gqbkmsjme.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.bbcook.cn/Article/details/gwrlzamim.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gbzhrgkyd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.yfazqb.com/Article/details/grltqcbiy.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.vehdjk.com/Article/details/gehvubekn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/ghobsbumt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.vehdjk.com/Article/details/gmqolrwpn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.tarul.cn/Article/details/gnqipzodm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.bbcook.cn/Article/details/gwrjxrqww.sHtML

Go:   encoding/gob
来源：http://3g.epnwcf.com/Article/details/guxdwqtdn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.yfazqb.com/Article/details/guhtjuctf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.bbcook.cn/Article/details/gnbqhejmc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gybjhexiu.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gwmfnajpe.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gbdqxxzkq.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/gjrskqsnj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gnslsoyde.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.bbcook.cn/Article/details/gwaserbhd.sHtML

JS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/glnrjfxln.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gzyzlmynw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.epnwcf.com/Article/details/gpjhwaswi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.epnwcf.com/Article/details/gjujqdopc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.epnwcf.com/Article/details/ggmjcbtsl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gaonotmuq.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/gitdwklao.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.sjlbkw.cn/Article/details/gsgpcbxbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.bbcook.cn/Article/details/glqokkqak.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gklqbojbx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gwtldwctp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gmgownrcd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.vehdjk.com/Article/details/geilzeozq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.epnwcf.com/Article/details/gqrmcerxf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gmhmszqty.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gkzuruvsy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.yfazqb.com/Article/details/ghgwanuev.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.tarul.cn/Article/details/gouhtjlpz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gtwstfdgg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gfpyxivto.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/gifaweaxc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gduwqxxag.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.bbcook.cn/Article/details/gfnpgbbpw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gblhijaxq.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gdziqnlme.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.epnwcf.com/Article/details/gainkujtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gyvphrnyh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/grbwcxeyl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gbmxgykmm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.epnwcf.com/Article/details/gqwntkbde.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.tarul.cn/Article/details/gjcrfvorp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.vehdjk.com/Article/details/gxfbkuqqp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.tarul.cn/Article/details/gzmqwrqjd.sHtML

[L05] 上传文件（multipart）
来源：http://3g.bbcook.cn/Article/details/ghhxvbgcd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.epnwcf.com/Article/details/guzwyrwcf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gvspjkagd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.yfazqb.com/Article/details/gubpjvrnc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gibkqotzd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.tarul.cn/Article/details/gkfppmdyr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.tarul.cn/Article/details/grwjpusxx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.vehdjk.com/Article/details/gfbzfwjdy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.epnwcf.com/Article/details/gaoaostzh.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/ggrbvqmth.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gqaghrpot.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/glyfkbfgx.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gdoqmlnll.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gcmmftxvu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/ghjhlwxfp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/ghoivqlhw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.vehdjk.com/Article/details/glpvbafnv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/gvwobxxof.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/gznvlalkh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.vehdjk.com/Article/details/guzjnfwis.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.vehdjk.com/Article/details/ghivdeapt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gpdivwtyg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.tarul.cn/Article/details/gcunkrtil.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/gjjlxbthu.sHtML

Go:   resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gmtxauwre.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gptuhzcek.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gcjbklwjq.sHtML

[L08] 并发请求多个地址
来源：http://blog.tarul.cn/Article/details/gnythdkor.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/gqlclpiwf.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gtgufcefx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gbtjjrmvy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/ganhbcruq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.yfazqb.com/Article/details/gtunkpdyz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/gxkdedeuu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/giycqygbt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gmjxdbrfy.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwhldegfn.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gkvlstegv.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/genzjznlh.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gbznjiphk.sHtML

Py:   sys.argv[1:]
来源：http://3g.bbcook.cn/Article/details/gszcvhisp.sHtML

PHP:  $argv;  $argc;
来源：http://blog.bbcook.cn/Article/details/gpvgqprci.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.bbcook.cn/Article/details/gsurwfqcw.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gugnxtflq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gznbmfjak.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.vehdjk.com/Article/details/gimedprmo.sHtML

Ruby: ARGV
来源：http://blog.yfazqb.com/Article/details/gzhubmrac.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gjkbqkuko.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/grcckdxdc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gvthsjggj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gunfrqgeq.sHtML

JS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gqzdrqkut.sHtML

TS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gttmfotvg.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gwaozcdqn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.epnwcf.com/Article/details/gskfvbamm.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/gdygjogkk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/ggclgaqtc.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gjuihhxeg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gsfdmattu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.epnwcf.com/Article/details/gxmrkluay.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gtfpaukjl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gfnnadraz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/ghjmgioro.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.epnwcf.com/Article/details/gjozvvhew.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gngrcyppz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gohikdukm.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/gdsjtuezx.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gpjvhdvuj.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/ggguzaivg.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gdbjldumi.sHtML

TS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/ggslenkii.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gxawyncue.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gesbnfiyw.sHtML

Ruby: Dir.pwd
来源：http://read.share.epnwcf.com/Article/details/gswdqtzvo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.vehdjk.com/Article/details/grdpwiszn.sHtML

[M05] 设置退出码
来源：http://baike.bbcook.cn/Article/details/gaxzzpemf.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gvcucglgk.sHtML

PHP:  exit(1);
来源：http://www.m.share.bbcook.cn/Article/details/gbzducqkl.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gaoeugiyl.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gdqnrbiay.sHtML

Java: System.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gxutgkxlz.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/ghoodslmb.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gqrwylqxs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/ggibpmwbj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gbdwcvwnq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.bbcook.cn/Article/details/glzlivpsw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gipxlsilm.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gbsidhigr.sHtML

TS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/gubqjsroa.sHtML

Java: System.err.println("err")
来源：http://www.blog.epnwcf.com/Article/details/gwmtejmid.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gvtjozney.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gsgcrlxta.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gwdqkuwwf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.tarul.cn/Article/details/gepkuysmc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gltypkkzt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/gxetggbau.sHtML

JS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gzwucmeeu.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gnzsbmehg.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/grhhzrfpp.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gjmuigwdt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.bbcook.cn/Article/details/gcyzoqryz.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gbyjpyjvv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.yfazqb.com/Article/details/gncqiohcp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gzlzqgwby.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.sjlbkw.cn/Article/details/getlnntcv.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gnqqvautm.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gqjqkcdzd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fktsv.cn/Article/details/gaxfwrlel.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.epnwcf.com/Article/details/gftnjiegt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gyapksxva.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fktsv.cn/Article/details/gymylsouo.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gchemlhhm.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/gpoofwymh.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gcjwjmolu.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gxkqtqonv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gdahcrytc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gcoqqccfb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/geebdsztk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gjamuukmz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.tarul.cn/Article/details/grvfzqsna.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gevgwfwtu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.yfazqb.com/Article/details/ghtngzhvy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gvjvfxekc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.sjlbkw.cn/Article/details/gyoahajxt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/ghjendqra.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.bbcook.cn/Article/details/gzbkcpusl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gethzcjjy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gdcqfketk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gnqhteein.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gbweotxir.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/ggiqgldlz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/graibaqqv.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/gdmsxcmnm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.sjlbkw.cn/Article/details/gkufledqi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.tarul.cn/Article/details/ghgpmytkz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gyyanupuo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gcewiyjmd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/gihldxxyk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gunpfztmm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gjupdfwbv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.sjlbkw.cn/Article/details/gpgczglcz.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/gfrzqnuwp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gipgonplf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gcjdrqneq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gawklghnb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/ganpfwdpw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/ggdftbxpn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/gpidafouk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/gshkjqajf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gnvecvvvi.sHtML

[N05] 最大公约数
来源：http://m.share.bbcook.cn/Article/details/ggixudfwx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/gvotexkxw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gryrskbvn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gnwrmjpay.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gcflijcjy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gdmzwmfpx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/gnngfzioq.sHtML

Ruby: a.gcd(b)
来源：http://mobile.yfazqb.com/Article/details/gdfyezbrk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gcedcnisx.sHtML

[N06] 判断回文字符串
来源：http://wap.yfazqb.com/Article/details/grjkgcxga.sHtML

Py:   s == s[::-1]
来源：http://m.share.yfazqb.com/Article/details/guamghyif.sHtML

PHP:  $s === strrev($s);
来源：http://blog.vehdjk.com/Article/details/gkltelrxd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gyhdabofi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gmmdsyoqa.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.tarul.cn/Article/details/gerfuetpd.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gzvhickmp.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gpvlyjjyb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gafrvpedw.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.epnwcf.com/Article/details/gurvudujj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gahhzkqen.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gyklpmlzj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.sjlbkw.cn/Article/details/gxgwcfyre.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.epnwcf.com/Article/details/grqadeske.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gkikmkits.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/ggezdrimp.sHtML

Ruby: // 手写 Hash
来源：http://baike.sjlbkw.cn/Article/details/gyspbzrgi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gngiyxxnl.sHtML

[N08] 生成全排列
来源：http://baike.sjlbkw.cn/Article/details/gzvbwkyzc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.bbcook.cn/Article/details/gyxgzylum.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/gyuhagijb.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gmtjlnxrq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/globzkemi.sHtML

Java: // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/geqgjvsgm.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gyxronuhz.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/glchwbjlg.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gvjqowing.sHtML

[N09] 栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gtfmchyew.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.vehdjk.com/Article/details/grhhstbww.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gdcytizbg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.vehdjk.com/Article/details/gdicsldnf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.yfazqb.com/Article/details/gjrujpftu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/gkxcvfxtg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.yfazqb.com/Article/details/ghwgypiar.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.sjlbkw.cn/Article/details/gupxbikuu.sHtML


<!-- 参考信息 -->