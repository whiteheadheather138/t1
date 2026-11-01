代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.yfazqb.com/Article/details/grjptxtsh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.yfazqb.com/Article/details/ghwcftzjv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.sjlbkw.cn/Article/details/gbgcgodts.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fktsv.cn/Article/details/gdiilnran.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gjlnulftq.sHtML

K. JSON 与序列化
来源：http://read.share.bbcook.cn/Article/details/gjrcmtkyk.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gpwquedlm.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.sjlbkw.cn/Article/details/gwnpjjqbz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.sjlbkw.cn/Article/details/ghoqyplfy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gswsodaza.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.vehdjk.com/Article/details/gatzjznig.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.yfazqb.com/Article/details/goblyqheg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.epnwcf.com/Article/details/glbhcaqhk.sHtML

Go:   json.Marshal(obj)
来源：http://blog.epnwcf.com/Article/details/gxpiwuprv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.vehdjk.com/Article/details/gqxtqixdh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gyfumetiu.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fktsv.cn/Article/details/gxqiecjfa.sHtML

Py:   json.loads(s)
来源：http://3g.sjlbkw.cn/Article/details/grryjlpiq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fktsv.cn/Article/details/gjayruipl.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gmgmljoxe.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gudbtdngx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fktsv.cn/Article/details/gxgkqvbnr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gyeayiptn.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.tarul.cn/Article/details/gkwtiyfhp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.vehdjk.com/Article/details/gfgjnvdus.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gsgzwimas.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fktsv.cn/Article/details/gpgplrhkd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.yfazqb.com/Article/details/gyjvwjvqa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fktsv.cn/Article/details/guvbkkrgv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.bbcook.cn/Article/details/gsvbpznue.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.tarul.cn/Article/details/gaxulibmc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.yfazqb.com/Article/details/gmpuypxqn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fktsv.cn/Article/details/gnexttvdu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.epnwcf.com/Article/details/gygqwlfti.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.sjlbkw.cn/Article/details/ggytewhxa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fktsv.cn/Article/details/gzbaeqapd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fktsv.cn/Article/details/gvlqsfzvy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.vehdjk.com/Article/details/gtrkqtadt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gtpjhzajw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.tarul.cn/Article/details/gkpttvazy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/griilezep.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/gaqftieao.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.epnwcf.com/Article/details/ghrpvhzvu.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/gdkhhiqwx.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fktsv.cn/Article/details/gdggiotnz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.yfazqb.com/Article/details/ggztopnzc.sHtML

JS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gmnkunkyc.sHtML

TS:   structuredClone(obj)
来源：http://read.share.epnwcf.com/Article/details/gowaoppwc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.tarul.cn/Article/details/gvnequren.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.yfazqb.com/Article/details/gqnejntai.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.yfazqb.com/Article/details/giarytfjd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.sjlbkw.cn/Article/details/grbykkahu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/goqrahjap.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.yfazqb.com/Article/details/ggmwbbmss.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.sjlbkw.cn/Article/details/gozxiplqn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.yfazqb.com/Article/details/gnyjsdpit.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.yfazqb.com/Article/details/gbjhutoeg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gmyomtbcv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gbeejrtby.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/ghdbbsdxy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gbyorcqlh.sHtML

[K07] 进制转换
来源：http://3g.epnwcf.com/Article/details/glnebcumi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/ghzxpexzf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.vehdjk.com/Article/details/gncyzryxs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gcobjsqma.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/groxwhtui.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/gdroxgmfw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.tarul.cn/Article/details/gblhgzloq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gqkgfzzcf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gfdgcliyb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.bbcook.cn/Article/details/gbfiaecaa.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.sjlbkw.cn/Article/details/grguabwzi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.vehdjk.com/Article/details/givmpnass.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gdlpintoj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/gsygdeorr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.bbcook.cn/Article/details/glejmjydf.sHtML

Go:   encoding/gob
来源：http://mobile.tarul.cn/Article/details/gmpliqnou.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fktsv.cn/Article/details/ggwyrqfnq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.vehdjk.com/Article/details/gdislitdv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gkchjnadc.sHtML

L. 网络请求
来源：http://m.share.bbcook.cn/Article/details/gcxyxegmu.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gmcycvjgb.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/gwjybnaha.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.vehdjk.com/Article/details/gchjeqoqg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.yfazqb.com/Article/details/gwfuqiquj.sHtML

JS:   await fetch(url)
来源：http://m.share.epnwcf.com/Article/details/giobmfovt.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gpcrcfoje.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.tarul.cn/Article/details/gepkjrtjr.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.tarul.cn/Article/details/glgyynvhv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.yfazqb.com/Article/details/gjwjjkslx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/ghmfuqmks.sHtML

[L02] 发送 POST JSON
来源：http://3g.yfazqb.com/Article/details/gyxdswrms.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.vehdjk.com/Article/details/gyhjrvhze.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/ggenguoad.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gmtrmjwya.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.bbcook.cn/Article/details/gbwepdjpk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.sjlbkw.cn/Article/details/gzkitvpfo.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/gdwpzgnzu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gnicnfwwg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gdxiaqsyx.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.vehdjk.com/Article/details/gjcmvburp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/gddaqjuac.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/gwxoflacx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gtjvuubtc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.vehdjk.com/Article/details/gktjcstvc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gqcurmhgs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.tarul.cn/Article/details/guepuyqwl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fktsv.cn/Article/details/gqjlynqsw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gtqdeevvw.sHtML

[L04] 设置超时
来源：http://wap.tarul.cn/Article/details/gnqpwjgfv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.bbcook.cn/Article/details/ggmhxahod.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.epnwcf.com/Article/details/gjcvoblvs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/gsftikmiq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.tarul.cn/Article/details/gdrjxclvo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.vehdjk.com/Article/details/ggpfzpblz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.epnwcf.com/Article/details/gpauvdxiw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.bbcook.cn/Article/details/ghqzegrov.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/gdusraduo.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.sjlbkw.cn/Article/details/gtokowocf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/gkynphhjr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.bbcook.cn/Article/details/gkpynsdrv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/gnexetcff.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gkbjtvvko.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.epnwcf.com/Article/details/grybvbgbs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gfrbjvbhe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/gjcahzgae.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.vehdjk.com/Article/details/gskbvxeec.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gumbnsfln.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/giguiboxh.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.epnwcf.com/Article/details/gunmuucgs.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gkvydgwsv.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gbhwbvsan.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/ghgaoqxzq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gnqzqmxde.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.sjlbkw.cn/Article/details/gcneously.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.vehdjk.com/Article/details/gqclzfalh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gdgylmnfx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/gpromilkc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gbrdseoyr.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gqsecwnlh.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/guqfamdse.sHtML

Java: resp.statusCode()
来源：http://www.share.bbcook.cn/Article/details/gpslxpdzi.sHtML

Go:   resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gzixghghy.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gvwvfjwjj.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gofvqozuc.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/ghnofftww.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gyibreuph.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gdwzppike.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnwkliql.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gjjpqvrvc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.bbcook.cn/Article/details/gckcvsnpi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.tarul.cn/Article/details/grjozcoai.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/gibgeztad.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gfggleiwz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gchigtjhm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gkbkccqun.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gtkkrixgn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.sjlbkw.cn/Article/details/gbiahwzze.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gbrwrqzcs.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gkzravvnt.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/gedacjqnu.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gvrqeoshy.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gdnpsehrs.sHtML

Go:   os.Args[1:]
来源：http://blog.bbcook.cn/Article/details/gfymowbwb.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/gvpinsoav.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/ghqwvshhm.sHtML

[M02] 读取环境变量
来源：http://mobile.bbcook.cn/Article/details/gsbuxkknl.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gfodmzyka.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.epnwcf.com/Article/details/ghkojubbj.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gaqrczhmg.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gnltfyalo.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/gehqhenbd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gaabwnrsa.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.bbcook.cn/Article/details/gxngwxqvd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gulknezxy.sHtML

[M03] 执行外部命令
来源：http://www.blog.fktsv.cn/Article/details/guyenjlvc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.bbcook.cn/Article/details/gtnafrelm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gopstttnx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gdfgumzbm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gxinyqamz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gejqrnomi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fktsv.cn/Article/details/gpxzyqvqj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/gkbpvohhk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/gxznyovfd.sHtML

[M04] 获取当前工作目录
来源：http://m.share.vehdjk.com/Article/details/gephlnyxy.sHtML

Py:   os.getcwd()
来源：http://www.share.yfazqb.com/Article/details/gndealetg.sHtML

PHP:  getcwd();
来源：http://baike.fktsv.cn/Article/details/gpqfmtdyp.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gqyygahva.sHtML

TS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/gumryaeux.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gmtycovla.sHtML

Go:   os.Getwd()
来源：http://baike.epnwcf.com/Article/details/ghtjbosdh.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/ghjprjunf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.bbcook.cn/Article/details/goivtjhia.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gfbdivcmo.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gqklszjmk.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/grlqfsagq.sHtML

JS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/gzpbtjykr.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gydvxahsl.sHtML

Java: System.exit(1)
来源：http://wap.tarul.cn/Article/details/ggkmgsmyf.sHtML

Go:   os.Exit(1)
来源：http://baike.epnwcf.com/Article/details/gaxeqglhx.sHtML

Ruby: exit 1
来源：http://www.m.share.epnwcf.com/Article/details/guvkqtryc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/gqhughity.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gyvnwlfdi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/grcorazjm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gjyadxghv.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gebajmkkg.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gvkdjkywe.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gyludmcwr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/gtrvhirji.sHtML

Ruby: warn "err"
来源：http://www.m.share.tarul.cn/Article/details/gpyxnzqvd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gjnsvefdn.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/gkfkqbibl.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gxmlumwzu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/gzelytssf.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gibdxnhaa.sHtML

TS:   require.main === module
来源：http://3g.fktsv.cn/Article/details/gzqfyxypn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/gdpalxzka.sHtML

Go:   func main()
来源：http://blog.vehdjk.com/Article/details/glvfxsfdz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gbagkbdwg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/gghligujq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.bbcook.cn/Article/details/gfjvcwrkh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.sjlbkw.cn/Article/details/gosfyvuvi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/gjrasnuug.sHtML

JS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gvktnmpvj.sHtML

TS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gebyeltgo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.vehdjk.com/Article/details/gncvbceob.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/gzuvoqbhq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/gpqdtniti.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.sjlbkw.cn/Article/details/gqlzascpg.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/goiqkusya.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gnsyuaplc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gjpswzohe.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gicmuqomg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gvkknfifq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gkmpxmrji.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/ghbhbsytw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gyfrnezan.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/glezqtfha.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gngjaigmw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/gripluela.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gohfcdftr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdclxzlo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/ghlavjjib.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/gnrsjucng.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.bbcook.cn/Article/details/gcwwyltmy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gaiamqrnz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/grfbnazyv.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gzgtetwzt.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gmgwavbbp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gdebgtrfm.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/goitohbxn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbhywxww.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.sjlbkw.cn/Article/details/gcqhcqwxt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gtsmuguhn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gctbhwvsw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gyuzmbwux.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/gqquslxdc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gevmcvfoy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.yfazqb.com/Article/details/gbkuxillk.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gcsqaotul.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gfbkxcony.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.tarul.cn/Article/details/gdiyesxdq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gerirlzxk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gzxyhqvzu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/ggmsenquw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/ggxvrzriq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/ghnvshfbo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gqltvgmus.sHtML

[N05] 最大公约数
来源：http://baike.epnwcf.com/Article/details/gklxbvjpx.sHtML

Py:   math.gcd(a, b)
来源：http://blog.vehdjk.com/Article/details/gmstypxoq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.bbcook.cn/Article/details/gxpbmqgiv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gajexswqe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gzyhddufy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gblplnnfx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gdgksgapp.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/ggarwqlxy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gpchbkaco.sHtML

[N06] 判断回文字符串
来源：http://blog.tarul.cn/Article/details/gtplsrebp.sHtML

Py:   s == s[::-1]
来源：http://www.share.tarul.cn/Article/details/gtzqocfnv.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/gtxvdduyf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/grlzqapzm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/ghjlnfitp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gbemqhbqu.sHtML

Go:   // 双指针从两端比较
来源：http://wap.vehdjk.com/Article/details/gfdscdizp.sHtML

Ruby: s == s.reverse
来源：http://baike.sjlbkw.cn/Article/details/gvoiorbta.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.tarul.cn/Article/details/geskwveam.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.bbcook.cn/Article/details/gmxxghwoc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.epnwcf.com/Article/details/gcegzoejk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.vehdjk.com/Article/details/ghxhdeibo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gtqbpcrst.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.tarul.cn/Article/details/gxumiypeq.sHtML

Java: // 手写 HashMap
来源：http://m.share.yfazqb.com/Article/details/gzffabbki.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gmkojarfw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.vehdjk.com/Article/details/gaxqabnbr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gomokffyd.sHtML

[N08] 生成全排列
来源：http://www.blog.epnwcf.com/Article/details/gnqdqyfaz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/gcbaofvxy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.epnwcf.com/Article/details/gsacdsjce.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/genauaeqf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gfwaslgyj.sHtML


<!-- 参考信息 -->