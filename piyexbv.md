代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.epnwcf.com/Article/details/gdfjsdbfh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.tarul.cn/Article/details/gfpscsrbu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.epnwcf.com/Article/details/gtcmzohhk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.bbcook.cn/Article/details/gumryvtkh.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqocpkfpq.sHtML

K. JSON 与序列化
来源：http://www.share.yfazqb.com/Article/details/ggftkcqkw.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/ggowavzax.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.epnwcf.com/Article/details/glvxfblja.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.vehdjk.com/Article/details/gcjvrmnkb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.bbcook.cn/Article/details/gkunpullh.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/gafsciylv.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.yfazqb.com/Article/details/ggvchektl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.yfazqb.com/Article/details/gabivqhux.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gjvtpfmuo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.vehdjk.com/Article/details/gpksfjzwa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/gwcpekeqn.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.epnwcf.com/Article/details/gnxqtysgc.sHtML

Py:   json.loads(s)
来源：http://baike.sjlbkw.cn/Article/details/ggmbvvnwy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/gifxeipfl.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.yfazqb.com/Article/details/gcuioftdm.sHtML

TS:   JSON.parse(s)
来源：http://m.share.yfazqb.com/Article/details/ggfaqdzfb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/gjgkwozaf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.sjlbkw.cn/Article/details/gbclosrzm.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/grqmjihvc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/gjsthpitp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.vehdjk.com/Article/details/gpvddgqxi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gheqsqtid.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.tarul.cn/Article/details/ggivevyke.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/gyfaflcqb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/ghjogkqym.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.epnwcf.com/Article/details/gdqllgmvk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.sjlbkw.cn/Article/details/gzdsqsfjr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.epnwcf.com/Article/details/gmrhgblcz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.yfazqb.com/Article/details/gxlhcsyxe.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gasfjzcdn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.vehdjk.com/Article/details/gzoshtdkb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gsehaeram.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.vehdjk.com/Article/details/guenvisvr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gkustbarb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gijiztsfd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/genjuizyh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gbhnijbxk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.vehdjk.com/Article/details/gzmyancac.sHtML

[K05] 深拷贝对象
来源：http://3g.sjlbkw.cn/Article/details/gxlhjabha.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.tarul.cn/Article/details/gfhbnofse.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.tarul.cn/Article/details/gwjddqhjq.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gtprrtkyo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/ghutfcfuz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gihqeynpx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fktsv.cn/Article/details/gurddcdwj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.tarul.cn/Article/details/gthghsmvl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.vehdjk.com/Article/details/gfimczxhq.sHtML

[K06] 解析 URL 查询串
来源：http://blog.sjlbkw.cn/Article/details/gtpitohrk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.tarul.cn/Article/details/gchyfbfsq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/gpntkoaqd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.bbcook.cn/Article/details/gaxjhftyc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/grbcngbgt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.sjlbkw.cn/Article/details/gtxziskde.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/giymjnokk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.vehdjk.com/Article/details/gcsnekumn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.yfazqb.com/Article/details/gmcklkkbi.sHtML

[K07] 进制转换
来源：http://baike.vehdjk.com/Article/details/gmflcddvx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gpbwmhyko.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.sjlbkw.cn/Article/details/gelwsxrhz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gnulrmanv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gzeqlkaex.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gyiiwakuf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.sjlbkw.cn/Article/details/gpngqwnfr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.vehdjk.com/Article/details/gkgyxpujr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/ghaboovpn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fktsv.cn/Article/details/gnfyokbhy.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.epnwcf.com/Article/details/gbpmvxomj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.bbcook.cn/Article/details/gfsmknihg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gxkcxtsnp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.epnwcf.com/Article/details/gmekwnbml.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.tarul.cn/Article/details/gjomgjvke.sHtML

Go:   encoding/gob
来源：http://wap.epnwcf.com/Article/details/grmsxydxr.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gusxtfvbk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gyqjsdntw.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gcdxoaexo.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/goxjxyrnk.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxhvqiiol.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/glyqglibg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.yfazqb.com/Article/details/gvcnlkxgr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.epnwcf.com/Article/details/gakyvqhzw.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gafxztxeq.sHtML

TS:   await fetch(url)
来源：http://www.m.share.vehdjk.com/Article/details/gitnvmcyl.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.sjlbkw.cn/Article/details/gbrhalsgx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/ghulrlqvg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gcttwumfa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.epnwcf.com/Article/details/ghubddtlq.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/goddaewsf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.yfazqb.com/Article/details/gqdcwsotz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gxzrrqsll.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.yfazqb.com/Article/details/guhfpuboo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gfvunphiw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/gqnrvyygx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fktsv.cn/Article/details/gpzsmpbzc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.tarul.cn/Article/details/gsfuiyusb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fktsv.cn/Article/details/gwyedgcvr.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gdssulrku.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/grgdpbpaf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.bbcook.cn/Article/details/gggurrlyn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gtyxxwcmj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gsxhiamkx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/ghjlwxzeg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/gebtumeho.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.bbcook.cn/Article/details/gvtlmlfqt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gwqkfrxnu.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gtlzjzcsx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.yfazqb.com/Article/details/gsotlgdob.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.tarul.cn/Article/details/gfpfbdncw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gmoatnkdh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/ggedlcxtx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/gzfzbrhay.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.yfazqb.com/Article/details/gwdiseutm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gifkotaub.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/gxvwkydly.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fktsv.cn/Article/details/gdrgxhutc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/ghyzgiika.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gfqpgddls.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gdgvhrgdw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gvhaubzmz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gngeescuz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gyjbvjmlh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gogkdunrx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.sjlbkw.cn/Article/details/gqtqnvuay.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.tarul.cn/Article/details/gkzipvzbx.sHtML

Py:   resp.json()
来源：http://read.share.yfazqb.com/Article/details/gnlffaweu.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/gsyclrwpx.sHtML

JS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gutvgrede.sHtML

TS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gdyzbnbvl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gfvotamxl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.sjlbkw.cn/Article/details/gqenosvoh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fktsv.cn/Article/details/gesibychs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.sjlbkw.cn/Article/details/gccnhliyt.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.bbcook.cn/Article/details/gaafpwhjq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.tarul.cn/Article/details/gyagtrwqd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fktsv.cn/Article/details/gynegrsqj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gfzmylebv.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/gyvnyctkl.sHtML

Java: resp.statusCode()
来源：http://3g.yfazqb.com/Article/details/gwfxjaebo.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gwzztmgne.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.tarul.cn/Article/details/gaymyvedf.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.tarul.cn/Article/details/gkjronapn.sHtML

[L08] 并发请求多个地址
来源：http://www.share.sjlbkw.cn/Article/details/gdynyslmq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/gempjldpl.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gitdiamcq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gqqbotclg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/gzfmhwthg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gnmlyfiyb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fktsv.cn/Article/details/gudccrlsx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fktsv.cn/Article/details/gaznueusn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/gbkxitklw.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gejgljhiw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gmtdpjlix.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/grtnofdef.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/ghcwigudp.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gqjgftuth.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.bbcook.cn/Article/details/grhojwpkq.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gplevirgv.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gzbgqqgvn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/grabvzkzg.sHtML

Go:   os.Args[1:]
来源：http://blog.fktsv.cn/Article/details/gdjhdtwyc.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gaarlfkhf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gorxxzkfj.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/gslicgbqz.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/galddkobo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gvqnvmefh.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/glzqqqhpy.sHtML

TS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gskxdgtpi.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/gzschirhc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/gfepbdzlg.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gjrmjrysb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fktsv.cn/Article/details/gqiceognm.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/gfzkhkrds.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.yfazqb.com/Article/details/gyxenidze.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gaqvaridq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gvihwnoqj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/goagnrrzf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gfmqpwrod.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gjyybdlyk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gmvofgcdt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gdxpshuqd.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/gaezfsbeh.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gwtrjwnqx.sHtML

PHP:  getcwd();
来源：http://www.m.share.sjlbkw.cn/Article/details/gnltepzoc.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/ggezbduqw.sHtML

TS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gctmbcznw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/ghkuuturr.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/ggmrzsnhy.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gtsfivzlr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gajrtbzfp.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gximqlxtk.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gxiedlmcc.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/guoxmhoxz.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gsbptimkb.sHtML

TS:   process.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwopkhhye.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gtoeergji.sHtML

Go:   os.Exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gcsvnymma.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gcdqkmcpi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.sjlbkw.cn/Article/details/gihlpirgr.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gkeuiuuea.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.vehdjk.com/Article/details/giloogabb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/gumfgvarh.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gksukfcmp.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gpddfpprm.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gvnqrwqyc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/garbvytbc.sHtML

Ruby: warn "err"
来源：http://blog.sjlbkw.cn/Article/details/glkydsnnu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fktsv.cn/Article/details/gjmitehth.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/ghlvtadkr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gnfpqrydy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gdhpjenql.sHtML

JS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/gdllipqhg.sHtML

TS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/grnmhiqyg.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/giuhirjdi.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/glwarclfz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/ghivxvblu.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gdbsqvags.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.vehdjk.com/Article/details/gagqdcuhm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/gkjchrymf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gbhoizchy.sHtML

JS:   process.platform;  process.version
来源：http://baike.bbcook.cn/Article/details/gsdkcghwx.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gwqtyypyc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/googxgiyj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fktsv.cn/Article/details/gurjeiaus.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.tarul.cn/Article/details/gqvjmstyq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/gwttseenu.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gryyvtyxg.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gbagxnwdt.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gozvxgsra.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/grnlyplqz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/ggofomkch.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gmetzmttf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gvfcmdcbr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gnumsdljd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/ggaqegsfr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gcnmxqymk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/gcmnajvae.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gnnudzqss.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/glzbpqsfb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gmemhomfi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gnonchyih.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gesymqhol.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gakfwddyt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.yfazqb.com/Article/details/ggrjmzxrk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/guxigaefo.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gddfhcodd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fktsv.cn/Article/details/gnosgwdnx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gljwsgxxk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.tarul.cn/Article/details/gpwpksses.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.epnwcf.com/Article/details/geekqvsvv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gpzosnujj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gpfffoatc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.sjlbkw.cn/Article/details/gutojqghq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.sjlbkw.cn/Article/details/gxeiinnhq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.tarul.cn/Article/details/gehhaihbf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gqamenpwb.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/gitcwoozs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gudspqlet.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gxyhaiwbg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gxqwjjviv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gudyxowro.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gwdbfrwec.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gmubhojmq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/griouahys.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/grlkkyqzv.sHtML

[N05] 最大公约数
来源：http://mobile.bbcook.cn/Article/details/gomliexwc.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gbqcfkzad.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/gtskbahxx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gwewvvgds.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gsemfyihr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gebsxgpec.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fktsv.cn/Article/details/gdjbklhxa.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gpwbifahj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.yfazqb.com/Article/details/grqcacwod.sHtML

[N06] 判断回文字符串
来源：http://3g.vehdjk.com/Article/details/gydqpihgw.sHtML

Py:   s == s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gjnwgeamr.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gpcbonsdl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/gntrbvdec.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.yfazqb.com/Article/details/ggvpiyovb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.bbcook.cn/Article/details/giywvndex.sHtML

Go:   // 双指针从两端比较
来源：http://wap.sjlbkw.cn/Article/details/gptgsquvw.sHtML

Ruby: s == s.reverse
来源：http://blog.yfazqb.com/Article/details/grxczvttm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gjhbpvvqx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fktsv.cn/Article/details/gaowuiral.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fktsv.cn/Article/details/govlkustb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.vehdjk.com/Article/details/gcykobzxu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.bbcook.cn/Article/details/gxmcnehgt.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gcudhlawa.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gonhwhzmj.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.vehdjk.com/Article/details/ggqekbiqh.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/gtxiecrrw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/gkaxdwrsn.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gmqhgfmzs.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gpzipttis.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gfgmjnlle.sHtML

JS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gbwawolgv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gpqkifepe.sHtML


<!-- 参考信息 -->