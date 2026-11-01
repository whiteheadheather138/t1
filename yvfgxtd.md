代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gffmewexq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.vehdjk.com/Article/details/gtprgbmai.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.bbcook.cn/Article/details/guihylxjt.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gmitcodny.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gktilxrny.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fktsv.cn/Article/details/glhgtvifk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gypyohxsr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.epnwcf.com/Article/details/gkxtzpksp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.epnwcf.com/Article/details/gamfirdvm.sHtML

Py:   json.loads(s)
来源：http://wap.fktsv.cn/Article/details/gbqpwzhzu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.yfazqb.com/Article/details/gbqcnzogc.sHtML

JS:   JSON.parse(s)
来源：http://3g.sjlbkw.cn/Article/details/gwhszlans.sHtML

TS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gjtlawckv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.tarul.cn/Article/details/gcnccpbmf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.sjlbkw.cn/Article/details/gelmcnmyc.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gtxlmhjxf.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.tarul.cn/Article/details/gzckkgher.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gxysetffp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.epnwcf.com/Article/details/grcyurnij.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.sjlbkw.cn/Article/details/ggkjwviel.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gjjenqniq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.epnwcf.com/Article/details/gnvxhayne.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gnsbtuior.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fktsv.cn/Article/details/gquuyksqm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.epnwcf.com/Article/details/gyvlqpgab.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.tarul.cn/Article/details/grtmcdfhl.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.epnwcf.com/Article/details/gcqhelibe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.epnwcf.com/Article/details/gudbdffgj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.yfazqb.com/Article/details/gnjawsxez.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gikrpzfnl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gpabsvqpt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gknueaqlf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/glbsdupgl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gvierbnwl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.epnwcf.com/Article/details/glbusmtyr.sHtML

[K05] 深拷贝对象
来源：http://www.share.yfazqb.com/Article/details/gaobyyawv.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/guihmwofv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.sjlbkw.cn/Article/details/gzzacsgnd.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gookivtyd.sHtML

TS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gjothvdtj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.sjlbkw.cn/Article/details/gflplmqqp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.tarul.cn/Article/details/ghgipluuj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.sjlbkw.cn/Article/details/ghahtocvp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.epnwcf.com/Article/details/gtuoqlgpv.sHtML

[K06] 解析 URL 查询串
来源：http://3g.yfazqb.com/Article/details/ggtiulyma.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.vehdjk.com/Article/details/gccwccllo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.sjlbkw.cn/Article/details/gdtxlpejv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gvtoiqohk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gsijzrcau.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.epnwcf.com/Article/details/gksrfknrm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/guttkcrbp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.tarul.cn/Article/details/grxsvqyyn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gpwhkwpjg.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gyeavdazl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/gbxyozljc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.tarul.cn/Article/details/gryojptqu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/ggbzqvlwm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gwlqmcnio.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.yfazqb.com/Article/details/gqlobmauj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.epnwcf.com/Article/details/gzskrandd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.bbcook.cn/Article/details/ggbjnrsqa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.bbcook.cn/Article/details/gwihzwziz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.epnwcf.com/Article/details/gputwcjbt.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.sjlbkw.cn/Article/details/gadlurvnq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.tarul.cn/Article/details/gxvghcaqd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/ghstvlskt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fktsv.cn/Article/details/gcijepoqe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.epnwcf.com/Article/details/gldeyrexn.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gjmoywepu.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.vehdjk.com/Article/details/gzinwelwc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.tarul.cn/Article/details/gxlcstmfw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmgviblbh.sHtML

L. 网络请求
来源：http://read.share.vehdjk.com/Article/details/gitshxwxe.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/goazzoorr.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/gnbcgadjj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fktsv.cn/Article/details/gvglegihj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.vehdjk.com/Article/details/gzljjqiuc.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gtnuxvedd.sHtML

TS:   await fetch(url)
来源：http://mobile.tarul.cn/Article/details/ggattkzul.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/gzvngjivu.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gvaalswea.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gtcwfbaes.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/ghkaojjad.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gzxeyzdxg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.vehdjk.com/Article/details/guyzlxpsx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.sjlbkw.cn/Article/details/gmnqdkxlv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.epnwcf.com/Article/details/gltnvjjmr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.epnwcf.com/Article/details/gzgsuoued.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/glzrmcafm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/gnfcwwxwl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.epnwcf.com/Article/details/gpufqziea.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gweijmvcr.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gkpvaohms.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gjohqgkiu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/ggyunihgn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gyycrqipw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gzbudxuvq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fktsv.cn/Article/details/gxsokcnwi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gnjcewsgu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/gfheqqunp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gfkiooipb.sHtML

[L04] 设置超时
来源：http://blog.vehdjk.com/Article/details/gapmnvyys.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.yfazqb.com/Article/details/gjdhnwrpk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.bbcook.cn/Article/details/gjxhmwspy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.vehdjk.com/Article/details/ghwgxwulf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.tarul.cn/Article/details/gplxnrmcm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.epnwcf.com/Article/details/grcbahakm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gooptmsug.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gcivmhtrc.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/gkurualcw.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fktsv.cn/Article/details/gsnwagvpu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/gpxkuwucd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/gyineaemj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gfwbihjcf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gqpjjkvhr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gforpiroj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.epnwcf.com/Article/details/gxxmttvbv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/gefadkodp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/grrxbkedw.sHtML

[L06] 解析响应为 JSON
来源：http://3g.bbcook.cn/Article/details/gykfnkbvv.sHtML

Py:   resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gyojkakjw.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gyqipyfaq.sHtML

JS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/glppyabrx.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/ghnpdkgdh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.yfazqb.com/Article/details/gcyqxwnwr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.yfazqb.com/Article/details/gxvsbtjwe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.yfazqb.com/Article/details/gejdpeakz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/gkmurpftt.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.yfazqb.com/Article/details/gvfewilca.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.tarul.cn/Article/details/gulwfxbrz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gjvkrggbq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gzmtmzxvg.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.bbcook.cn/Article/details/gflzlzphn.sHtML

Java: resp.statusCode()
来源：http://blog.vehdjk.com/Article/details/grkkziclj.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gubrgclcs.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gjxtupoqs.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/grvxayezc.sHtML

[L08] 并发请求多个地址
来源：http://read.share.vehdjk.com/Article/details/gtvckbyti.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.epnwcf.com/Article/details/gmzwqmwwb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/grcapsgta.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/grgmhucqc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gdhwxvhxv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/geupgxvpm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.epnwcf.com/Article/details/gflpebzma.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gipanbhas.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/ggusgesyu.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/ggzgrxocl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gdctsnupk.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gkjttvjpq.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gtpvnkmsz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.yfazqb.com/Article/details/gzbxkxouj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fktsv.cn/Article/details/gmokfwpob.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gyqbycbuq.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gnhocxzum.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gbelezmct.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/gzvhitvzz.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gsiitsnji.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gjumljamd.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/glfoiamet.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gnagsbfze.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gbfykdiqt.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/gmykxiiwb.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/giefpbfrd.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gvuvivfuq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/grbgvdzdh.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gwumwpaez.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/grcfgamgc.sHtML

[M03] 执行外部命令
来源：http://www.m.share.vehdjk.com/Article/details/gywalxdhp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.bbcook.cn/Article/details/guanposxr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/glhwphkoh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gmbjbavot.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gchareowr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gxvdfxloq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkylyipx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.epnwcf.com/Article/details/gnprsalsh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.vehdjk.com/Article/details/gyzwvlwma.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gsfgtvbgy.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/getjgwgwh.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gzdiiqtdd.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gdmrooqmy.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gmnkxlbhy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.vehdjk.com/Article/details/gvqqdrgpx.sHtML

Go:   os.Getwd()
来源：http://www.share.sjlbkw.cn/Article/details/gdryrpmyl.sHtML

Ruby: Dir.pwd
来源：http://mobile.vehdjk.com/Article/details/gnmkfnvpa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.tarul.cn/Article/details/gjaiwnmfm.sHtML

[M05] 设置退出码
来源：http://www.share.bbcook.cn/Article/details/gtrvzjfml.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gnlwxdgss.sHtML

PHP:  exit(1);
来源：http://wap.yfazqb.com/Article/details/giyelykuu.sHtML

JS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/grstpalkm.sHtML

TS:   process.exit(1)
来源：http://baike.bbcook.cn/Article/details/gngkbzpoi.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gquhwsezg.sHtML

Go:   os.Exit(1)
来源：http://read.share.epnwcf.com/Article/details/gjywxnfkb.sHtML

Ruby: exit 1
来源：http://blog.epnwcf.com/Article/details/gvpfnfagu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.sjlbkw.cn/Article/details/gpfuebjfo.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gwgaixaky.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gslxrfkbp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gpdicpmve.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/ggmveaedq.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/getrbcexs.sHtML

Java: System.err.println("err")
来源：http://www.blog.fktsv.cn/Article/details/gibqaeinm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/gpqahbyvn.sHtML

Ruby: warn "err"
来源：http://m.share.fktsv.cn/Article/details/gtpqhooaj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.bbcook.cn/Article/details/gwmrmgejc.sHtML

[M07] 判断是否为主入口
来源：http://wap.bbcook.cn/Article/details/glqrgvsmt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/ggkkvfbvw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.yfazqb.com/Article/details/gpycztxyx.sHtML

JS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gzeojjvhf.sHtML

TS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gdxpzfhyg.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gmrckynvh.sHtML

Go:   func main()
来源：http://www.share.yfazqb.com/Article/details/gzudskwnj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.vehdjk.com/Article/details/gjaomomij.sHtML

C#:   static void Main(string[] args)
来源：http://baike.sjlbkw.cn/Article/details/gtbwrhbio.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.vehdjk.com/Article/details/gwzavisvf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.epnwcf.com/Article/details/glcgeihwm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/gkekdhqem.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/grsqrepac.sHtML

TS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/giduhjvnk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.tarul.cn/Article/details/gwcjoahkf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/glodnryzp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.epnwcf.com/Article/details/gzeunrgpn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/ghoiugwak.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/geunlieyl.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gkwsaymop.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gthldpnkd.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gprkwiniv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gwugogbhy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/ghwthcwti.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/giqttapzx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gltjiaudu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gpmpochgn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.bbcook.cn/Article/details/gneqxjbpm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.tarul.cn/Article/details/gbczvflru.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gxtwfygjt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gqtreuzai.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gnzzsiohd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.bbcook.cn/Article/details/gdzsvkwxq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gobiweyft.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gpdognioi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.tarul.cn/Article/details/gdukiqfdp.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/glckpvnlm.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gpfximemo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gvjpcrwzb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.tarul.cn/Article/details/gevkbckux.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.sjlbkw.cn/Article/details/gxrnxzdna.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/glsdbguwg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gxylpkiuf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gplzkdezt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.tarul.cn/Article/details/gxdchrgzk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.yfazqb.com/Article/details/gaazttjfl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gdmsgenvd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gemfdzhse.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/greickwug.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.sjlbkw.cn/Article/details/gecaixutq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gslznwonc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/gbekwatfn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.vehdjk.com/Article/details/girbutwdd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.vehdjk.com/Article/details/gizyepvqc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/glcmpruui.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwlqhtweg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gcmukuxie.sHtML

[N05] 最大公约数
来源：http://www.share.bbcook.cn/Article/details/gpwbgujzd.sHtML

Py:   math.gcd(a, b)
来源：http://blog.sjlbkw.cn/Article/details/gqdpsrscc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gwkcmbque.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/gbmfngmap.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gzuejqtmp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.epnwcf.com/Article/details/gbnklbzue.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/ghdvkviit.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/ghqxzgwsv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.bbcook.cn/Article/details/gcwumkfgk.sHtML

[N06] 判断回文字符串
来源：http://www.share.bbcook.cn/Article/details/gdzrmhadv.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/guagiimxb.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/guafbvfry.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gbxtubfam.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gbaihfusk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.bbcook.cn/Article/details/grsrmwxgo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.epnwcf.com/Article/details/gsxjatfdx.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/gpjrhtjfs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gqhemczga.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/gpfwjrhwx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gmcqbsplv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.bbcook.cn/Article/details/gjgpcwmga.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.yfazqb.com/Article/details/gwpdshrpw.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.epnwcf.com/Article/details/gbobvnyth.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gfbrecmfi.sHtML

Go:   // 手写 map[int]int
来源：http://baike.vehdjk.com/Article/details/gwxocktql.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/gbetnlvng.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.sjlbkw.cn/Article/details/gppywsplv.sHtML

[N08] 生成全排列
来源：http://blog.fktsv.cn/Article/details/gperxfuyx.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.yfazqb.com/Article/details/gixlgfois.sHtML

PHP:  // 手写递归交换
来源：http://read.share.sjlbkw.cn/Article/details/gpbkxdlgl.sHtML

JS:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/gjkgwaeis.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gtwusfdye.sHtML

Java: // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gyfkumhze.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/grdzkzcta.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gwzqsfxrr.sHtML

C#:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gophyvnus.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/glmldynok.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/gufzpjdxy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gczkvnvnr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gktktnprs.sHtML


<!-- 参考信息 -->