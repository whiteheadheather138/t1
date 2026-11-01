代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.vehdjk.com/Article/details/gbhhdimwf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fktsv.cn/Article/details/gkzmnepht.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.yfazqb.com/Article/details/gwbgnlmik.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.yfazqb.com/Article/details/gfkxosoel.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.tarul.cn/Article/details/geeclvfsu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.tarul.cn/Article/details/gnvlqosca.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gsjfnxtvl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gjxisqlfn.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gysmnrqnb.sHtML

K. JSON 与序列化
来源：http://mobile.sjlbkw.cn/Article/details/gjkbxxdbw.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gljwgdebl.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fktsv.cn/Article/details/gweqqcxih.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gpvaerand.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.tarul.cn/Article/details/gdxipvgrd.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.vehdjk.com/Article/details/gjtnifgoy.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.vehdjk.com/Article/details/gqaxrefhm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gvktqqmgx.sHtML

Go:   json.Marshal(obj)
来源：http://blog.vehdjk.com/Article/details/gkdphmujh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fktsv.cn/Article/details/gpqrftjfn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gznxqqwob.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/gksxsucvf.sHtML

Py:   json.loads(s)
来源：http://wap.vehdjk.com/Article/details/gplbrfqpo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.bbcook.cn/Article/details/gfpedzclv.sHtML

JS:   JSON.parse(s)
来源：http://m.share.sjlbkw.cn/Article/details/gtnefmqmf.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gbaoeomsl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.vehdjk.com/Article/details/gyxnpysza.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gptxjtchk.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/grdkngsok.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/ggpzgsrck.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.sjlbkw.cn/Article/details/gefmmzcae.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gwejmbhzp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gmgufuegp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.epnwcf.com/Article/details/gzgfkibnp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gniwqjoax.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gukifdpwo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.bbcook.cn/Article/details/gwktytoyv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.epnwcf.com/Article/details/grgkkdnww.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fktsv.cn/Article/details/gsraljdxu.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.tarul.cn/Article/details/gyevlomjb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.yfazqb.com/Article/details/gjmcqqgrx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gqgzygqrk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gxhmpxwga.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gpktvmggk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gmsuljjkh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gsbxcorll.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gfrsrjiuz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.vehdjk.com/Article/details/glrexajxf.sHtML

[K05] 深拷贝对象
来源：http://baike.vehdjk.com/Article/details/gxlabwwjp.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gczmptdxe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.yfazqb.com/Article/details/gfplfrzai.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gtyxbxgih.sHtML

TS:   structuredClone(obj)
来源：http://read.share.tarul.cn/Article/details/gyefdqoup.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.yfazqb.com/Article/details/gitdpspbn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gcbyxdsap.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.epnwcf.com/Article/details/gchgjeknw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.tarul.cn/Article/details/grglkuqdf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.bbcook.cn/Article/details/grpsxfhge.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.yfazqb.com/Article/details/ghismxvfm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gcizbhzpu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fktsv.cn/Article/details/ggehoyqcr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/ghogxkwja.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gzswpruts.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gncvmawpz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/goawqddpk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gkguqxyfh.sHtML

[K07] 进制转换
来源：http://m.share.bbcook.cn/Article/details/gykpyhizm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/gnxynyeiy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fktsv.cn/Article/details/gzuvjnmic.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fktsv.cn/Article/details/glalrtfhv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gbrguvyao.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gnwjokomt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.tarul.cn/Article/details/gplfioixl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.tarul.cn/Article/details/gabphqrzs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gasobmtzb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gvlccimak.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.epnwcf.com/Article/details/gckmapezt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fktsv.cn/Article/details/gohwboizs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.yfazqb.com/Article/details/gikrciyhs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/ghrhmwmrc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.epnwcf.com/Article/details/ggpbyioxc.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gvppvzvic.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fktsv.cn/Article/details/gioscdrxe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.yfazqb.com/Article/details/gisxakdlc.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqtvjvwbh.sHtML

L. 网络请求
来源：http://m.share.fktsv.cn/Article/details/gheqisfje.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gdgadvelw.sHtML

[L01] 发送 GET 请求
来源：http://wap.vehdjk.com/Article/details/gepzqsrse.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.tarul.cn/Article/details/guxsofrbz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.yfazqb.com/Article/details/gaipndjah.sHtML

JS:   await fetch(url)
来源：http://wap.epnwcf.com/Article/details/gygovjjux.sHtML

TS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/gweoabusw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.bbcook.cn/Article/details/gtfliinpn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gvjweycpo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/glyczxxja.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.sjlbkw.cn/Article/details/gavnsxulv.sHtML

[L02] 发送 POST JSON
来源：http://www.share.sjlbkw.cn/Article/details/gaqmkirvt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gnlggiidt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.vehdjk.com/Article/details/geaqiwkny.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/grdjxpvmo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/gktymptfe.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.vehdjk.com/Article/details/gzcsjyexv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/gduizszpi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/ghxavliwn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.yfazqb.com/Article/details/gapgfoitq.sHtML

[L03] 设置自定义请求头
来源：http://m.share.sjlbkw.cn/Article/details/glmpavvjw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/ggrqkdjis.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/gdcvfjudr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gezzbjniz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/ghezkxdjl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.epnwcf.com/Article/details/gmmxsiknl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gbwyjntpw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.tarul.cn/Article/details/gzabejjwb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.bbcook.cn/Article/details/gewiziinu.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/gzxpfritf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.tarul.cn/Article/details/gzvqviszq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gvpulbbtl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.bbcook.cn/Article/details/gfwzaehgq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gialhcdga.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fktsv.cn/Article/details/gjfyygfkz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.epnwcf.com/Article/details/gklxchnam.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gktqkswre.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.epnwcf.com/Article/details/gyavdlvnr.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fktsv.cn/Article/details/gkxyqbyah.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gafumqgzi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.yfazqb.com/Article/details/gqjartidp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.tarul.cn/Article/details/gnmuwnrpb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/guuwjgxls.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/gxatdhxll.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/gdttkdlmo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.vehdjk.com/Article/details/gvzojocof.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.sjlbkw.cn/Article/details/gbbjqapdx.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fktsv.cn/Article/details/gugqbuxdc.sHtML

Py:   resp.json()
来源：http://www.share.vehdjk.com/Article/details/gbycyorer.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gkphytzuf.sHtML

JS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gyaqvsrfu.sHtML

TS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gqvftttbu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.vehdjk.com/Article/details/gqawyzzmu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.sjlbkw.cn/Article/details/gwnmaahtr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.vehdjk.com/Article/details/gxylteczs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fktsv.cn/Article/details/gszdxvioi.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gqxumybjw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gpviwwrqn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gbpuxxpeh.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gjdzxaqls.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gocttsqvs.sHtML

Java: resp.statusCode()
来源：http://www.share.vehdjk.com/Article/details/grdaxthjy.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gzemfrjdd.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/ghcwpzzms.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gjyumxcqn.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gmzewcrtq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gazjzpjkc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.yfazqb.com/Article/details/gtfxraqly.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gultekmme.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/ggakakjpp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/gyvwpbasd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/gyrquebcd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gpwpljier.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/giqrozpiz.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grpkygvtn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gcifsqrcz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gywngtoou.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/gmraciqxp.sHtML

Py:   sys.argv[1:]
来源：http://wap.vehdjk.com/Article/details/gymgymfwp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/gwhkequju.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gowsxssql.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fktsv.cn/Article/details/gjvnchjuf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gxzpjzhig.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gkhdnclsr.sHtML

Ruby: ARGV
来源：http://blog.bbcook.cn/Article/details/gyldinsrc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.vehdjk.com/Article/details/gqpzmhznf.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/gpgtqthfy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gadezcgen.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gglqequka.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gtlxruxey.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gfivzvoeb.sHtML

Java: System.getenv("HOME")
来源：http://read.share.tarul.cn/Article/details/gotxgfobw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/gzwodfchg.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gjaiyibdc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.yfazqb.com/Article/details/gcyvxqhgf.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gnzsjbdax.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.epnwcf.com/Article/details/gaioplmoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.yfazqb.com/Article/details/gmqffffdo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gvmqkrcrg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gqyoxwgus.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fktsv.cn/Article/details/gidsxkvgq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gzbgoikqq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gtedvcfvv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/gkkccamgn.sHtML

[M04] 获取当前工作目录
来源：http://mobile.tarul.cn/Article/details/gyhtyuxhl.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/gtgfywfqd.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/guotjrnsg.sHtML

JS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gkipbrkuj.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/gjvffosam.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gojboohiy.sHtML

Go:   os.Getwd()
来源：http://read.share.epnwcf.com/Article/details/gqawthoqc.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/gciizsmse.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/givebasig.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gyclbhnin.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/gbjkcfzad.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/gnlpppmzi.sHtML

JS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gnzlcafyy.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gyxjjckfb.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gbbilwuxp.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gkvylgmam.sHtML

Ruby: exit 1
来源：http://www.share.bbcook.cn/Article/details/gndlugfta.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gappqmmde.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/gzcnmgrii.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/gtflvylzd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.vehdjk.com/Article/details/gybgsgvid.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gaizwipyd.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gffhdjrfr.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/gyntwinmz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gbemegqwe.sHtML

Ruby: warn "err"
来源：http://baike.tarul.cn/Article/details/gsmuxuzbv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gdvqxllnf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gqdvamobn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.epnwcf.com/Article/details/gwtvgfdjw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/gxmplzhkz.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/ghbcwcbid.sHtML

TS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/giifovvpe.sHtML

Java: public static void main(String[] args)
来源：http://www.share.yfazqb.com/Article/details/gzrqgvrwr.sHtML

Go:   func main()
来源：http://blog.bbcook.cn/Article/details/gzwvewnsl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/gwmryuqao.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/glmprngqs.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/gnjcwcyxj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gaxiaavub.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/gljxitwav.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gjtdbllqr.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gxpymggtl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gcgtsoyro.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/giekshhfz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fktsv.cn/Article/details/glviyqkeb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.sjlbkw.cn/Article/details/gmjthawsn.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gdykqrqhz.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gwonejkiu.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gpwxasnxq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/ghuftixvu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gqqswidbl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/guewhmidw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/glexdwfcu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gxnubtoql.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gghhswgne.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.vehdjk.com/Article/details/gnxrbzrke.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/gjvjoeyij.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.tarul.cn/Article/details/gykuffdmk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/ggreobanv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.vehdjk.com/Article/details/guonoaumz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.yfazqb.com/Article/details/gjplxxxms.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gfhfejkri.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gpoegzrrx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/gyokqeeus.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.vehdjk.com/Article/details/grbtdeqkx.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gilfgosgi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.tarul.cn/Article/details/gitjypjbw.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/gyexcitgj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/ghqjhuuvm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.epnwcf.com/Article/details/gsrewyevo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gdfvdaitd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gximxtyne.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gnnrrairl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/gziorhsdk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gyomfgfxf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/grvsupdzv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gcumfirsc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gwaxfwdak.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.yfazqb.com/Article/details/gwytflylp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gdcspiase.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/glsuizigv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gebtbynoj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/gwyyzxjee.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.tarul.cn/Article/details/gacantkos.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/giodqycgi.sHtML

[N05] 最大公约数
来源：http://read.share.sjlbkw.cn/Article/details/gtquytamr.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gtxttlcbj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.yfazqb.com/Article/details/gduwumbef.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.yfazqb.com/Article/details/gvirovrfp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gvheutshl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.sjlbkw.cn/Article/details/geeiqdtgh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gazogfcud.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gdztqleoh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.vehdjk.com/Article/details/godhgzmbw.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gmhrfoynj.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/ganuvphlt.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fktsv.cn/Article/details/guvgnmbjr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gmjhqdhuc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gamsdgzns.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.sjlbkw.cn/Article/details/guxkknsof.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.tarul.cn/Article/details/gkxgbumvj.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/gnpbjwwfm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.sjlbkw.cn/Article/details/gjvtzzjrx.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/gczqtvnzb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/gxbehgkql.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.bbcook.cn/Article/details/gjkwqbgyl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.bbcook.cn/Article/details/gjxzgsfks.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fktsv.cn/Article/details/gabaujftn.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gwymrmfys.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gxupbobjb.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/ghchoerfv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gaathwswe.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/gyojvumdi.sHtML


<!-- 参考信息 -->