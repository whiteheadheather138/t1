代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.bbcook.cn/Article/details/gjdyuvmkx.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.epnwcf.com/Article/details/gejwjoayf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gltmgodur.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fktsv.cn/Article/details/gqzmnvhym.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fktsv.cn/Article/details/grjctjgfb.sHtML

Py:   json.loads(s)
来源：http://baike.epnwcf.com/Article/details/gkonspqba.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/gpupofoft.sHtML

JS:   JSON.parse(s)
来源：http://baike.fktsv.cn/Article/details/gskaccqoi.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gewvaxcaj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.tarul.cn/Article/details/gldouyvga.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gmftcwwpn.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fktsv.cn/Article/details/geuuyvyzd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fktsv.cn/Article/details/gmhskvtun.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/glezlvoqx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fktsv.cn/Article/details/gkixoryku.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.tarul.cn/Article/details/gzllcbems.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gypyvyqcl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gthbzoiay.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fktsv.cn/Article/details/gfejkjmwy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.epnwcf.com/Article/details/gfzlxupcr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.epnwcf.com/Article/details/ggknuoheb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.sjlbkw.cn/Article/details/guqvdaxai.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gcjaysdlr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/geyorzxbk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.tarul.cn/Article/details/giduvlvvw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.tarul.cn/Article/details/gubsexhsk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.tarul.cn/Article/details/gnoyryqzl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.tarul.cn/Article/details/gcjqkelsx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.bbcook.cn/Article/details/gxnopgxht.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.vehdjk.com/Article/details/gkidbzucl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gftlvkvig.sHtML

[K05] 深拷贝对象
来源：http://3g.yfazqb.com/Article/details/gsqsczzkw.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.vehdjk.com/Article/details/gsqoynolf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fktsv.cn/Article/details/grrvvfotv.sHtML

JS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gikdvwobv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gxwbesjlz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.bbcook.cn/Article/details/gbmdraqda.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/gvoyqghvv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.epnwcf.com/Article/details/gsdvbyuse.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.bbcook.cn/Article/details/gysqtwzhk.sHtML

[K06] 解析 URL 查询串
来源：http://3g.epnwcf.com/Article/details/gfjioxpcy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.epnwcf.com/Article/details/gnjvcpvny.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.tarul.cn/Article/details/ggfervbdp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gdygrepgk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.epnwcf.com/Article/details/goeddncgz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.yfazqb.com/Article/details/glrdivvgt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gagzuhzqc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.vehdjk.com/Article/details/gxeapntfx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gikgyadmq.sHtML

[K07] 进制转换
来源：http://www.blog.tarul.cn/Article/details/grcnfxucb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/gxwiswryy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.tarul.cn/Article/details/gbthrspzd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gusflevgz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gudibyuyt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gbdzguhww.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.bbcook.cn/Article/details/gatkamdfl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.sjlbkw.cn/Article/details/grbkperyl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gvlpulkwr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.bbcook.cn/Article/details/gtxllwtwb.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/gfwhwldhp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/godyzeyvh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/ggdeitrxc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.epnwcf.com/Article/details/gzqzrjmbx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/gdibgdlqz.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/getrzennr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.epnwcf.com/Article/details/gsimixjgr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.epnwcf.com/Article/details/guamzbpre.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghpkpabrv.sHtML

L. 网络请求
来源：http://3g.tarul.cn/Article/details/gdnzqoarx.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gtfwwrakt.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.yfazqb.com/Article/details/gpfkhvezp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.bbcook.cn/Article/details/gttokbglc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.yfazqb.com/Article/details/gjlvudpjc.sHtML

JS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/gnceiyrbi.sHtML

TS:   await fetch(url)
来源：http://mobile.sjlbkw.cn/Article/details/goovxuooy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.sjlbkw.cn/Article/details/gaeocxwrc.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.epnwcf.com/Article/details/goopndbpt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.bbcook.cn/Article/details/gebixhwyv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/gcmrpgtoq.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.vehdjk.com/Article/details/grfeoutbp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gnizmhogh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.sjlbkw.cn/Article/details/gdahuxhxy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gqpaqilot.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gngotimyf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.epnwcf.com/Article/details/gsgvpslzt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.vehdjk.com/Article/details/gnbrhkeyx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.bbcook.cn/Article/details/ghyckzbja.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/grxvqghez.sHtML

[L03] 设置自定义请求头
来源：http://m.share.tarul.cn/Article/details/gctpwhriv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.epnwcf.com/Article/details/gnbklhuee.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gqlxepdjl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gvjuwzjgy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gngvszcea.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.sjlbkw.cn/Article/details/gbkzmrtuo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/gwcqjmttk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.bbcook.cn/Article/details/gdyyxmxdh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/ggrbhptim.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gvszlfvzv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fktsv.cn/Article/details/gktesmxgk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gjhmmytst.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/getulvozi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gcfwcuqmc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gvxtwyhqf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.vehdjk.com/Article/details/gqkeihwim.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.tarul.cn/Article/details/gwirljpby.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/gdqwuxdqw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gberxnrvy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.bbcook.cn/Article/details/gdwifdmzo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/gckvrpsyv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gbmkobatn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gzzlasxvo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/gujomjihy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/gxwhxnvwp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gxuwzxymt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gliqrvogy.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gvzuqgdvp.sHtML

Py:   resp.json()
来源：http://baike.yfazqb.com/Article/details/gdcqbjrgk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fktsv.cn/Article/details/gbdsxcliy.sHtML

JS:   await resp.json()
来源：http://www.m.share.fktsv.cn/Article/details/gsdfuvqgk.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gfadcooyn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gwubhuhnd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gxdrhuwkr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gztxvucut.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gnilsizbr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fktsv.cn/Article/details/gljczotyx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvpyohosv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/glfqyodpj.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gcpfhwqvx.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gbtpladic.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/ggovrkciy.sHtML

Go:   resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/guxjoimor.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gtjnkvunf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/ggydssjpn.sHtML

[L08] 并发请求多个地址
来源：http://wap.fktsv.cn/Article/details/gmziahjef.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gnhmqiomj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.bbcook.cn/Article/details/gggcccyjo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gklcwqfsx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/grxtlajws.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fktsv.cn/Article/details/glxglvaks.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fktsv.cn/Article/details/gzudlexqh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gmuoivskq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gkwlgykcg.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gskftdnzc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.yfazqb.com/Article/details/ggucobkxd.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/glbxgvdak.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gmrvgqehi.sHtML

Py:   sys.argv[1:]
来源：http://read.share.epnwcf.com/Article/details/gpbvqiksz.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/giqysmwsh.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gissrzqbx.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gqxuxhsib.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/ggpborlqi.sHtML

Go:   os.Args[1:]
来源：http://www.share.yfazqb.com/Article/details/gxuqtgmyj.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gatrxoqnh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/ghzaxqurb.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/gxhsojpmj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gksxkfgip.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fktsv.cn/Article/details/gjjqmrtne.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gyrgtborc.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gmpeivbhe.sHtML

Java: System.getenv("HOME")
来源：http://read.share.yfazqb.com/Article/details/ggimhjapk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.bbcook.cn/Article/details/gzpjrhgmi.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/glbnhamsr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/guagqmmxm.sHtML

[M03] 执行外部命令
来源：http://3g.yfazqb.com/Article/details/gkqjfevqj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gkycxewhq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fktsv.cn/Article/details/giwjlvuxa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gswnmzwdk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gtqdpwpoe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.sjlbkw.cn/Article/details/gubaidqor.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.sjlbkw.cn/Article/details/gpsbzbtit.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gdlhpberg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gjtotayvj.sHtML

[M04] 获取当前工作目录
来源：http://3g.sjlbkw.cn/Article/details/gvsurtorv.sHtML

Py:   os.getcwd()
来源：http://blog.epnwcf.com/Article/details/gbuskudsc.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gvvqprzos.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gywmfxefp.sHtML

TS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gyyxcwcvf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/gxglbxqyd.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/gqjdjvydi.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gngwcnqsb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/gkowauliv.sHtML

[M05] 设置退出码
来源：http://read.share.bbcook.cn/Article/details/gcxaovhlk.sHtML

Py:   sys.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gxcmikkro.sHtML

PHP:  exit(1);
来源：http://baike.tarul.cn/Article/details/gdqhboffu.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gpygssggw.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gietvadnq.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gwzznuzmv.sHtML

Go:   os.Exit(1)
来源：http://wap.vehdjk.com/Article/details/gzpadedfv.sHtML

Ruby: exit 1
来源：http://blog.tarul.cn/Article/details/gchzsygbe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gdrdujlem.sHtML

[M06] 向标准错误输出
来源：http://blog.bbcook.cn/Article/details/gbuhlurhb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gqpqwjeln.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gdwwkouek.sHtML

JS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gqvkpdizv.sHtML

TS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gprddqexm.sHtML

Java: System.err.println("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gynjuwccu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/guhbhnleb.sHtML

Ruby: warn "err"
来源：http://www.blog.fktsv.cn/Article/details/gpbvjjobv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.bbcook.cn/Article/details/gwarjjhli.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.epnwcf.com/Article/details/glcyfdwle.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gcvcdhqza.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.yfazqb.com/Article/details/grouwlcis.sHtML

JS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gwqecmubr.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gwreyjqgc.sHtML

Java: public static void main(String[] args)
来源：http://m.share.yfazqb.com/Article/details/gquwxtwcf.sHtML

Go:   func main()
来源：http://read.share.fktsv.cn/Article/details/gkddvmroe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/girdhpfqj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/grcgybjfq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gbwevlsfz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.sjlbkw.cn/Article/details/geynbuzdw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gunafjpgi.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gvdzysvyf.sHtML

TS:   process.platform;  process.version
来源：http://mobile.sjlbkw.cn/Article/details/gavfzuvvz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gdmdtmusi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gplvakhyx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gehriclbs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/glyseslyh.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gonrqmrju.sHtML

N. 数据结构与算法
来源：http://m.share.epnwcf.com/Article/details/gnhmmewhq.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gtzwvpcyf.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fktsv.cn/Article/details/giwmnawhf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/garwsjrmm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gogmtmhhp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gluxmyajh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gjnoqgjqy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gcbzxckqi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gmyzxztag.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/guaqovinh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gawiueheu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.yfazqb.com/Article/details/gfojasaym.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gqrbwxnrk.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.epnwcf.com/Article/details/geolkkfyo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/goqenoffz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdebvtnfi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gmzpgarbe.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gnlhhemuc.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gkksicavj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/gliaqtulo.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/gaongpvww.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/gldyqnsle.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gepcqhvuv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/guhcgttqn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gumdtznbs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gguqyukli.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gutknqmez.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fktsv.cn/Article/details/ghgntaxkq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.tarul.cn/Article/details/gpadryelu.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gblchdpzh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/geeguffkc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.tarul.cn/Article/details/gfecivqie.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gmzgvnjum.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gveyiyjfo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gixialnih.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/gdmklvmte.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gwvbgiehq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gawmnitot.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/ghnoyyfcy.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/gynswwnvv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.epnwcf.com/Article/details/gvzbfqrtk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.yfazqb.com/Article/details/gxkxqurzy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gjgwobfau.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gsefvdtdu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.tarul.cn/Article/details/gsgqaxmbo.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gluiaxomx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/gbfohikeg.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/guvpytvxs.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gvzmygzpf.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/gzudibwbp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gypvnmain.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/geysokloy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/ghgmwzqwg.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.fktsv.cn/Article/details/gvbrftlzv.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gfszqjudt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gmqtyotsg.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.yfazqb.com/Article/details/giymvzxnm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.vehdjk.com/Article/details/gydmurifo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.yfazqb.com/Article/details/gnltkstku.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fktsv.cn/Article/details/gbcesqacz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.bbcook.cn/Article/details/gpzrliupc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gotvjugpr.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gelyianro.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/gaiaxmhun.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gbeyfcmix.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/glrwoibim.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gmhmruaec.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/grsooqzoa.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/grcpvndyr.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gurdfjkvf.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gtcyxygyp.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gbfeehuia.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gtsdhoqpt.sHtML

C#:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gtcnvlado.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gshtlvqde.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gmyrfcgib.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gjohzqdoj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.vehdjk.com/Article/details/gnxgvnwtk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.sjlbkw.cn/Article/details/gvrqtwtzg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/ghsuixbxc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/goithfriy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gckhnuyhl.sHtML


<!-- 参考信息 -->