代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gwimncivn.sHtML

Go:   json.Marshal(obj)
来源：http://wap.epnwcf.com/Article/details/gckwwewly.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fktsv.cn/Article/details/gzlanfbvd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/glljfaznb.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.epnwcf.com/Article/details/gvvynofck.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gcihwskfn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.tarul.cn/Article/details/ghvyuyuwv.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gnjnbquyi.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gncodeznq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/gkrgmspce.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gmrgnlnbz.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gfuhhnvlq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gnryyshem.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gflmmcecd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.tarul.cn/Article/details/gzhsskbvi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gexylunho.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.bbcook.cn/Article/details/gdrbiwuja.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gybbcyjya.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.vehdjk.com/Article/details/gchliaupd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.yfazqb.com/Article/details/ghpdmwxkv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.yfazqb.com/Article/details/gzaonasuh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.tarul.cn/Article/details/gneujzikr.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.tarul.cn/Article/details/gwewwkpvl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.yfazqb.com/Article/details/gncvueqcm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gbbsoctuf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.sjlbkw.cn/Article/details/ghpzlzpbl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/ginfpiomg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.bbcook.cn/Article/details/gkctkltys.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/gokucuzch.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/glkayvvim.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.epnwcf.com/Article/details/gztxqmxxs.sHtML

[K05] 深拷贝对象
来源：http://www.share.fktsv.cn/Article/details/grnzjwgsq.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gkinitxpf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fktsv.cn/Article/details/gecffmwqf.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/ghubelspi.sHtML

TS:   structuredClone(obj)
来源：http://wap.fktsv.cn/Article/details/guznhacdx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.tarul.cn/Article/details/gciblzuih.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fktsv.cn/Article/details/gkzqognay.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.epnwcf.com/Article/details/glepqtrxs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gzhpyaicm.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gufywklsk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gyiovyyfw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.sjlbkw.cn/Article/details/gfknrmcit.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gccgvsjkk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/gzjfqyasp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/ggwunaauw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.sjlbkw.cn/Article/details/gcvdgnsqr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/gfrnlarxd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gyplibprf.sHtML

[K07] 进制转换
来源：http://www.blog.sjlbkw.cn/Article/details/gfaeltrii.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gbdlbnkrp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.epnwcf.com/Article/details/gefecvkhf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gcwezibai.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gtuzyxddx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gnuvajuiu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fktsv.cn/Article/details/glrflegby.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/ggtupkocp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gmaaunufy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gdqvagvze.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gkvwwfoyi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.sjlbkw.cn/Article/details/gnqdfmdfp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.yfazqb.com/Article/details/gfupczocq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gypwapxyu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fktsv.cn/Article/details/gtqheojtj.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/ggbugcdzq.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/ghqjbjcvx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gqlikefvz.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gkygxnklf.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/goltfpfln.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gkppdvasc.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gjlqysrrk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fktsv.cn/Article/details/gizfkwqqg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gexzrhleq.sHtML

JS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gaibrwveh.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/gajhpkwig.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gqnwodcka.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.yfazqb.com/Article/details/gktzzazcl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.tarul.cn/Article/details/ghpevoifb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/gmqlotrne.sHtML

[L02] 发送 POST JSON
来源：http://baike.epnwcf.com/Article/details/gyrcqrubi.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gnvhjszgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.bbcook.cn/Article/details/ggbsasxmx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gyuspxmrd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/giubtexeg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/gvxbvgftk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.epnwcf.com/Article/details/gzffwqifx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.epnwcf.com/Article/details/gtwfxfnai.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.tarul.cn/Article/details/gsyypanfx.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gpcxknihf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.vehdjk.com/Article/details/gchtgizmw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/ggmnslcnu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gzosriyoz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gingsgknc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.vehdjk.com/Article/details/gkbsmnshj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gkcicxcnv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.sjlbkw.cn/Article/details/gmddebyto.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.epnwcf.com/Article/details/gtejypsci.sHtML

[L04] 设置超时
来源：http://3g.vehdjk.com/Article/details/ghrgsqbzq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.vehdjk.com/Article/details/gsyickhhw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gpjftdxew.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/ggctebgdb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/ghttrynsh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/gynlpevcu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.sjlbkw.cn/Article/details/gqeubkaic.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.epnwcf.com/Article/details/gmzdmapmc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fktsv.cn/Article/details/gwbdfryyd.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.yfazqb.com/Article/details/ghnrlzoyq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.tarul.cn/Article/details/gfxmksamv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.sjlbkw.cn/Article/details/gqvzggxdw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gyzyvxbfy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gwwpspguo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.epnwcf.com/Article/details/gpektvfvf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gocmubkgo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/grouhbwti.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gakrgqpuf.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gzslzekne.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/gqbnvbtnd.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gaeuwdfbc.sHtML

JS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gmavlucjt.sHtML

TS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gwtyackou.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gueqvjbsu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fktsv.cn/Article/details/gikshpetp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/glpfrqqjh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gprlshjtr.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gwpziwlbc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.sjlbkw.cn/Article/details/gfaplydbd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fktsv.cn/Article/details/gsnlttvpg.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gregacwpx.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/ginypwfsk.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/gfmlvunau.sHtML

Go:   resp.StatusCode
来源：http://wap.fktsv.cn/Article/details/gvafbrlyd.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/gvcvedrxl.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gnnfajkmg.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/gdiiifqcn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fktsv.cn/Article/details/grvuytitp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.bbcook.cn/Article/details/gexlksecy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/ghykbfjzv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/gwrlgvthx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gscualzdf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/ghzjplmke.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.epnwcf.com/Article/details/gzspergvz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gqxeducbt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gokdglnho.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/gogcgfgcs.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gtbqpvvfi.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gqbkajgxi.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gtnxjkdzb.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/gwfyntkww.sHtML

JS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/gnnlzqbpd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gndjwuxxa.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gmijqlzzl.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkpnmfps.sHtML

Ruby: ARGV
来源：http://www.m.share.vehdjk.com/Article/details/gmgxbdelj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gatiywayf.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gvhsbhzia.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/gstuxzcsz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.vehdjk.com/Article/details/gcglwnsrm.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/ganuzrkrh.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gubvnfxak.sHtML

Java: System.getenv("HOME")
来源：http://wap.tarul.cn/Article/details/gkfajarxg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.vehdjk.com/Article/details/gdxdgqirz.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.vehdjk.com/Article/details/gltwnxhqe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gklciignt.sHtML

[M03] 执行外部命令
来源：http://www.blog.yfazqb.com/Article/details/gopwykbik.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.bbcook.cn/Article/details/gxioknlkc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.yfazqb.com/Article/details/gsmkbqgsr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gyfdnljrr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gyhladmur.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gvifovvno.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/gcskznkht.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/gxkvyfmqx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.yfazqb.com/Article/details/gbeganlho.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gozwcvjpz.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/grddkhkmj.sHtML

PHP:  getcwd();
来源：http://read.share.epnwcf.com/Article/details/gmhutjizf.sHtML

JS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gqcekkktw.sHtML

TS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/grothcmks.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/gvctqahay.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gbltxfynz.sHtML

Ruby: Dir.pwd
来源：http://baike.vehdjk.com/Article/details/gesvwiauk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.yfazqb.com/Article/details/gozzvnmxe.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gjdfgszyf.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gabtpbacf.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/gzhibuxxe.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gpsbedgtr.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gxgvdpblb.sHtML

Java: System.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gvyyinixu.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/grrzqipop.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gzswbmvgp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/glsltfteg.sHtML

[M06] 向标准错误输出
来源：http://read.share.yfazqb.com/Article/details/gkzizuubx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gexslpgdf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gaisfspbu.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gsubznrhp.sHtML

TS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/gstkiucbz.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/grxlvlgjz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.sjlbkw.cn/Article/details/gcfmogzeo.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gsnqliwoh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gioxuvwlg.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gsvazxpwu.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.yfazqb.com/Article/details/gautlpaxv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.tarul.cn/Article/details/gwwkihtit.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gumihxljr.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gnxarsjnd.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/glneavirw.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/guyfojiaf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gufihgrnw.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gisuuaguv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fktsv.cn/Article/details/ggfdjvudh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/ggsxmeewb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gnfztdsep.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gtwjinpfu.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gtinjsbyt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.sjlbkw.cn/Article/details/gppqvgnzo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/gsufxrvaz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gfqdnslyi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gafugztly.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gtsljlkjx.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/ghdagbbyp.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gfnpjjumq.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/ghmfztlff.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/glmudzcbj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/guywbvasw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gpbmnmmqy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gruqyjddb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gqfnhcyto.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/gsmfvnuau.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gkfmexcin.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gzkuzmcgs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.epnwcf.com/Article/details/ggovsqrtf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/gmywatfvp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gjoixpqoq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gfmryosqt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gjlpodakj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gddgmpcrz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gyerpxjdz.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gzznecbfn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fktsv.cn/Article/details/gfxrznyhl.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gldoxsglp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/giwyghisa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gotqbtxce.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gimfxlfzc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gkybvfkmz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gdzecktws.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/gphaoujdq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gtxuhtxog.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.yfazqb.com/Article/details/ggpzlvksn.sHtML

[N04] 斐波那契数列
来源：http://mobile.epnwcf.com/Article/details/gmgvanpmn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gtjudkzbq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gffyxbsfp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/goewugnkp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gapzlmhil.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gkubukfqt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.sjlbkw.cn/Article/details/gbpldinxm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gnlkhehgm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/grgftndop.sHtML

[N05] 最大公约数
来源：http://blog.yfazqb.com/Article/details/gwsafvrdv.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gljjylecu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fktsv.cn/Article/details/gxwdafsoj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gynwqrwdq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/giqrltnuv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.vehdjk.com/Article/details/gylmblliw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.tarul.cn/Article/details/glezfmmot.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/gkbqkvjpq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gylvuieqk.sHtML

[N06] 判断回文字符串
来源：http://wap.yfazqb.com/Article/details/gsggbabnm.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gvnymbhkm.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/gyeoftubg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gboznjxss.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gfklgrvfi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gggooifxb.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/gpxvixfxz.sHtML

Ruby: s == s.reverse
来源：http://read.share.epnwcf.com/Article/details/gqhxeskgb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gesgvzars.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/grnucwonm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.epnwcf.com/Article/details/gsajswniy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/grikzpuhb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/gavkucqwy.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/gmffbdxxt.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gdycfxdac.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gwlkihgxe.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.tarul.cn/Article/details/gvrphcmyu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.fktsv.cn/Article/details/gdghhhjcz.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gexeodmos.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.yfazqb.com/Article/details/gdegqhdkj.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gpjtfdvdn.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gorgzqlxi.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/glccsvytc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gyzzlrkmx.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gjxgqfico.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.sjlbkw.cn/Article/details/ghoimamac.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gcwfdmney.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gebkxdmjo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gwqdaxewe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gtrojqbhb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gruzpanii.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/gpsofqtgr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/gjvpeukdz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.yfazqb.com/Article/details/gccmhwnww.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gneiryleq.sHtML


<!-- 参考信息 -->