代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.vehdjk.com/Article/details/gjniquqxo.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gistqyofx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.yfazqb.com/Article/details/gehlmpeyh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/ghbwunign.sHtML

[K02] JSON 字符串转对象
来源：http://blog.tarul.cn/Article/details/gewalvgjl.sHtML

Py:   json.loads(s)
来源：http://wap.sjlbkw.cn/Article/details/gragypttg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/girnrozjp.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gezybljme.sHtML

TS:   JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gntnkawuu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gwhvuqjqp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.yfazqb.com/Article/details/gxegfulml.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.epnwcf.com/Article/details/gtbvdljbs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.yfazqb.com/Article/details/gplkpqdpo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/grbwvdvsc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.epnwcf.com/Article/details/gkrzzictu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.yfazqb.com/Article/details/gszalzvzc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gxzcdiugr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gsstlmlnb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.bbcook.cn/Article/details/gsmlodxnf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gmgkosetw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.yfazqb.com/Article/details/gppzepoyd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.tarul.cn/Article/details/gksupxvzs.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.yfazqb.com/Article/details/gznryqxyn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.sjlbkw.cn/Article/details/ggxyfqtqw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.tarul.cn/Article/details/gwhchmdfb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gjcxsjbgs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/gsqdsmbkh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.epnwcf.com/Article/details/gzrukjdlb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.tarul.cn/Article/details/gghsjgnia.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.sjlbkw.cn/Article/details/gkgniggyq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fktsv.cn/Article/details/gxkceyfzy.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gmitxdier.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gshsvunvl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.epnwcf.com/Article/details/gsjsiwqsl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gvswjkois.sHtML

TS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gqgleiroi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.bbcook.cn/Article/details/gnnqwjuwc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.bbcook.cn/Article/details/gmvxiwpuy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/glsesuiym.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.bbcook.cn/Article/details/ghmyxrzuz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.sjlbkw.cn/Article/details/gwejaacrj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gwwyyywpl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.bbcook.cn/Article/details/goohryopq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gdmnolcrs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/ghfbxsukk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fktsv.cn/Article/details/geuyovxpr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gewnrggae.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.yfazqb.com/Article/details/ggfelwlot.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gqkaxmrwg.sHtML

[K07] 进制转换
来源：http://read.share.tarul.cn/Article/details/gdvhsyljh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gytpkqsni.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.sjlbkw.cn/Article/details/gyikdfvgu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gvlgzwakg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gyungdpdw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gwdlewbth.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.sjlbkw.cn/Article/details/geuthydsu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gvpunxqmj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/givlgopdn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.yfazqb.com/Article/details/gcilpsxan.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.sjlbkw.cn/Article/details/gvwxmcdrg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.tarul.cn/Article/details/grqubbcyq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.epnwcf.com/Article/details/gnzqgonqz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gzljirige.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.epnwcf.com/Article/details/gulfttqyg.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/gabufaulx.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.yfazqb.com/Article/details/gklxnohwx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.vehdjk.com/Article/details/gmxojtkhi.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/goqowxwsk.sHtML

L. 网络请求
来源：http://wap.sjlbkw.cn/Article/details/gcmslveem.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gwmfqboer.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fktsv.cn/Article/details/gryjlbpps.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.bbcook.cn/Article/details/gtsormuwr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gfckrgcsr.sHtML

JS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/galbmvfmt.sHtML

TS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gjsqsljkl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gmptspens.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.sjlbkw.cn/Article/details/gejqgtfbd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/gkilcpfct.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/gjxipjchv.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/gpwhqdhag.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gbmbcjups.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.tarul.cn/Article/details/gidrdiesf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gvkfwtsei.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fktsv.cn/Article/details/gmamhfbjx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.yfazqb.com/Article/details/gebewtygg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fktsv.cn/Article/details/gcywnlggh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.epnwcf.com/Article/details/glfebdwqz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gcvzpgmpy.sHtML

[L03] 设置自定义请求头
来源：http://m.share.yfazqb.com/Article/details/gkcfzcpmd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.sjlbkw.cn/Article/details/gprfgbusb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gxrlcbayj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/gzjvsiehf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.yfazqb.com/Article/details/getoprcru.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/golazkflb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/glhbzxwtb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.sjlbkw.cn/Article/details/gzgbiyjxc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/golvbnxjw.sHtML

[L04] 设置超时
来源：http://www.share.vehdjk.com/Article/details/gezcpslta.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.tarul.cn/Article/details/gzgmvrfbt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.vehdjk.com/Article/details/gmomglyyf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/ghbgoqvwd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gkangerym.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/glccpsqup.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/ghjieyvfl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gjgimxbif.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/gongfxehw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gttezruhb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fktsv.cn/Article/details/gmknpsnlp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gyzaabroz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fktsv.cn/Article/details/gthdupdpf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/gxegcvnng.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gwshetuqp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/gjuswhccx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.sjlbkw.cn/Article/details/gsffmhlvm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.bbcook.cn/Article/details/gmkwjdgbo.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fktsv.cn/Article/details/goxaqjpqm.sHtML

Py:   resp.json()
来源：http://3g.fktsv.cn/Article/details/gypthhaba.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.bbcook.cn/Article/details/gmocziyqv.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gykcjytbl.sHtML

TS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gfgqhwtuu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/gemzguvko.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gkyjnzvzd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.bbcook.cn/Article/details/gefdgyhlk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gttwimady.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/ggldemaux.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/gpdoitbvn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.epnwcf.com/Article/details/gsaewhjgp.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/getfnadzh.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gicrhialw.sHtML

Java: resp.statusCode()
来源：http://blog.epnwcf.com/Article/details/gpwllfzgp.sHtML

Go:   resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gqfogwgjk.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gbozpflhf.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/galmudhky.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gkbfugqba.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.vehdjk.com/Article/details/goqrhadvu.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.epnwcf.com/Article/details/gltxwicve.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.sjlbkw.cn/Article/details/ghbsnezzh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/gjrbsfdfj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gelimzlvr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gcuecbiln.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.sjlbkw.cn/Article/details/gkyjdbxkf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gxtorsfhd.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkpxfljkx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/gxkedyifj.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gjwcnalnd.sHtML

[M01] 读取命令行参数
来源：http://blog.sjlbkw.cn/Article/details/gteoumugc.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gmzizkbkc.sHtML

PHP:  $argv;  $argc;
来源：http://blog.tarul.cn/Article/details/golvmotrd.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.tarul.cn/Article/details/gkcqboekv.sHtML

TS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gcknhjoak.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gzbijayjz.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gcnvglsne.sHtML

Ruby: ARGV
来源：http://blog.bbcook.cn/Article/details/gvpjuxjxr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gmonkkquh.sHtML

[M02] 读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/gzeeuoflp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.epnwcf.com/Article/details/ghqmdxtlz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gooegpjtm.sHtML

JS:   process.env.HOME
来源：http://www.blog.epnwcf.com/Article/details/gmknrhhoo.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gipzbwwen.sHtML

Java: System.getenv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gadjjyfry.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gygsegfzx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/galkjhrml.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gtwpmcnxv.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/gnubqpcrb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gpwjmtavk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.tarul.cn/Article/details/gtbvwgoym.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gwrnhixsg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/guoqkvxxz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fktsv.cn/Article/details/gbylosres.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.bbcook.cn/Article/details/grctmvgbz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/gdoazsxcx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/gpinnozwa.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gdtdrlwpy.sHtML

Py:   os.getcwd()
来源：http://m.share.bbcook.cn/Article/details/gqdmsrqzp.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/gcrifchwi.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gqgulatqd.sHtML

TS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gwuiupnsz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/gwtorrvbl.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/gylwpoxkj.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gyaaajjpk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gcekypodv.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/gfzcsvdnc.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gktpeskaj.sHtML

PHP:  exit(1);
来源：http://mobile.tarul.cn/Article/details/glyfxgwlm.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/geumuvskf.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gtietoqrs.sHtML

Java: System.exit(1)
来源：http://3g.yfazqb.com/Article/details/ghouikotj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gxyeqcaiu.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gmrqeidfm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/gpjayiznr.sHtML

[M06] 向标准错误输出
来源：http://blog.fktsv.cn/Article/details/gmtilpjvl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.epnwcf.com/Article/details/gytxwdnne.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gnrsaaulm.sHtML

JS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/gjbllwida.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gjiefebfe.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/grbotzyai.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.epnwcf.com/Article/details/grqrjknkf.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gymhfhtub.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gqoeuuxtn.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/guawcfdxu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.sjlbkw.cn/Article/details/gqclhrczy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.tarul.cn/Article/details/gmojmmbmc.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/guyyiuesi.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gkiuugpuu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gfmsztdms.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/gctoehvuq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.sjlbkw.cn/Article/details/gbsqzmqdc.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/glfeumijf.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gjlzkdcyo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.tarul.cn/Article/details/gygdxdags.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gaobpoblw.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gllwpubva.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gttvzjgyz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gpwobselt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fktsv.cn/Article/details/ghyqouyuo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gnpsgguip.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/gnuuetoob.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gqwomfobg.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gvppwbhnu.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbjenjyqs.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/glsniwwlu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gwwoxbejr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gdfbqkajf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/ghyzqivgm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/ghjxshwau.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/glswskdpv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gtezdwrir.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/gawrgwdav.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gwzqzrbfx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gvpwxevgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gpfxexotb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.bbcook.cn/Article/details/gjokwcdpe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gxmkcvbes.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/guybppxlk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.sjlbkw.cn/Article/details/gxoeplqug.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gtispfuzq.sHtML

Ruby: arr.sort
来源：http://blog.bbcook.cn/Article/details/guetlkmti.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gryjzrlrc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gbjamjbgz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gqbviibro.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gatagkfmw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gdijturhy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/gmgtvzvia.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gubdwmeyk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/gstahisnd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.sjlbkw.cn/Article/details/gqlzrmdxc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gwgmzszio.sHtML

[N04] 斐波那契数列
来源：http://3g.sjlbkw.cn/Article/details/gwthcjsyu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gxlmzrodn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.bbcook.cn/Article/details/gpnhcammn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gmoowvkol.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gpetixbsm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gikbftmph.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.vehdjk.com/Article/details/gzcwbndcv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.yfazqb.com/Article/details/gevkzsche.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gjenaxddd.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/ghrbnyqrm.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.vehdjk.com/Article/details/gytkifazn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/glxeuxlho.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gqgcsrnbt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/glqggkajn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.vehdjk.com/Article/details/gxlnbfcsh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/gxaunhcwi.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gnvhwyerj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/grlwxvslc.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/grmujteoa.sHtML

Py:   s == s[::-1]
来源：http://www.share.tarul.cn/Article/details/gacpsquag.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/gvgvkotfh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.tarul.cn/Article/details/gbsqgfrrr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gatgkylad.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.sjlbkw.cn/Article/details/gmzjkvpih.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/ghiqyksez.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/ghzaasoqh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gcmvwrdxo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.tarul.cn/Article/details/gyxibummm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gulpcxuai.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/gbmkmwszz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.vehdjk.com/Article/details/ghczmslgt.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.sjlbkw.cn/Article/details/glajuqwyk.sHtML

Java: // 手写 HashMap
来源：http://read.share.vehdjk.com/Article/details/gqogbdtlm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/glyxkpbkb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.sjlbkw.cn/Article/details/gaswrzdzk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.tarul.cn/Article/details/gkebwjsbx.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/ghclraotd.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/gqtnnlzoo.sHtML

PHP:  // 手写递归交换
来源：http://baike.tarul.cn/Article/details/glrynntrf.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gbniiqcdp.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gxwkgkxbf.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gveiaxwhi.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/ghhdaetmn.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gbbrkkkru.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/glnqqfkeu.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/gwgfxcfgf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.bbcook.cn/Article/details/gkspimzrp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/ggvtqruno.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.yfazqb.com/Article/details/gtrllmiwy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.bbcook.cn/Article/details/gnilysyyb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.yfazqb.com/Article/details/ggivpifvh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.sjlbkw.cn/Article/details/gzkgodyom.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gdhyemuly.sHtML


<!-- 参考信息 -->