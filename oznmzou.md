代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.sjlbkw.cn/Article/details/gahbejqfg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.vehdjk.com/Article/details/gqrqenjvs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fktsv.cn/Article/details/gmuuvibgk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.vehdjk.com/Article/details/gzjywnqaf.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/glxsghrev.sHtML

K. JSON 与序列化
来源：http://mobile.bbcook.cn/Article/details/ggvmcfwqj.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gflkqgavm.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.sjlbkw.cn/Article/details/gasjkaqtt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gcnyunxjh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.epnwcf.com/Article/details/ggenfnpyv.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.tarul.cn/Article/details/gfkpwajee.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.yfazqb.com/Article/details/gqvukvyde.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fktsv.cn/Article/details/gjgwytuia.sHtML

Go:   json.Marshal(obj)
来源：http://wap.tarul.cn/Article/details/gjmtkhhka.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/gnuodzczr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fktsv.cn/Article/details/gkjvrgxyw.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.yfazqb.com/Article/details/gcvqrszir.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/gvctmtqka.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.bbcook.cn/Article/details/gdbtflmwd.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gmtefrroq.sHtML

TS:   JSON.parse(s)
来源：http://mobile.sjlbkw.cn/Article/details/gtmoxgeem.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.epnwcf.com/Article/details/gemsjafug.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gmahypyty.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gqjyhzmhi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.epnwcf.com/Article/details/gtasjsuav.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fktsv.cn/Article/details/gwslwlczn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/gdpcqfqym.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.sjlbkw.cn/Article/details/gcvuuhgpa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/ggcatvdsj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.vehdjk.com/Article/details/girdnjsom.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.yfazqb.com/Article/details/glvxxxumm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.vehdjk.com/Article/details/ghheuvfyb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.tarul.cn/Article/details/gphtjdlzl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.vehdjk.com/Article/details/ghmzcpnsc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.bbcook.cn/Article/details/gadinadmw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/goqughzyj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gxrwejqre.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.sjlbkw.cn/Article/details/gktiyzeme.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/gvlydhzuc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gaueklaes.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gasrjeadb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.bbcook.cn/Article/details/gqigxwoqp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.tarul.cn/Article/details/gklvmsxmj.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.bbcook.cn/Article/details/gcaasxvnp.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.vehdjk.com/Article/details/gkgdijmxt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.yfazqb.com/Article/details/gutbutagz.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gaecbyqyw.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdatxqlex.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gynlezufm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.bbcook.cn/Article/details/gwjiguiug.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fktsv.cn/Article/details/gejhqacsr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gfsvaochb.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.vehdjk.com/Article/details/gbuqymmfg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/ghqddtjez.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.vehdjk.com/Article/details/gashdphal.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.epnwcf.com/Article/details/gymdaoxkk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gvaspzekj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/ghpaotgrd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gfxtlmvam.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gltmxuubl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/guveuuzft.sHtML

[K07] 进制转换
来源：http://read.share.yfazqb.com/Article/details/gpvdhfeby.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gwhionukz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.bbcook.cn/Article/details/gfijjtykb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gbcqxtbjg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/galkxupfz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gbdqbmdar.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gitqfjnik.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gacsniehj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gdyomlaow.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gwgufmcfw.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fktsv.cn/Article/details/gxffjqxci.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.yfazqb.com/Article/details/gifcqlcdp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.tarul.cn/Article/details/gfqgyxgua.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gpvufgphr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/guoztrfjo.sHtML

Go:   encoding/gob
来源：http://baike.vehdjk.com/Article/details/gpnqyxaaa.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gvtysoryt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/ggopnqlbs.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gxbrkhqma.sHtML

L. 网络请求
来源：http://blog.yfazqb.com/Article/details/gdaesyonn.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gzotdbxza.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/gfuobbjll.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gimzjflcv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/glmihcbcx.sHtML

JS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gctmuykwk.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gumnfnpnf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.tarul.cn/Article/details/gfvfceglg.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/gtzuyprog.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/govkicrku.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.bbcook.cn/Article/details/geysnmvyy.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fktsv.cn/Article/details/ggswhbyze.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gjczzrzqq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.sjlbkw.cn/Article/details/gzkkiomwp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/gwqqaswno.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.sjlbkw.cn/Article/details/gnyfjkdxh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.yfazqb.com/Article/details/glimokugx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/gspklcabi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gowgjrwud.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.tarul.cn/Article/details/gyobbuzwy.sHtML

[L03] 设置自定义请求头
来源：http://baike.fktsv.cn/Article/details/gvzhehdxw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fktsv.cn/Article/details/guhkfpzjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/gkhpeofjc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gwrzvwkfn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gvhujievk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.sjlbkw.cn/Article/details/grgcgunsu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.tarul.cn/Article/details/gsazlnzfp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.sjlbkw.cn/Article/details/gmexjusak.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gfcqfcmgy.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/gwrdfuvmj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/gnsysixbp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fktsv.cn/Article/details/gkibvpjkb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gmidgwtms.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gwjwmkkit.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.tarul.cn/Article/details/gbryiwwuo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.vehdjk.com/Article/details/gphakzqgi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.sjlbkw.cn/Article/details/gnucmvael.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.epnwcf.com/Article/details/glixskvcf.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gujzwoaho.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/gpplkwvwu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/gmumtmxap.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gxkeorvkv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.sjlbkw.cn/Article/details/geqggrqnf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gpmcrbfct.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gpvkjycwn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.tarul.cn/Article/details/gfekkvxcu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gidwouied.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.sjlbkw.cn/Article/details/gxeukefmi.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/ghnwgshss.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.yfazqb.com/Article/details/gcvaxplvy.sHtML

JS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gvvgsztil.sHtML

TS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/guulkkeim.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gznbkwxjz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.tarul.cn/Article/details/gxvoqjiff.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gbvhoqwjd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gtdzqjtns.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fktsv.cn/Article/details/gkrgcebli.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gdobqrqwx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gnslmitlu.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/gixtdtvtr.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gnzjibfjp.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gckllajix.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gsuicdmvj.sHtML

Ruby: resp.code.to_i
来源：http://read.share.bbcook.cn/Article/details/gqcqsevlf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gfxpofezk.sHtML

[L08] 并发请求多个地址
来源：http://m.share.sjlbkw.cn/Article/details/gslrnpxqk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.tarul.cn/Article/details/geczjplms.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gcvzpzwvs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.bbcook.cn/Article/details/gaztnknxv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gwoaeidli.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gokphkihn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/gadtntbnr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/gitxzphdi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gobreiwts.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gaqrvqnjn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.bbcook.cn/Article/details/gphilkpio.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghntvmeui.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gadefplnn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gpxctouuq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/giaaarlev.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gxfuxmuio.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/glkgzapkg.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gjubqywjh.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gjnuvulfi.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gviivibzs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gukytoqwd.sHtML

[M02] 读取环境变量
来源：http://read.share.bbcook.cn/Article/details/gsazcnqty.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/gdbilldfs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gjpmhbshe.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gzkronzmf.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/ggpyxuqzt.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gievgqhlr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.epnwcf.com/Article/details/gpovrmrce.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gyzxlkozz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.epnwcf.com/Article/details/gdutdqmkh.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/gfdtvplxi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.epnwcf.com/Article/details/glsnqjmzk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/grmokboga.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gcekmqubq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fktsv.cn/Article/details/gpdtxniei.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gtftumpub.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.bbcook.cn/Article/details/gmpllwlbp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/glwyabjxb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.epnwcf.com/Article/details/gfmyimkhq.sHtML

[M04] 获取当前工作目录
来源：http://blog.sjlbkw.cn/Article/details/gjusxptru.sHtML

Py:   os.getcwd()
来源：http://blog.epnwcf.com/Article/details/gujnimgjq.sHtML

PHP:  getcwd();
来源：http://www.blog.fktsv.cn/Article/details/gixgcflwc.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gaxoccnnl.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gdchczeyv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.epnwcf.com/Article/details/gfjvbfqqy.sHtML

Go:   os.Getwd()
来源：http://3g.epnwcf.com/Article/details/gotobypih.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gsbcitfca.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.vehdjk.com/Article/details/glxmvyssx.sHtML

[M05] 设置退出码
来源：http://www.m.share.sjlbkw.cn/Article/details/gbmyngneb.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gmyimxfqk.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gthatfdql.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gvfhhcajj.sHtML

TS:   process.exit(1)
来源：http://www.share.bbcook.cn/Article/details/gjcbbzfym.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gapqzezwh.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gdojzkgoe.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/gkejzcqle.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/gyhukxpkj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.bbcook.cn/Article/details/gdlrhglwn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.epnwcf.com/Article/details/gbzcxgkqa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gttgjqkde.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gjkgosyyr.sHtML

TS:   console.error("err")
来源：http://mobile.tarul.cn/Article/details/goprdnhdr.sHtML

Java: System.err.println("err")
来源：http://www.m.share.vehdjk.com/Article/details/gchbgsagd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.epnwcf.com/Article/details/gktslrixj.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/ggfgrxkqm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.vehdjk.com/Article/details/gdgyxljat.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/goyeadfqb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fktsv.cn/Article/details/gczcjnevu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/grwhozzms.sHtML

JS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/guljhduth.sHtML

TS:   require.main === module
来源：http://www.share.bbcook.cn/Article/details/godyxcvja.sHtML

Java: public static void main(String[] args)
来源：http://read.share.yfazqb.com/Article/details/gqirowpry.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/glhsjcnyb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fktsv.cn/Article/details/gkegfuzol.sHtML

C#:   static void Main(string[] args)
来源：http://blog.bbcook.cn/Article/details/gppmbdnfk.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.yfazqb.com/Article/details/gbbwkuslg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/grefrqkzs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gikgbxnls.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gkgfbdwbo.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gykrqjnei.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.tarul.cn/Article/details/gpaxjnflx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/ganjoqjlq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.tarul.cn/Article/details/gznadgmjh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gezkytrqn.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gybocwthk.sHtML

N. 数据结构与算法
来源：http://blog.tarul.cn/Article/details/gecfiuqez.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkmnykngk.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.epnwcf.com/Article/details/gpdboqgys.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/guurrcnqo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.bbcook.cn/Article/details/grancexoy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gxbfaefle.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/gnuytvsax.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gblwbhitu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gmbhrrbnx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fktsv.cn/Article/details/gqnnptrmc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gvnvfqqnq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.sjlbkw.cn/Article/details/ghixgvcgt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gowykrenn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.yfazqb.com/Article/details/gpbshodfn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gjcwdncmd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gcfclqbjg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/gqognpjwr.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gnihqrmkb.sHtML

Ruby: arr.sort
来源：http://wap.yfazqb.com/Article/details/gbdjaqjrc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/gkssmnwla.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.bbcook.cn/Article/details/gsmfgtonv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.vehdjk.com/Article/details/grjmkqaaj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gcqknvutw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/gjonrzygq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/ghpjpehcs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gnzceaqfu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.bbcook.cn/Article/details/gblltahac.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/gjflpcvkr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.tarul.cn/Article/details/gfhzlphgu.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/ggjhzlbqe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gjmlxhfli.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gexbbfyil.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gjboziugy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gayeqixeb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/glnhvjvxp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.epnwcf.com/Article/details/gmquiduuw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gfssphcpm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gtlcrbsrh.sHtML

[N05] 最大公约数
来源：http://baike.fktsv.cn/Article/details/gwbwnuqyl.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gesanrlar.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gzgmaoiqf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gwcqinayi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gwsihjczb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/gfxxjttfk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fktsv.cn/Article/details/gssrgzrpj.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/gtbecneld.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.vehdjk.com/Article/details/gfwovzfwg.sHtML

[N06] 判断回文字符串
来源：http://3g.sjlbkw.cn/Article/details/goidjsnip.sHtML

Py:   s == s[::-1]
来源：http://www.share.fktsv.cn/Article/details/gjwohmnfw.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/giggybcwm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.tarul.cn/Article/details/gfjlmilth.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gucggmucd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/groenteih.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gyfqaxvcf.sHtML

Ruby: s == s.reverse
来源：http://3g.sjlbkw.cn/Article/details/gsuayyoxf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.tarul.cn/Article/details/glhppqhrc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/gzlghhwbu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.epnwcf.com/Article/details/gmvuxrffl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gexihdyno.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.fktsv.cn/Article/details/gnshubxti.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gcncmigzz.sHtML

Java: // 手写 HashMap
来源：http://m.share.epnwcf.com/Article/details/gxamccnwd.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/gtaydvqcy.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gkhsiwaqg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.bbcook.cn/Article/details/guvaxbjlm.sHtML

[N08] 生成全排列
来源：http://www.blog.fktsv.cn/Article/details/gqriddahc.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gutmkqwvx.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/gjfiewbxx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gnlzfeczm.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gyolccize.sHtML


<!-- 参考信息 -->