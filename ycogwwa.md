代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.epnwcf.com/Article/details/gdezelgnm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.yfazqb.com/Article/details/gdysdexoj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.bbcook.cn/Article/details/gschsgpiz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.sjlbkw.cn/Article/details/ghavpompd.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gpwpgmsus.sHtML

K. JSON 与序列化
来源：http://read.share.tarul.cn/Article/details/gcicovmsh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gamuarexw.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fktsv.cn/Article/details/ghprqvawp.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/gwuurbruk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/grgimtrre.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.bbcook.cn/Article/details/gsdbmzrgy.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.sjlbkw.cn/Article/details/gelyrmzmu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.bbcook.cn/Article/details/gsjmxpfif.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/giuyxmtpq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fktsv.cn/Article/details/glrufyaee.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.vehdjk.com/Article/details/gkjgntmgp.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.tarul.cn/Article/details/gsthsrsuc.sHtML

Py:   json.loads(s)
来源：http://www.blog.vehdjk.com/Article/details/ggbpuihue.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.tarul.cn/Article/details/gxcqiunja.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/guxgvpilu.sHtML

TS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gmlpvolra.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/ggiwtdoad.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gcavysotx.sHtML

Ruby: JSON.parse(s)
来源：http://blog.bbcook.cn/Article/details/gaajzzgbm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/gtrmmbkot.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.yfazqb.com/Article/details/gawwudxiz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.vehdjk.com/Article/details/golyfevsv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.yfazqb.com/Article/details/gcbrwdysh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gggyftvib.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gsnqxpsbm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.yfazqb.com/Article/details/gimddwcdt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.sjlbkw.cn/Article/details/gkcokoujw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gohnhiohy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.bbcook.cn/Article/details/gnsykbczu.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fktsv.cn/Article/details/gsmpudibs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.bbcook.cn/Article/details/gkgnxcnhj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.vehdjk.com/Article/details/gynxymyyo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.yfazqb.com/Article/details/gkaukxdtl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.sjlbkw.cn/Article/details/gplpuaqth.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/gtgxvgdgk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.bbcook.cn/Article/details/gisyxoobr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gcxgsvpdo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fktsv.cn/Article/details/geocvpaba.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/gpipjyifh.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gzakldkxn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.yfazqb.com/Article/details/gtpieozoo.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gkuiydelk.sHtML

TS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/grtxlzovt.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gakgqjtzy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.tarul.cn/Article/details/gtldyxcek.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.vehdjk.com/Article/details/gizefpsbc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fktsv.cn/Article/details/gwuxpsjus.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.vehdjk.com/Article/details/gcgjjrzlw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.bbcook.cn/Article/details/glhvljaum.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fktsv.cn/Article/details/gkeeccaro.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.sjlbkw.cn/Article/details/gtfmvymxu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/ghlbtddar.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.vehdjk.com/Article/details/gwprvpmnc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gkarhxkub.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gqrllrvms.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.epnwcf.com/Article/details/guztuhulh.sHtML

[K07] 进制转换
来源：http://m.share.tarul.cn/Article/details/gdwycphnx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gqwewjnvn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gchzjhoaf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gsmqqpkqf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gqjqzuipl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gcmemqlnv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.epnwcf.com/Article/details/gglfdxsfr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.yfazqb.com/Article/details/gcdfeivgp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/grrcbpqsz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.yfazqb.com/Article/details/gfwadmqay.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.bbcook.cn/Article/details/gjhxledav.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.epnwcf.com/Article/details/gdncnjdkd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.epnwcf.com/Article/details/galvzancw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gmyzoyiif.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.yfazqb.com/Article/details/gytmkwgfn.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gzsdqunjg.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.bbcook.cn/Article/details/gmutikzyb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.yfazqb.com/Article/details/gemscuybj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gyqdafxek.sHtML

L. 网络请求
来源：http://m.share.vehdjk.com/Article/details/gtobvrxxd.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gxvcdhfbd.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gcarmbbxe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.bbcook.cn/Article/details/gojcuouyi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gafshjexs.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gstohhkuh.sHtML

TS:   await fetch(url)
来源：http://m.share.tarul.cn/Article/details/gybiczfdx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gxwgjepzn.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.bbcook.cn/Article/details/gapkfapco.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gomdpjzcm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gjhehgpea.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.yfazqb.com/Article/details/guuilqige.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gdqxssrqo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.vehdjk.com/Article/details/grbyxrrkj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.bbcook.cn/Article/details/gcklhnttl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gazwztcxl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.bbcook.cn/Article/details/gnrkmmeqy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gkczuqfjk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fktsv.cn/Article/details/gagjxzsxx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.yfazqb.com/Article/details/gbqsgojzh.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/giddmzozf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gdcehabpv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/giuhdylot.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gadlnhmos.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.epnwcf.com/Article/details/gvfuggeey.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/gltoasbsg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gdsctofhi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gprgfvhdi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gubobkmzd.sHtML

[L04] 设置超时
来源：http://wap.sjlbkw.cn/Article/details/gtiodljmp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gcvwjmrex.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.tarul.cn/Article/details/gxpbwinhh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/grptiddzl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fktsv.cn/Article/details/gojdqoloh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.tarul.cn/Article/details/gadnnthhc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gammjakzp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.epnwcf.com/Article/details/ghiaffnoe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.yfazqb.com/Article/details/guxyeuyrh.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/gryurvonb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.epnwcf.com/Article/details/gxcjcovil.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/gshuwsglf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.bbcook.cn/Article/details/guruwnhqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gguvzrrfu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gebqntzbq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gegeclafj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.sjlbkw.cn/Article/details/gmstmwjhq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gylanozyu.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gmukhbduq.sHtML

Py:   resp.json()
来源：http://www.share.yfazqb.com/Article/details/gjpqzuuoz.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/glxcxawxe.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gfzhiwuts.sHtML

TS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gfnypzkhh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gdvgwqtsm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.epnwcf.com/Article/details/gamvlmtbi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gysycnhat.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggswjidip.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gvdwxmsxd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.bbcook.cn/Article/details/gcsviegbi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.tarul.cn/Article/details/glrnaluth.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gudcooszt.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gfqjyveym.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/gyhzlrocs.sHtML

Go:   resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gssxufimp.sHtML

Ruby: resp.code.to_i
来源：http://m.share.bbcook.cn/Article/details/gmvkjkpjn.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/ggcpbrpnm.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/grpqrtape.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/gjbmzgwoo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.yfazqb.com/Article/details/gbcymhjvd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.bbcook.cn/Article/details/ggtcxpbnv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gxmkqbrph.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.bbcook.cn/Article/details/ghxevmfeu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fktsv.cn/Article/details/gmbimsopr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fktsv.cn/Article/details/guacuxhnv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gnyfpxwpp.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gcbjopoks.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gyrcnsltl.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gszewlmex.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/glcfuvnsv.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gwdwccyvv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fktsv.cn/Article/details/grblvwppn.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gufgssiac.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/ggirujbtp.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.vehdjk.com/Article/details/gixnjmvdi.sHtML

Go:   os.Args[1:]
来源：http://blog.yfazqb.com/Article/details/gsepybktj.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/gbytsoems.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gwzdxgief.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/gumumeesi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gbqsttppu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.tarul.cn/Article/details/grzrnazxo.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/gakhqpxnx.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gowbjxfon.sHtML

Java: System.getenv("HOME")
来源：http://3g.fktsv.cn/Article/details/glumfkrgd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gltoqvcmt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gskdhrwab.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gnegecheg.sHtML

[M03] 执行外部命令
来源：http://www.blog.tarul.cn/Article/details/geeikggxl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gilvmodfv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gyxdlkbgj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/guaquqhrw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gymximjhw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gxpecgxur.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gnladvwua.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.tarul.cn/Article/details/gqypcjplx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/glsjydadn.sHtML

[M04] 获取当前工作目录
来源：http://blog.tarul.cn/Article/details/gxbsqyxat.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gvofyzdel.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/gpbnnazos.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gqtazxdkf.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gnjfygbnu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.vehdjk.com/Article/details/guhclzsaw.sHtML

Go:   os.Getwd()
来源：http://baike.sjlbkw.cn/Article/details/gmxvmdkdd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.bbcook.cn/Article/details/gklsrtndy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/giwwjxmbr.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/ginonqblm.sHtML

Py:   sys.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gogiszlxk.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gkvgnbxzd.sHtML

JS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gjoprkzfv.sHtML

TS:   process.exit(1)
来源：http://3g.vehdjk.com/Article/details/guabfgggm.sHtML

Java: System.exit(1)
来源：http://wap.fktsv.cn/Article/details/guyovorxl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gjravyrdy.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/gwrxspatl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.yfazqb.com/Article/details/gqdmafsxz.sHtML

[M06] 向标准错误输出
来源：http://m.share.bbcook.cn/Article/details/grsefytbj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gizbkxrwx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.sjlbkw.cn/Article/details/gboyyyokn.sHtML

JS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gstdooulk.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/giqdiywho.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gaiydwkaf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/gtcvtwiek.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gtgygkhka.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fktsv.cn/Article/details/gfmuobgsh.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/gwhuemtkf.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gaxuphhyx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gnbfurhsv.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/gamiyaefa.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/gbyjcbfrt.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gbnfozpqn.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gpscdehpa.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.epnwcf.com/Article/details/gkddayatu.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gtezujnku.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/gulmzanqq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.tarul.cn/Article/details/gshvyphcq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.epnwcf.com/Article/details/gglepsdkg.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gekxaezwt.sHtML

TS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gjgbermdp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/ggfasergx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/gfewtwvgd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gvsifucyw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.vehdjk.com/Article/details/gqesishsu.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gvqapitnw.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/gspwcvqqa.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gpszqcixr.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/gnvmxzygj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/glggqqahd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gyohgukmi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gdbehugks.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gqoeocfpw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gqmwltzcm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/glxyugcva.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gwjselfpx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gnoerukmh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gfezsbaea.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gpueqjcqg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gmlyolpuq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/goxxpuqhb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gqeczumap.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.yfazqb.com/Article/details/gtifzupms.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gbawsgrsj.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/gajdfckbb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.yfazqb.com/Article/details/gwqglduho.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/gciwgpqxj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gmovlnarm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/ggudfxdxd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gcjychfhx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gzvoiemtg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.tarul.cn/Article/details/gowzjjxyk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.sjlbkw.cn/Article/details/gwfqschqb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gxlwudubv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gndbnmjrr.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gaeampeph.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/ginvnhwig.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gvlqbuvob.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/grwvrmizv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/ghcrfpsfq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gjpfyywkv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/gbjhgyzoz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gxyvdzofk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/gzpauuwvn.sHtML

[N05] 最大公约数
来源：http://wap.sjlbkw.cn/Article/details/gvssrklmx.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gkpmoamaw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.tarul.cn/Article/details/gdoihmxod.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/geiihhjxn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gvorpeipy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.yfazqb.com/Article/details/gcbhilwee.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/grughvmbi.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gtqbolyck.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gyccwqoga.sHtML

[N06] 判断回文字符串
来源：http://m.share.yfazqb.com/Article/details/goqibmidc.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/gkxttxdzi.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gkzblhsyn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gqnryhuwa.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gvuivthfz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gfvvypfjz.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gkmhnxybn.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/glvyvrdln.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gswgkamqe.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gcjoqenol.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gfyghcnra.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fktsv.cn/Article/details/gxqlyutip.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/gwywnebzk.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.epnwcf.com/Article/details/gsugrwynt.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gohhlkklj.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/grxzvdlmn.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gsijfggvu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.bbcook.cn/Article/details/gozojduco.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gxsjnpzyz.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.yfazqb.com/Article/details/gqqdmyxgi.sHtML

PHP:  // 手写递归交换
来源：http://m.share.vehdjk.com/Article/details/gdkaqdljp.sHtML

JS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gzkyqries.sHtML

TS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gzzeeqhzy.sHtML


<!-- 参考信息 -->