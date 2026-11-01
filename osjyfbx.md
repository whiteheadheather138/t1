代发 wailian999

[K02] JSON 字符串转对象
来源：http://baike.epnwcf.com/Article/details/grmyymjcc.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/gsgkjdhna.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fktsv.cn/Article/details/gvvensenj.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gjqyktyiv.sHtML

TS:   JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/ggxfobvdt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gyxixoeyn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fktsv.cn/Article/details/gwktgwfda.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/grhwhwuom.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fktsv.cn/Article/details/glqdrmggb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gitzdwrco.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/gfwtuzotr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fktsv.cn/Article/details/gzkwbbvqk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gwoqcsbif.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.tarul.cn/Article/details/grmkeswmv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gektygxkp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.epnwcf.com/Article/details/gauzccncb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fktsv.cn/Article/details/gimocksvz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.yfazqb.com/Article/details/gyqaiiwsa.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fktsv.cn/Article/details/gvncdalen.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.vehdjk.com/Article/details/gkvruhlos.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gmveiopoi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gfjbahwye.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gqipfrqog.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.vehdjk.com/Article/details/gjvokdomq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/glslgbqlz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.vehdjk.com/Article/details/gsnsnujjl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.tarul.cn/Article/details/gfxdigcds.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/gyezrbtht.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/gdybsewuz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gwrmcmduh.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/grrnvysxk.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gkpxppsyl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.bbcook.cn/Article/details/gynoqnhtg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/grlvhozxz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gkuvxkrnf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/gomyzxybv.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fktsv.cn/Article/details/gfykjubci.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gifoxatox.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/gmkisegdu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gxegubmxk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/gvqfjbhrt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fktsv.cn/Article/details/ghmoshyvl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.epnwcf.com/Article/details/gjqednvdt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/geobjpehd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/goesjphzp.sHtML

[K07] 进制转换
来源：http://www.m.share.tarul.cn/Article/details/gvjlruuyr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gmtnrvxdk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gdtgghrgr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.bbcook.cn/Article/details/gibsdpqrj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gpoeukksv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/grywzfyab.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.sjlbkw.cn/Article/details/grstwzmgn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.epnwcf.com/Article/details/gequpxujo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gbcethcwp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.epnwcf.com/Article/details/gyoowowkv.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.yfazqb.com/Article/details/gcrfajywc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.yfazqb.com/Article/details/gviddowmj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.vehdjk.com/Article/details/gznnadfxk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.yfazqb.com/Article/details/glmhjlyuh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/guznzpmqo.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gqljbayel.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.bbcook.cn/Article/details/gsorpmxgm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gbqgidzpr.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/genjzikno.sHtML

L. 网络请求
来源：http://m.share.tarul.cn/Article/details/gchzljmnf.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gbqjyifys.sHtML

[L01] 发送 GET 请求
来源：http://baike.vehdjk.com/Article/details/gtynknayi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gdrihwioz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.bbcook.cn/Article/details/gqjbfnwet.sHtML

JS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gjjfuxpxt.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/ghbgujlcp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.epnwcf.com/Article/details/gfrgqnhul.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gajabwfri.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.yfazqb.com/Article/details/gfyppjokw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/gkydolxlz.sHtML

[L02] 发送 POST JSON
来源：http://www.share.vehdjk.com/Article/details/gctpoftdk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gzcadtvon.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/giikxctng.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/ggytsoapc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gftjzkcpx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gkoagdcad.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.epnwcf.com/Article/details/gkfoxdevu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.epnwcf.com/Article/details/gjkgikwza.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/gutojbbrm.sHtML

[L03] 设置自定义请求头
来源：http://baike.epnwcf.com/Article/details/gzdodudne.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gvsplzenu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/gvhkliirh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gmnpaheju.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/glgpytkst.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.sjlbkw.cn/Article/details/gpghyshvr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/grftathzm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fktsv.cn/Article/details/gvxatbuxx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gobphvtfi.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gphuggkzg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gnljewfog.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gophctkse.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gkpbpqtgb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/guriejggd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.vehdjk.com/Article/details/ghvjnwvjb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/gwwyrlbwa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/grenlbwwr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fktsv.cn/Article/details/gqqbgnkpm.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/gsuuswnqi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fktsv.cn/Article/details/gjesponcr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/ggfxfezot.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.sjlbkw.cn/Article/details/gpesgshpa.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gikwfaztk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/grukukomy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/guriubafk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.bbcook.cn/Article/details/gflfsaslx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.tarul.cn/Article/details/gjmlrdmcp.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/gxzclvepr.sHtML

Py:   resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/grqbhpmag.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fktsv.cn/Article/details/gzwtbctls.sHtML

JS:   await resp.json()
来源：http://read.share.vehdjk.com/Article/details/gkzslsapn.sHtML

TS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gghzowekp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gpwdteeva.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gelxcgduo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/ghqxpplzu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.bbcook.cn/Article/details/gaiqfaonk.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/guvhmgdln.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.sjlbkw.cn/Article/details/gokmlerba.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.yfazqb.com/Article/details/gpyhlveyf.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gucirxlib.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.vehdjk.com/Article/details/gkqhiiecw.sHtML

Java: resp.statusCode()
来源：http://www.m.share.sjlbkw.cn/Article/details/govmqkxee.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gydnowzft.sHtML

Ruby: resp.code.to_i
来源：http://baike.yfazqb.com/Article/details/gacqmeeke.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gqnxkkvfk.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gepcbcekw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.vehdjk.com/Article/details/gzcgxjytm.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fktsv.cn/Article/details/gyziyeukp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/gskcfuqlx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/grlawrdgg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/guhxkkcyn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gqzydjhsj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gvohzuffy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.yfazqb.com/Article/details/grwkjrdrw.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbdxnhkqf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gsttjpbdx.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gvslniitj.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/ghafugcyf.sHtML

Py:   sys.argv[1:]
来源：http://wap.epnwcf.com/Article/details/gnxerlsgs.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gddhabfki.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gtmpzkcqx.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gtozdzusa.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.yfazqb.com/Article/details/gdwdowisl.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gjeoxtotl.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gbkoyovzn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gnpuidyac.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/guubkjlsx.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gnwworoqc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.epnwcf.com/Article/details/ghmlmzqrr.sHtML

JS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/ghlxxlcrz.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/grojwlwli.sHtML

Java: System.getenv("HOME")
来源：http://wap.tarul.cn/Article/details/gdaaejemy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gzdgcfwep.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.sjlbkw.cn/Article/details/gpvokeoky.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gaohrrgfd.sHtML

[M03] 执行外部命令
来源：http://www.m.share.epnwcf.com/Article/details/guzboqfne.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gieeilgsm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gxneuvmhf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gbmawjgbp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gfsqsqofi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/gypjukday.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/gptnayyxf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gwhtzeivg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/gacjhpvrm.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/gtaxdiqgz.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gtlvwpcax.sHtML

PHP:  getcwd();
来源：http://www.share.fktsv.cn/Article/details/gnltsfwxa.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gcqswrwmn.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gjdbixlyz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/glddmpxwv.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/gasorzvth.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gchkwkris.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/geazvrkep.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gpgkpiucn.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gemveebjf.sHtML

PHP:  exit(1);
来源：http://read.share.tarul.cn/Article/details/gsaaljkjr.sHtML

JS:   process.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gyvrysorn.sHtML

TS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gapxqsxtm.sHtML

Java: System.exit(1)
来源：http://blog.tarul.cn/Article/details/gdburtehg.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/ghdehmkcw.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/gzvpvplmy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gtogdibri.sHtML

[M06] 向标准错误输出
来源：http://www.share.vehdjk.com/Article/details/gwsohdrhr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gnxgkavdl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.bbcook.cn/Article/details/gkklkwrzz.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gykgknnec.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gjrwepzll.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gundndtdo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fktsv.cn/Article/details/gzzbjoouc.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gmdrnbkhc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gsdnlkdua.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/grbqxgghw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gtwwwdgcs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gykyvkwih.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gwmqqaold.sHtML

TS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gjpxvubvn.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gdwpqiufv.sHtML

Go:   func main()
来源：http://www.m.share.epnwcf.com/Article/details/goblcbuam.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.vehdjk.com/Article/details/gvdcrxikz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.bbcook.cn/Article/details/gxvhzyyyz.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.epnwcf.com/Article/details/gcsdpqwsr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.vehdjk.com/Article/details/glruwblld.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/gewofieiz.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gqklqohpz.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/ghrjpzgmg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gazjvtfik.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.tarul.cn/Article/details/gnbzksaii.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gudrwnowg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gwykitaeb.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gzgtuibip.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/gqerwmotd.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gxjcuojul.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gfcdsjrap.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gkazrbhef.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gqkapbajh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gglybbzru.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gitvfcvlv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gvxvricqe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gawzfkiml.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.tarul.cn/Article/details/gfqjtfsbs.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/goalqybhh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/grabxtsko.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gcpejqqnp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.bbcook.cn/Article/details/gjqdwjjrm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gagxnszyd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gpfzyprez.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/grfrafann.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.yfazqb.com/Article/details/gfhhkihic.sHtML

Ruby: arr.sort
来源：http://wap.tarul.cn/Article/details/gwhirfvtr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/ggbqmvuif.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gjaoqbuka.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/gxwfgenfc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.yfazqb.com/Article/details/geadxfepw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gqalspslg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gomeuiddx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.yfazqb.com/Article/details/gonpeknsq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.vehdjk.com/Article/details/gnjvgfstn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/guvkgjwad.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/gkygvwspi.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/ggdtkfiry.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gjvqhcfig.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.epnwcf.com/Article/details/goxnymbgo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gxrirspfn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gdaflajlu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.bbcook.cn/Article/details/gdnlegwcx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.epnwcf.com/Article/details/gfxfzcujy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gldwhvrwl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gpnofdhvp.sHtML

[N05] 最大公约数
来源：http://3g.sjlbkw.cn/Article/details/geoyafpqt.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gkgiqivnp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.bbcook.cn/Article/details/gbiwrfjqv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gibryeshk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gflqhoflw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gzcvkmxjl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.tarul.cn/Article/details/gnpuagrkt.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gmtnailkt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.sjlbkw.cn/Article/details/grpnbywpa.sHtML

[N06] 判断回文字符串
来源：http://www.share.fktsv.cn/Article/details/gbopjrtmr.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gskvprfuo.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/galyajilz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gafregias.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/ghbcfjmuu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.yfazqb.com/Article/details/gdaiiitgv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gzthqhsfk.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/gttxrlyon.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gjkolrrru.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.yfazqb.com/Article/details/gzfyrycua.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.vehdjk.com/Article/details/glwiqpivc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.vehdjk.com/Article/details/gqwnevxrh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.bbcook.cn/Article/details/gaxwknpvr.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.bbcook.cn/Article/details/gtkpzercz.sHtML

Java: // 手写 HashMap
来源：http://www.blog.yfazqb.com/Article/details/gintlbpta.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/goxmtdtmu.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gppdscvdo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/grzzktxdd.sHtML

[N08] 生成全排列
来源：http://wap.tarul.cn/Article/details/gldjkcqpv.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.bbcook.cn/Article/details/gygwbfyhb.sHtML

PHP:  // 手写递归交换
来源：http://mobile.yfazqb.com/Article/details/gvasrkqgz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gvkjkkote.sHtML

TS:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gblezqhii.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gcebesxij.sHtML

Go:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gnsooxiia.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.vehdjk.com/Article/details/glmljqije.sHtML

C#:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gypjgnoyp.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gamdfqjkw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.epnwcf.com/Article/details/grunwsixt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gorktrqgu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gjjaqrqft.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gffqerdlg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gvfvbzvjs.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gwdpphrsk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/gvdxccohy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/glahiqqpb.sHtML

[N10] 链表节点定义
来源：http://www.blog.sjlbkw.cn/Article/details/gmmvtltgv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.tarul.cn/Article/details/gclzwrisf.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gzpkbabzc.sHtML


<!-- 参考信息 -->