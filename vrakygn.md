代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fktsv.cn/Article/details/grghsesuq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.bbcook.cn/Article/details/gfyvowzxa.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.bbcook.cn/Article/details/gjhchjwto.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.tarul.cn/Article/details/gmwyfeqvn.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gvupwkaln.sHtML

K. JSON 与序列化
来源：http://3g.vehdjk.com/Article/details/gmcuifyol.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gebsoeszh.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.sjlbkw.cn/Article/details/ghjmjtrlv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.bbcook.cn/Article/details/grlbejrkd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.epnwcf.com/Article/details/gjyxaiekh.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gkeymkjun.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gdzywgyvg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.tarul.cn/Article/details/gobuauckb.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.vehdjk.com/Article/details/gutidfywv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.epnwcf.com/Article/details/glckoxbwq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.tarul.cn/Article/details/gkdgmygxx.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fktsv.cn/Article/details/ghhjgopts.sHtML

Py:   json.loads(s)
来源：http://blog.fktsv.cn/Article/details/gllpzbobp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.vehdjk.com/Article/details/gfevfkrki.sHtML

JS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/gxopidljs.sHtML

TS:   JSON.parse(s)
来源：http://wap.epnwcf.com/Article/details/gxaoksvqb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.yfazqb.com/Article/details/gxsskojxz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/grbzznlgd.sHtML

Ruby: JSON.parse(s)
来源：http://wap.vehdjk.com/Article/details/ggjxnppla.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.vehdjk.com/Article/details/gynpxtixm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbxpbrvj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/garixbhpn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gpvoqjwhq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fktsv.cn/Article/details/gyozkooqc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gtbrmubpz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.epnwcf.com/Article/details/gbaihdcul.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.sjlbkw.cn/Article/details/gmklhxqqx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gnrngwdrh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.tarul.cn/Article/details/glrwaepvt.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gwcqophwg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.bbcook.cn/Article/details/gfnqmkrub.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.sjlbkw.cn/Article/details/gztlivbxa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.sjlbkw.cn/Article/details/glifjggdb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/gunjpqgtp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.epnwcf.com/Article/details/gsdhtyvzz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/giyhmtigq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.bbcook.cn/Article/details/ggotlcfbx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.tarul.cn/Article/details/gzfmlujey.sHtML

[K05] 深拷贝对象
来源：http://www.blog.bbcook.cn/Article/details/gspeuqlki.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.sjlbkw.cn/Article/details/gfklfhuhu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/glqnteokx.sHtML

JS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gfdspsfgy.sHtML

TS:   structuredClone(obj)
来源：http://blog.vehdjk.com/Article/details/gybfyoygw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.tarul.cn/Article/details/gjvyzcwzz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.sjlbkw.cn/Article/details/gfnlbsasi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.sjlbkw.cn/Article/details/gtrdfhbmo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.sjlbkw.cn/Article/details/gccwbtmyx.sHtML

[K06] 解析 URL 查询串
来源：http://3g.bbcook.cn/Article/details/gjnzwzpxw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/gfvodatij.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/gbuaqbend.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.tarul.cn/Article/details/gexdlwbhi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/gnvgytmxd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.vehdjk.com/Article/details/gajgarvhw.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.bbcook.cn/Article/details/gqnhpjgwc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gtxflyoyk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/gqwtxuuch.sHtML

[K07] 进制转换
来源：http://m.share.yfazqb.com/Article/details/gpgbjprnq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gacwqawyf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.bbcook.cn/Article/details/gnenqvghp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/ggxjovhvr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gedpovopa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gwtvrxeza.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fktsv.cn/Article/details/gjcgnxyjc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gcztxxvin.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.tarul.cn/Article/details/gzwiolrph.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gshhgjyiw.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.tarul.cn/Article/details/gzxlwrdwj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.sjlbkw.cn/Article/details/guzmdhbpp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/gauzidvas.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.tarul.cn/Article/details/gmnacwkci.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/gvijekona.sHtML

Go:   encoding/gob
来源：http://wap.sjlbkw.cn/Article/details/gxcvjnvgn.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.epnwcf.com/Article/details/gouzyzotk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gpyhvcvjv.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gloyvjqfx.sHtML

L. 网络请求
来源：http://baike.epnwcf.com/Article/details/gfhezknxh.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/ggldxlfyb.sHtML

[L01] 发送 GET 请求
来源：http://mobile.bbcook.cn/Article/details/ghharmqrj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.yfazqb.com/Article/details/gcsqzgtef.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.tarul.cn/Article/details/gkbntslya.sHtML

JS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gkihglfar.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gtwocyqwv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.epnwcf.com/Article/details/gjbnwdvui.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.vehdjk.com/Article/details/gyyuigcll.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.vehdjk.com/Article/details/gdawdsjno.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.tarul.cn/Article/details/gpxqqsuxv.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gtmpoybje.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gngwxersz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fktsv.cn/Article/details/ggclbjewo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/gmkcvdrck.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.yfazqb.com/Article/details/glwcopqcr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fktsv.cn/Article/details/gzysajdry.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.epnwcf.com/Article/details/glhribmol.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.yfazqb.com/Article/details/gjyellrlh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fktsv.cn/Article/details/gaydfktxd.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.epnwcf.com/Article/details/glztkpsmv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/gzurkxieg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gyefwnogk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/gxchzgqsc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gonuezcum.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gmzracguh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.vehdjk.com/Article/details/gnyezhfnh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fktsv.cn/Article/details/gxeomndop.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gnblfjymu.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gimavgfbt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.vehdjk.com/Article/details/gjxnijdid.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.bbcook.cn/Article/details/gyyghraxa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/guatiezww.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.yfazqb.com/Article/details/gscfdewmb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.tarul.cn/Article/details/gvyujjwhm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.epnwcf.com/Article/details/gmpqscyvd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.vehdjk.com/Article/details/gkkljzfmy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.bbcook.cn/Article/details/grjlotnmk.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fktsv.cn/Article/details/gbwrzcfbz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.sjlbkw.cn/Article/details/glnbduulf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.vehdjk.com/Article/details/ghfnpajib.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/glqakskjz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gxuglezfh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.epnwcf.com/Article/details/giuhypfjc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gwnqilsbf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fktsv.cn/Article/details/gblnpfxtk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.bbcook.cn/Article/details/gvukigriq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.bbcook.cn/Article/details/gmeuhdpvr.sHtML

Py:   resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gnqncztyi.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.bbcook.cn/Article/details/ggltavcal.sHtML

JS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gwqyuogqz.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gweodmwrr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gptdjntja.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.epnwcf.com/Article/details/gzenaiolg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/gzcgwmikx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gqlfuarrf.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fktsv.cn/Article/details/gklrsjhri.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.sjlbkw.cn/Article/details/gdpbymrqm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.epnwcf.com/Article/details/gwfyfnhjy.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.yfazqb.com/Article/details/gxudyodiz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrealqhd.sHtML

Java: resp.statusCode()
来源：http://3g.tarul.cn/Article/details/gjbzsxmjl.sHtML

Go:   resp.StatusCode
来源：http://blog.fktsv.cn/Article/details/guerrnjeo.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/gjtdjgqeu.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gfculyndi.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gorjewgdm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.yfazqb.com/Article/details/gzzkfqbmg.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gppharoyq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gmmrqgvtu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/gupifqmtu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gmcdzduhw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fktsv.cn/Article/details/gsjkeywre.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fktsv.cn/Article/details/grymbizdm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.yfazqb.com/Article/details/gkdzeaatk.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxoonjkyv.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gqxnwymcr.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gmzbmworj.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fktsv.cn/Article/details/gfcklhrqu.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gyrhcdtil.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.bbcook.cn/Article/details/gwupsrwrd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gskzkyzdw.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gzvuxknyw.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gailjivbo.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gbmaflpaa.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gqtkpyakz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gokixcmnq.sHtML

[M02] 读取环境变量
来源：http://3g.bbcook.cn/Article/details/gahbbavel.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gcylxnewz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gfumdmera.sHtML

JS:   process.env.HOME
来源：http://www.share.bbcook.cn/Article/details/galrnsgxw.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/guqnzresv.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gxbhqsvjm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gtsheufol.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gbrcglias.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gcvrymmcl.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/gllaespdp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/gfjxwthex.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fktsv.cn/Article/details/gcsvjioec.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gprvbzdiy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gplquvoct.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/giuzuvdgr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fktsv.cn/Article/details/glaqscpey.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.epnwcf.com/Article/details/ghxgciuog.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gnitrufgx.sHtML

[M04] 获取当前工作目录
来源：http://3g.vehdjk.com/Article/details/gewvopkos.sHtML

Py:   os.getcwd()
来源：http://www.blog.epnwcf.com/Article/details/gcpqsetpd.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/gxvplpews.sHtML

JS:   process.cwd()
来源：http://3g.fktsv.cn/Article/details/gfgjjfeyl.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gihvmzrht.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.sjlbkw.cn/Article/details/gawwoyive.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gofgezema.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gwgeeajms.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gozmzjivi.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gfwdlwpyi.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gbhturirj.sHtML

PHP:  exit(1);
来源：http://mobile.fktsv.cn/Article/details/gmbgdhlqd.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gmlovmlmm.sHtML

TS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gpmunoqca.sHtML

Java: System.exit(1)
来源：http://wap.epnwcf.com/Article/details/gwdlrpcnx.sHtML

Go:   os.Exit(1)
来源：http://m.share.epnwcf.com/Article/details/gsrqzwtiu.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gookoymya.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.yfazqb.com/Article/details/gbfwkyqyb.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/gctijtkwn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gxzidsmnt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gqubpymwh.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gtczumxtw.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/ghrlfsuyt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gdgpdqeew.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.vehdjk.com/Article/details/gkxbhkkka.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gzpnxadls.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gwwvfttwa.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/gpmwkkiqr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gtjwgjxbc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.sjlbkw.cn/Article/details/gdbsqpgnz.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gsmbfrzvs.sHtML

TS:   require.main === module
来源：http://www.share.tarul.cn/Article/details/gnmusfhvh.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gaqkuvfut.sHtML

Go:   func main()
来源：http://mobile.epnwcf.com/Article/details/galprokvc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/ghbmkuohf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/guitrczbf.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.bbcook.cn/Article/details/gibmiyjvm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/ghyazgzaz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fktsv.cn/Article/details/gtszhejte.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gioqdzzvf.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gdlopogjm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcltffkqh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.tarul.cn/Article/details/gluwdkmyg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/gvrxlyyya.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gxfcdbgms.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gaqfjavjf.sHtML

N. 数据结构与算法
来源：http://mobile.yfazqb.com/Article/details/gfmzbmlrp.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gkbhdfpcx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gfnoluuwu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gzsfrhxfv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.vehdjk.com/Article/details/gcikporxh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gedvjwuqq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/gaovoshtw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gwnldvanl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/geihadspx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.sjlbkw.cn/Article/details/gwsoginpl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/glzffiajo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.sjlbkw.cn/Article/details/gbjjojcmr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/gdjuupwgw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.yfazqb.com/Article/details/gasebgjfe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/gjvbiraoy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gjnnjsyju.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gjpvxtcdq.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gjdyyqaen.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gepmmzbvu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.bbcook.cn/Article/details/grgoxcqvu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gwxjpwlhm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gmvlpajhq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gsmbbquss.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/gldealagh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfkpqzlq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gidaqvugb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gryczaqaa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/gyrtjdxdb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gpvlzitfm.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/ggffgdcht.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gjciavjta.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gxfpizqrh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/ghvbkjskj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gksjadmej.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/grwyufgbn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.yfazqb.com/Article/details/gjqbjbrav.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gluplpewg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gwkdaygxi.sHtML

[N05] 最大公约数
来源：http://mobile.vehdjk.com/Article/details/gsemxloka.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.tarul.cn/Article/details/gjvuiwyxc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.vehdjk.com/Article/details/gbvhcwttj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/geyqfhrec.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gccfzczac.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.tarul.cn/Article/details/gotmwujzs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.yfazqb.com/Article/details/gooxzzxdw.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.epnwcf.com/Article/details/glhdkbgta.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fktsv.cn/Article/details/ghvobajjl.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/gepyoddyv.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/gazboadhq.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.epnwcf.com/Article/details/ghfbrhkgf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gpkvluzsx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gqianxmtp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gnxgtetul.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.sjlbkw.cn/Article/details/gueoeyzho.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gvcprpesn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gczecetzg.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/gbgphdfww.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.yfazqb.com/Article/details/gsnynjfir.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gplqxplzj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/gmcumswmb.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.bbcook.cn/Article/details/gxbmmkiwa.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/gjqyywdpu.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.vehdjk.com/Article/details/gpuvowohu.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gfnhfaxap.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/gykpxvdki.sHtML

[N08] 生成全排列
来源：http://read.share.sjlbkw.cn/Article/details/gcckiabwf.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fktsv.cn/Article/details/guqmoqjom.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/gywxhhifn.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gokcjrbzq.sHtML

TS:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/ghhrgviuy.sHtML


<!-- 参考信息 -->