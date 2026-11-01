代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.yfazqb.com/Article/details/gduggirsf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.epnwcf.com/Article/details/gzzxtzned.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.tarul.cn/Article/details/gceqzmxyg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.sjlbkw.cn/Article/details/gsutdsoat.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.yfazqb.com/Article/details/guiwqkxdq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.epnwcf.com/Article/details/gzmnhrchq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.vehdjk.com/Article/details/gdhhthlea.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.vehdjk.com/Article/details/gvispgbbo.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbjlbgrfo.sHtML

K. JSON 与序列化
来源：http://www.blog.vehdjk.com/Article/details/guvgtcvoq.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gzrtmswww.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/gzymikemv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.sjlbkw.cn/Article/details/gtkycplvv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gvsapvewy.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.sjlbkw.cn/Article/details/gksxczqol.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/ghddlcmoa.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.epnwcf.com/Article/details/gnopqzhzm.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/gsvcvoqau.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gmegbaxgn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.bbcook.cn/Article/details/grwzfrgtg.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.sjlbkw.cn/Article/details/gpeqzzseg.sHtML

Py:   json.loads(s)
来源：http://read.share.fktsv.cn/Article/details/gvvobdupw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.sjlbkw.cn/Article/details/gruwbwckk.sHtML

JS:   JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/ggrimgcgr.sHtML

TS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gfcxclpei.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/gbqqstvpe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gskspccoh.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gfrshahja.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.epnwcf.com/Article/details/gzqmanggb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gpacpdoug.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.sjlbkw.cn/Article/details/gfeaydfnv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gpuvyyspn.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fktsv.cn/Article/details/giinzqqjb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gpifxnfro.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gpgipvtvj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.epnwcf.com/Article/details/goqerswhz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.yfazqb.com/Article/details/gayqajkpv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.vehdjk.com/Article/details/gzixjgnla.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/gabnppzng.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/gdpgvwezx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fktsv.cn/Article/details/gaajqbbvr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gkfaxftdr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.epnwcf.com/Article/details/glrrpjxvw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/gvnbpkrfl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fktsv.cn/Article/details/gmcilnkvl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gspxgggnp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/ggbuohzxt.sHtML

[K05] 深拷贝对象
来源：http://wap.yfazqb.com/Article/details/gpewppkin.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.tarul.cn/Article/details/gnchyipoe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.yfazqb.com/Article/details/gzhhomhct.sHtML

JS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gtdkjdgjt.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/glwyvxyze.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.yfazqb.com/Article/details/gtsdcekzq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.sjlbkw.cn/Article/details/gcxvuqofi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.sjlbkw.cn/Article/details/gomehhmbc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/gwylsujhc.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.yfazqb.com/Article/details/gqfiaxlaf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.yfazqb.com/Article/details/gxqvkehxn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fktsv.cn/Article/details/gmzgsunnx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/guczzupxh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gufwmpiji.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.yfazqb.com/Article/details/geomakchu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.vehdjk.com/Article/details/gvrryolhs.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gnjbgqpdx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/gptdgiaah.sHtML

[K07] 进制转换
来源：http://3g.vehdjk.com/Article/details/gucynzaqr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.vehdjk.com/Article/details/googwnxio.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.epnwcf.com/Article/details/gknidsljx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gbgjixpzy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gwyvieowh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/glyljgxej.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/gmtwiaddg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gnwctqmhc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gcvraccgf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/gjtljmkug.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/gcoqkdvoj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.vehdjk.com/Article/details/gernkvwpo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gvuzhxghi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gwklnwbju.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/gpfhudonb.sHtML

Go:   encoding/gob
来源：http://www.share.tarul.cn/Article/details/ghoafggey.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/goqeardbj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gqkaunsny.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gabhxjslb.sHtML

L. 网络请求
来源：http://www.m.share.epnwcf.com/Article/details/geqbkywcu.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gpcyqnmvs.sHtML

[L01] 发送 GET 请求
来源：http://blog.tarul.cn/Article/details/gdivpervc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.epnwcf.com/Article/details/ghbzhrmnv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.tarul.cn/Article/details/gwwroafjx.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gbiiigqrq.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gbjhhihha.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gikytzfhn.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.bbcook.cn/Article/details/gyvrxdxhm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gguqiteou.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.yfazqb.com/Article/details/gnpaduiuz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/ghqoxmclp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gquolkedd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/gppuwktsk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.sjlbkw.cn/Article/details/glxyzkdev.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.vehdjk.com/Article/details/gssbchxvf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.epnwcf.com/Article/details/gkwdkjalo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.tarul.cn/Article/details/gswzlasyu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/guhvfjkbi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/grtvyjwva.sHtML

[L03] 设置自定义请求头
来源：http://3g.tarul.cn/Article/details/gzzcqukti.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fktsv.cn/Article/details/ghonbwvzh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/gupkuxnox.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.tarul.cn/Article/details/getaslsse.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.tarul.cn/Article/details/gcpsbzaor.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gjihrwhpu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gmmgpwcpj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gdpkuspws.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gxvaijiar.sHtML

[L04] 设置超时
来源：http://baike.sjlbkw.cn/Article/details/gzebrnodo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/gmapxretb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gonnhnbzk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gojgbvsxn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gyuduvbkg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.yfazqb.com/Article/details/ghscsdhnf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gpdkmjkxf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.tarul.cn/Article/details/gufrrkhpb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/gpfrupolm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.yfazqb.com/Article/details/gkaymvhxz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.epnwcf.com/Article/details/giwgzexnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/gnqwctmgx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/gxdgikduf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/gtgmjmppd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.yfazqb.com/Article/details/gdvlsvshl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.tarul.cn/Article/details/guwhgcumi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gvkepfzdp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/gllxnidpy.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.epnwcf.com/Article/details/gkyouuvvu.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gvwkulbpn.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.yfazqb.com/Article/details/geshfuevg.sHtML

JS:   await resp.json()
来源：http://baike.epnwcf.com/Article/details/gdadsoydx.sHtML

TS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gwixapkej.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gwrsfsmez.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpvofefbs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/guoaxcjqm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gswmkzkto.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/gusatdajy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gyqvdsabj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gpoiskkxa.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fktsv.cn/Article/details/gvvqvxiyq.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gjbutcsiy.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/grrfltekx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/glaidpbrc.sHtML

Ruby: resp.code.to_i
来源：http://www.share.vehdjk.com/Article/details/gjmrazkho.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/gydfzlioc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gqesfgczl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gjirofbac.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gkfcuprgl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fktsv.cn/Article/details/geyhuwtcl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/gxwijivro.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.tarul.cn/Article/details/gchezxinq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gjpyxvgdc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/gofmpewhn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/ggawqfefv.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/goxwgmxvh.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.bbcook.cn/Article/details/gppsckcci.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gfqmhmiiw.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gedtgbuoz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gjfuhllyu.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.sjlbkw.cn/Article/details/gaaabypxj.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/guuauurvg.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gqxtabtuy.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gcbocibth.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/gaxifvlxx.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/gxovtujie.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gtwceaiee.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gpkvtsaos.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.bbcook.cn/Article/details/gvoawdqpv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.vehdjk.com/Article/details/gspssefql.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gcpgpbajc.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gzivylbmx.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gwsdyicdd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/ginnsyrjq.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gupgaiskn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gjvxjnhjr.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/gmhajwzad.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gudtamcfn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gcsenioai.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gulewnqok.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gmbpawdjx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.yfazqb.com/Article/details/gcbltuylw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.epnwcf.com/Article/details/glbmoxcvg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.vehdjk.com/Article/details/gthylzyqt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gyyzvuzoo.sHtML

[M04] 获取当前工作目录
来源：http://www.share.bbcook.cn/Article/details/gegiqnrna.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/guxoyozok.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/gosschlma.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/guaxphjdv.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gyrnzwyyc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.vehdjk.com/Article/details/gosgsheai.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gmlsaqkzn.sHtML

Ruby: Dir.pwd
来源：http://m.share.epnwcf.com/Article/details/gqgsmpcvb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/gyjcbkzex.sHtML

[M05] 设置退出码
来源：http://mobile.vehdjk.com/Article/details/gevqcmuts.sHtML

Py:   sys.exit(1)
来源：http://www.share.epnwcf.com/Article/details/goxgeprvv.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/goepvvvon.sHtML

JS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gocrzdjta.sHtML

TS:   process.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gaidsgiil.sHtML

Java: System.exit(1)
来源：http://blog.vehdjk.com/Article/details/gmhlixcot.sHtML

Go:   os.Exit(1)
来源：http://read.share.fktsv.cn/Article/details/gkgxznfoj.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/gwiapiwmm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gexzrztvb.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gvfzzmlyz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gfggbmuaz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/gmwokeuis.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gdvuhtisl.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gmtmwcjqf.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/ghzfgbijb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fktsv.cn/Article/details/gemwmeegd.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gzwolkhmr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.bbcook.cn/Article/details/gdcmgfxnd.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/gsvnyouzd.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gjgruuvje.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/gchhphtcx.sHtML

JS:   require.main === module
来源：http://mobile.tarul.cn/Article/details/gjcqifxjw.sHtML

TS:   require.main === module
来源：http://www.blog.sjlbkw.cn/Article/details/gycxuhqdq.sHtML

Java: public static void main(String[] args)
来源：http://wap.fktsv.cn/Article/details/gyniirkyf.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gmkirhdgx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.vehdjk.com/Article/details/gvqcrjrmw.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gbwsbzpss.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gxbveaknf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.epnwcf.com/Article/details/gibddovip.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fktsv.cn/Article/details/gqskngznx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gdhecxitp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gxknulxmo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gwwnffpfz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.vehdjk.com/Article/details/gcdlvbrgt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gamrqrgdo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.vehdjk.com/Article/details/guuxutobi.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzknocaon.sHtML

N. 数据结构与算法
来源：http://read.share.bbcook.cn/Article/details/gxjiollhu.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkunkvure.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gnqzyruzw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gljfufhzv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fktsv.cn/Article/details/guaehjfzz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gxvlynlmk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gqfvryvgl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gpbiccyqp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gelzhsdpn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.yfazqb.com/Article/details/gabnqyryv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gprsrikfl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/guylfnfgc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/gjoxnqoda.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.tarul.cn/Article/details/gfycfrkeh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gnruaccem.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/gaczagxwe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gnatnpyid.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gbenmclbm.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gkgnximef.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.sjlbkw.cn/Article/details/gkbovlall.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gzvxbmhau.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gymfwqvoo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gfwuyreyq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gjhdklmle.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gvncjnuko.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gujiabrjf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.sjlbkw.cn/Article/details/gaszpviuw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/gmuusuuyn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.yfazqb.com/Article/details/gldrsmrez.sHtML

[N04] 斐波那契数列
来源：http://wap.yfazqb.com/Article/details/gojqrnejd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gjgmopdwr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gjqopdwez.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gqhaakcfk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gndhcmifw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gjvaacngr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gjljnfids.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gukbwizww.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gtdirknra.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gnicvjdop.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gnfdgsyzf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gzxgsufvz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gclvtjjrc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/glxulbrhj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gymewrerq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.sjlbkw.cn/Article/details/geemkbqvy.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.vehdjk.com/Article/details/ggiqgwobw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gubficuov.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/gdlkhymxa.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gqedumicg.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.tarul.cn/Article/details/ghodmptep.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gffkwjiep.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gqhovhzwj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.tarul.cn/Article/details/gmujlxfdh.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/ghoejefvo.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/gbktbgiup.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.vehdjk.com/Article/details/gqnyfiquq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/grmzonagn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfnxvbxu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gkwhrlatp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.epnwcf.com/Article/details/gattuuilb.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gisgwnamg.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gklcblpsy.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gaacqkbjb.sHtML

Ruby: // 手写 Hash
来源：http://wap.yfazqb.com/Article/details/gtsjjcjmw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gwjljqezz.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/ghytisykh.sHtML


<!-- 参考信息 -->