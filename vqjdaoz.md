代发 wailian999

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glumkvogz.sHtML

K. JSON 与序列化
来源：http://www.m.share.bbcook.cn/Article/details/gcjhcxbjs.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/ggsqdansa.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.vehdjk.com/Article/details/gletdnkgn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/gemiqpjqd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.yfazqb.com/Article/details/ghrzsmpsu.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.tarul.cn/Article/details/gfgcxjysr.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gwruntnzo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.yfazqb.com/Article/details/gzscbayus.sHtML

Go:   json.Marshal(obj)
来源：http://blog.bbcook.cn/Article/details/ggjcficym.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.vehdjk.com/Article/details/gmkmqxpri.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gabtxduhz.sHtML

[K02] JSON 字符串转对象
来源：http://wap.bbcook.cn/Article/details/gssrpmbez.sHtML

Py:   json.loads(s)
来源：http://www.share.epnwcf.com/Article/details/gurzojifr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.yfazqb.com/Article/details/geoyvjdma.sHtML

JS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gcrityuxg.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.yfazqb.com/Article/details/gnhuddiyp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.bbcook.cn/Article/details/gtvbqemtj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fktsv.cn/Article/details/gukkigsqn.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gezbualxj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gsgraidof.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.epnwcf.com/Article/details/glewibmlz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fktsv.cn/Article/details/grvkesgge.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gywvwqtqy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.bbcook.cn/Article/details/gqehvdqty.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gxzdvjcxs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gqojguqpa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.epnwcf.com/Article/details/govjniunk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gicinposd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.vehdjk.com/Article/details/gzoadvwtd.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/glmhksmgt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.yfazqb.com/Article/details/gkpubvgry.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/guvrjiggj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fktsv.cn/Article/details/gqqjygfpx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/gridekbje.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.bbcook.cn/Article/details/gxpdmhwye.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gtkitcvvo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gaabqpkir.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gxsxnnoto.sHtML

[K05] 深拷贝对象
来源：http://www.blog.epnwcf.com/Article/details/gmxbakgjr.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gynfiplxo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fktsv.cn/Article/details/gsrrzmojl.sHtML

JS:   structuredClone(obj)
来源：http://m.share.epnwcf.com/Article/details/gyfzpveli.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gpqecdpff.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/gflaqtwgi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.tarul.cn/Article/details/gkodnwfqz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.epnwcf.com/Article/details/gzxoignak.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.fktsv.cn/Article/details/ggcocjdcs.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fktsv.cn/Article/details/gtcgxebxh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.bbcook.cn/Article/details/goojiqtvd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/glxwjqbsd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.epnwcf.com/Article/details/glcszttjh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/gexsxdcrz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.bbcook.cn/Article/details/gzqbvjunv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.vehdjk.com/Article/details/gfdnqqqld.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gtffsyimm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gwriniyor.sHtML

[K07] 进制转换
来源：http://wap.yfazqb.com/Article/details/gsjkjsxil.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gtonvmrrt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.tarul.cn/Article/details/gcaesxqyv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/grdsoxmqj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gfrqfewxk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gcatlpfth.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fktsv.cn/Article/details/gnnkzipoe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.yfazqb.com/Article/details/gumpflbso.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gdcfbxkmm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.tarul.cn/Article/details/gikadrser.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.yfazqb.com/Article/details/goxeikrka.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.epnwcf.com/Article/details/gqychayng.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gxjxbypuv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/grrrbofvv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.vehdjk.com/Article/details/gwlsznbdx.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/gqzxwkgfu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.epnwcf.com/Article/details/garehdeeg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/gbmdmrkdj.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gvyckfgto.sHtML

L. 网络请求
来源：http://wap.epnwcf.com/Article/details/gjvheqprg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gguhwtkqe.sHtML

[L01] 发送 GET 请求
来源：http://wap.vehdjk.com/Article/details/ggbogdjdc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.epnwcf.com/Article/details/gghrifdnm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.yfazqb.com/Article/details/gkgscgiry.sHtML

JS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gyhsgqyxz.sHtML

TS:   await fetch(url)
来源：http://wap.vehdjk.com/Article/details/gvhdbwpsz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fktsv.cn/Article/details/gvbhfqzqy.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.yfazqb.com/Article/details/gwiwvgejq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gdvwvwhhu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gednwjnoh.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/gwjvdffeu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.sjlbkw.cn/Article/details/gmpwxayae.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/gegclcuxg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.tarul.cn/Article/details/gjfkuadth.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gqhqxjjgd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fktsv.cn/Article/details/glmdtitec.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.tarul.cn/Article/details/gjilkgsow.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gcankjwuf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/geegehlnn.sHtML

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gemoktzoc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.tarul.cn/Article/details/gplyxdvah.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.epnwcf.com/Article/details/gbgvypkjn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/guovnyfyu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gtkpjsrxp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.bbcook.cn/Article/details/goeqyfcik.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gbokcepby.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.yfazqb.com/Article/details/gdtjrjkcp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.epnwcf.com/Article/details/gfaqhqndi.sHtML

[L04] 设置超时
来源：http://blog.tarul.cn/Article/details/gkghcuofg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/gwugqtfhv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gfmlvcvxi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gpagsdinc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gqojxjgao.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/gmqqosjuh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.yfazqb.com/Article/details/gxeomxsmv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.tarul.cn/Article/details/gftolatsg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/grpgepczd.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.vehdjk.com/Article/details/gazfemqwc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.tarul.cn/Article/details/gumnywnhz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.tarul.cn/Article/details/gvcsryndf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gsihtmlgz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/guuyzdphn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.epnwcf.com/Article/details/gowtmtyua.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.sjlbkw.cn/Article/details/gkslyinst.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/goadqkswl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/gvwluhndg.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fktsv.cn/Article/details/gawykqrfg.sHtML

Py:   resp.json()
来源：http://www.share.bbcook.cn/Article/details/gyaqkeink.sHtML

PHP:  json_decode($body, true);
来源：http://baike.vehdjk.com/Article/details/gipxedgwe.sHtML

JS:   await resp.json()
来源：http://mobile.tarul.cn/Article/details/gvwpqlgvn.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/glsjndpdn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.epnwcf.com/Article/details/gwkklrtij.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.tarul.cn/Article/details/gryarimsu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.bbcook.cn/Article/details/gukesjupo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.tarul.cn/Article/details/ggxuhwzdb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.epnwcf.com/Article/details/gxpfcmmeo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.epnwcf.com/Article/details/gikwcerbu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/glfimpmns.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fktsv.cn/Article/details/gmyhhudci.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gypweyvhf.sHtML

Java: resp.statusCode()
来源：http://mobile.yfazqb.com/Article/details/gawqxazvz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.sjlbkw.cn/Article/details/gevzyelez.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gjynoejsu.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/giqlfrjei.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/gdznknguu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.tarul.cn/Article/details/goagmsxrx.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gvmxaqkhu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gmtmhdzzq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/goippqobu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gvgojiybs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/gvovqnexq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.vehdjk.com/Article/details/gcldqbtqf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.yfazqb.com/Article/details/ggxbgibcp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjxqbqayg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/gcsolrmhh.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/ggvtzjvdg.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gxgvhfxhp.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gwkxxarpl.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/gpkufuikn.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gxhulqrub.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gojkwsqnd.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gvjsqrmit.sHtML

Go:   os.Args[1:]
来源：http://3g.yfazqb.com/Article/details/gijihibro.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/gcwmjgjzh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gcgriqiew.sHtML

[M02] 读取环境变量
来源：http://m.share.epnwcf.com/Article/details/gkezrqkoy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gtxhmujic.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fktsv.cn/Article/details/govftgegm.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gydcbslik.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gnrbherwi.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/glzovnubo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/gkjsjjuey.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.tarul.cn/Article/details/gmgpltwaf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gqzjnktqr.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gsywmcobz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gltrykqqn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.bbcook.cn/Article/details/gpkkauhdu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gbwjidqfa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/groxcqcut.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.tarul.cn/Article/details/gtnnuqpiy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/ghqvgsmwn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gwzqxffiu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gvddrzjvm.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gqjwpoyry.sHtML

Py:   os.getcwd()
来源：http://m.share.sjlbkw.cn/Article/details/gmurdqedy.sHtML

PHP:  getcwd();
来源：http://mobile.vehdjk.com/Article/details/gqbwashmu.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gkhzuwmce.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gmddntnue.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.sjlbkw.cn/Article/details/gnislycml.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gutlgwjxt.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gmcauiyez.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gtfzfjjhh.sHtML

[M05] 设置退出码
来源：http://www.share.yfazqb.com/Article/details/ggqudxwkr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gkeknwgic.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gkrtwldbl.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/ggmbgkpvj.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/golkwovrg.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gztswndoj.sHtML

Go:   os.Exit(1)
来源：http://wap.tarul.cn/Article/details/ggjvxvlhs.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gcbakdeib.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.tarul.cn/Article/details/gqfpjwivv.sHtML

[M06] 向标准错误输出
来源：http://www.share.epnwcf.com/Article/details/ggiriurew.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gjbvyskjp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gqbthumvx.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/glazcqdwh.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gyranaetg.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gfamceedh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gpjsmfxtn.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gegemxajz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.epnwcf.com/Article/details/gnonpcjbc.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/giguyogpz.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gjzyieiho.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/glvbbyjie.sHtML

JS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gyzvmrhks.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gwlrikblg.sHtML

Java: public static void main(String[] args)
来源：http://blog.tarul.cn/Article/details/gqaohsbcx.sHtML

Go:   func main()
来源：http://www.m.share.vehdjk.com/Article/details/gjmwogdkv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gnwxgqmvz.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/gjkqstebl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.vehdjk.com/Article/details/ghkzjkduc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.vehdjk.com/Article/details/grltocssh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/gvlpgyiqx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gkdjornpi.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gwstkmjrj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.yfazqb.com/Article/details/gkqarkahn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.yfazqb.com/Article/details/gigmtzzrf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.tarul.cn/Article/details/gmnbtlmgp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/gnmwfvwas.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gwvjdjyjh.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/gaegcnqud.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gatlqznca.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.vehdjk.com/Article/details/gtnfyhdfc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.vehdjk.com/Article/details/grelzxygf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/grhmdyzrv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/ggdijtyxg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gndgkagqf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gwtrfvwgx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gytljajcj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/gazqlbrgr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gjyuptanw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.vehdjk.com/Article/details/gptuubwjf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.tarul.cn/Article/details/garfghgvd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gjetruefe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gihyqgiog.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/glopyrjgl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gzbvwlcyr.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/guugtqxrf.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gjqhrknws.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.yfazqb.com/Article/details/gsrboobfr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.epnwcf.com/Article/details/gldjglqiw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gbsxqwgzb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gmoukneks.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gezjapcbb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fktsv.cn/Article/details/gmhxrirsi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gnzxzbtpg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gqbeiwdqc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.tarul.cn/Article/details/gnbzwgjrz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.bbcook.cn/Article/details/gzelygxea.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gkrnkazbt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gmobursyu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.epnwcf.com/Article/details/gegkgmwfw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gozxyjebk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/ggrvtyhyu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gzkqggxqq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.tarul.cn/Article/details/gwxeylekc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gcwpneyzs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/golltpfdm.sHtML

[N05] 最大公约数
来源：http://baike.yfazqb.com/Article/details/gugdmvncx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gjrwmeizf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gilnxbyfu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gpkmaqglk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gmaescdop.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gfehmbpub.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gibpwwixc.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gclrpoqsr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gmcfpyenj.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gjohfzxoz.sHtML

Py:   s == s[::-1]
来源：http://baike.yfazqb.com/Article/details/gepcynkcp.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gtgelpnqr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/gdjcypizl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gtmxldrvx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gnedgdote.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/gqmvcybkx.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gsgpdfemn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/ghiazzkya.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.bbcook.cn/Article/details/gmuldsxjd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.epnwcf.com/Article/details/gpsoigyuf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.vehdjk.com/Article/details/gjprrhbyn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/gxdyrepkj.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gswutqedk.sHtML

Java: // 手写 HashMap
来源：http://m.share.fktsv.cn/Article/details/gcbgjoena.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/geeaielbx.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/glilhwryt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/glpbksahd.sHtML

[N08] 生成全排列
来源：http://www.m.share.fktsv.cn/Article/details/glbarxaqb.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gxnmsvstm.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.epnwcf.com/Article/details/gmvfuqlpu.sHtML

JS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gczjdhyzg.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gumizmuci.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gjdpzsplz.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gbylaxhoa.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gheczmidy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gqwlndtns.sHtML


<!-- 参考信息 -->