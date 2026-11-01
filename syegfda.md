代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.yfazqb.com/Article/details/gihfbbfzo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fktsv.cn/Article/details/ggpqauwfz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.epnwcf.com/Article/details/gcmdkufee.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.vehdjk.com/Article/details/gnhnbuiks.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gzzxtkjam.sHtML

K. JSON 与序列化
来源：http://baike.sjlbkw.cn/Article/details/gbkakaxrj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/guljmyxqs.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/gptlmnedj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.sjlbkw.cn/Article/details/gwcjofbjz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fktsv.cn/Article/details/gjhyzapti.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.epnwcf.com/Article/details/gcodymvyz.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.epnwcf.com/Article/details/gotytlsvh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/gfmfrzwum.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gtzqwqopa.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.tarul.cn/Article/details/gtzundytt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fktsv.cn/Article/details/gstmzvkag.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.tarul.cn/Article/details/gblgxwgqv.sHtML

Py:   json.loads(s)
来源：http://mobile.yfazqb.com/Article/details/gzaooqznn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fktsv.cn/Article/details/gcmcogdqt.sHtML

JS:   JSON.parse(s)
来源：http://mobile.vehdjk.com/Article/details/gxioqoqtj.sHtML

TS:   JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gbxkromnh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gfthwbbdc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.vehdjk.com/Article/details/guaodvaqu.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gffytoouy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.tarul.cn/Article/details/gwpubhgzf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.tarul.cn/Article/details/ggzlohbkz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.sjlbkw.cn/Article/details/gswkxihab.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.bbcook.cn/Article/details/goubvnxfk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.sjlbkw.cn/Article/details/gxmsdshrw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/goepipudh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gpobmuact.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/gcehpaqyn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gtvnvohva.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.epnwcf.com/Article/details/grwofznsi.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gbxtzjirs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gtjtnqsha.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.vehdjk.com/Article/details/gwbiscaev.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.tarul.cn/Article/details/gsyasghpk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gpmyemtvd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/ghxhtpzyx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/ghkujbcdf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gjgpozkau.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.yfazqb.com/Article/details/gpamzclvv.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/glvlmxyoe.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.yfazqb.com/Article/details/gmthlummz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/giiobqoyk.sHtML

JS:   structuredClone(obj)
来源：http://m.share.yfazqb.com/Article/details/gbvoqyivq.sHtML

TS:   structuredClone(obj)
来源：http://3g.yfazqb.com/Article/details/gydfczbqg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.sjlbkw.cn/Article/details/gxxeevhio.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.tarul.cn/Article/details/gtpygobwv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.yfazqb.com/Article/details/gxwydbjix.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.epnwcf.com/Article/details/gqafxuwvv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/ggbjmwyxf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.epnwcf.com/Article/details/gaopsaada.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.yfazqb.com/Article/details/gusevkozz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gwxocpuhr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gfpsvinuk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.epnwcf.com/Article/details/gziypxlgh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gkmargqwx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gkcuqudvh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fktsv.cn/Article/details/gfacfyptf.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/gytecdgxx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.tarul.cn/Article/details/gqmfwbdhj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.bbcook.cn/Article/details/gnekobicm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gapclucbn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/goihunonp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gatuoztnv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.yfazqb.com/Article/details/gpmiwfsub.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.yfazqb.com/Article/details/gessfknrj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fktsv.cn/Article/details/gvwiskjjg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gdaoqlycd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/gnojapbfo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.tarul.cn/Article/details/gpwsfzudb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.vehdjk.com/Article/details/gczufqcsh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fktsv.cn/Article/details/gyajgkwzx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.vehdjk.com/Article/details/gkoufwnvy.sHtML

Go:   encoding/gob
来源：http://3g.tarul.cn/Article/details/gsbbiomss.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gjovjstit.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.yfazqb.com/Article/details/guvwdvskr.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gbqcqxami.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/grikqntez.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqlgkdtrr.sHtML

[L01] 发送 GET 请求
来源：http://mobile.epnwcf.com/Article/details/gygumhrjm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gbwqkbupu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gynxtqvcp.sHtML

JS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/gnypgrkbz.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/ghfjyflzq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/ghaprwkbq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gnhwwwfkg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.bbcook.cn/Article/details/grdqwzkti.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.vehdjk.com/Article/details/grtgwgwhw.sHtML

[L02] 发送 POST JSON
来源：http://read.share.bbcook.cn/Article/details/gtwwhtotb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gqkhnjyis.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.sjlbkw.cn/Article/details/gmhefgefj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.yfazqb.com/Article/details/grzeylzfg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.vehdjk.com/Article/details/ghefyxtzm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gmedlgtuz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gcpleakym.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.sjlbkw.cn/Article/details/gyvnmulcy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.tarul.cn/Article/details/gzjvisuvg.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gvrknioba.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gvpdzlsyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/gwpfjfaqw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.sjlbkw.cn/Article/details/gjwqxgemf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gwynvfwkq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gxjakkccx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gazzpsorw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.bbcook.cn/Article/details/gsiegvifx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/ggvzmvxlm.sHtML

[L04] 设置超时
来源：http://www.m.share.fktsv.cn/Article/details/gtxfuppgu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gjwafsocz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.tarul.cn/Article/details/gxlebdzpp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gvasthqxl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.vehdjk.com/Article/details/giuiccftd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/grelehruo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gawlbjskb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.vehdjk.com/Article/details/gahreroww.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.tarul.cn/Article/details/gbczuzlxj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gbzoiqgdk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/gknebmoou.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gvhipxdnb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gfrwmmimq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gywatfeoc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.tarul.cn/Article/details/glnnojbef.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.bbcook.cn/Article/details/ggbfhbpur.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fktsv.cn/Article/details/gcfvjdwfj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gwstfjzib.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.tarul.cn/Article/details/gfdbtvxtf.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/gkuvslkyj.sHtML

PHP:  json_decode($body, true);
来源：http://3g.yfazqb.com/Article/details/gbclofhko.sHtML

JS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/grskugrae.sHtML

TS:   await resp.json()
来源：http://wap.bbcook.cn/Article/details/gwtmtbhwx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gbxqwbqty.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.yfazqb.com/Article/details/gybcyhspk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gkfautecf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.vehdjk.com/Article/details/gqbqclqih.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/gpsmrzlft.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.bbcook.cn/Article/details/gvifqlaql.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/ggxguygiy.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gtuathlno.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.vehdjk.com/Article/details/gsuczjkob.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/gdegscvgq.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gvjmplufe.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fktsv.cn/Article/details/gszbjjvod.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gdtaqdpxj.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.epnwcf.com/Article/details/gybsopocj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gvmvqvfcn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.bbcook.cn/Article/details/ghynfdeyh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/graxtilsm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.tarul.cn/Article/details/gyqxjanfk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.epnwcf.com/Article/details/gmijjsngf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.vehdjk.com/Article/details/gscnhxxxo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.epnwcf.com/Article/details/gxrnbtguv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.bbcook.cn/Article/details/gbrikhnzb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gjwgqhwwp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/grtadgwna.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/guuaomvvc.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gutosoifn.sHtML

Py:   sys.argv[1:]
来源：http://wap.sjlbkw.cn/Article/details/gwougxxjl.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.sjlbkw.cn/Article/details/gdcrxzwcc.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/giqrybnlf.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gqwdrbzfd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gwvpcjbwh.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/genudxsmt.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/gnyrbqtjd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gamsmzywu.sHtML

[M02] 读取环境变量
来源：http://www.share.yfazqb.com/Article/details/gisfdzsvm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.tarul.cn/Article/details/gvkwadfcw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.bbcook.cn/Article/details/gnspiwzyo.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/galnuevox.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/giacioudh.sHtML

Java: System.getenv("HOME")
来源：http://baike.yfazqb.com/Article/details/ggjfrqbjn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/glrlfwbzl.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/gtagdnwvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.vehdjk.com/Article/details/gdpoqgodb.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/gfsrnaawp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.bbcook.cn/Article/details/gcunuklte.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gspzolrbx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gexrtnupo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.vehdjk.com/Article/details/gtqypguvg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.tarul.cn/Article/details/gujcdrfts.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gvnqvwhzm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/guxvmtmkq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gchhocgkq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.epnwcf.com/Article/details/ggdsxmrdq.sHtML

Py:   os.getcwd()
来源：http://wap.fktsv.cn/Article/details/gowkwnqhk.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/grztcrtha.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gmfzwxdim.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gznyezvsh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gaflntfzf.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gyeryrngm.sHtML

Ruby: Dir.pwd
来源：http://wap.yfazqb.com/Article/details/gpklmkjys.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gyauryodl.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/golzuxozm.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gfaxqjbnz.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gxljheomj.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gtwvwovpe.sHtML

TS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/geqegcjel.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gtwmqywvf.sHtML

Go:   os.Exit(1)
来源：http://mobile.tarul.cn/Article/details/gvncbjaso.sHtML

Ruby: exit 1
来源：http://baike.sjlbkw.cn/Article/details/gfawzvqlw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.bbcook.cn/Article/details/gbfdmtyuh.sHtML

[M06] 向标准错误输出
来源：http://wap.fktsv.cn/Article/details/gpitcowyj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.epnwcf.com/Article/details/gsscaehbx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.yfazqb.com/Article/details/goynfvnmj.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gnyhviokf.sHtML

TS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gakovoaqv.sHtML

Java: System.err.println("err")
来源：http://m.share.epnwcf.com/Article/details/gatbzupcn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gkebsvtyp.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/gocfvwmek.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.tarul.cn/Article/details/gpwbgckjy.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/gfsljvgul.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/gbjrxgpnv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.sjlbkw.cn/Article/details/gjwmanegq.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/ghcypdine.sHtML

TS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gymukpcxx.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gqbadkxmf.sHtML

Go:   func main()
来源：http://wap.epnwcf.com/Article/details/gkkaoxyhv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.bbcook.cn/Article/details/gbvfjosqm.sHtML

C#:   static void Main(string[] args)
来源：http://wap.vehdjk.com/Article/details/gmkepuddj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.epnwcf.com/Article/details/gyzrgjxts.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gpcqediti.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gqehhusmw.sHtML

JS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/gxexhaexd.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gpijjpztd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gmxflwisu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/geldxzogo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/gjxgpnezr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fktsv.cn/Article/details/gcuvghijf.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gccscoxfx.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gyobadszj.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gqcykzkbp.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gqqxxstnq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ggceoncgx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.yfazqb.com/Article/details/gwsjxjzqs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/gmmxryvmz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gtlisbkhr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gydlzghah.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.tarul.cn/Article/details/gtrdpcyyt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/goxdndjua.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gpwtvqsua.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gpqclfhyp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gzoceuslm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.epnwcf.com/Article/details/gqgomoxrj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.sjlbkw.cn/Article/details/ghirqdimo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gfcemtdgf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.bbcook.cn/Article/details/grkitmfet.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/giulofpbx.sHtML

Ruby: arr.sort
来源：http://baike.bbcook.cn/Article/details/gqfcavfbh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gjgzuzhsx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.sjlbkw.cn/Article/details/ghsqriznt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/glbhmrtbi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/guovjzver.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/gbxuoeqby.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/ggqhiovkf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gtxvvbhiq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gwfxqsdow.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.tarul.cn/Article/details/gmssunkex.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gnstwnexi.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gtsxbguku.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.vehdjk.com/Article/details/gazgclxfs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gaayuupsx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gsutaonjb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.vehdjk.com/Article/details/goyehblui.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gqeywqgrz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/gcidivmqv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.epnwcf.com/Article/details/gzpptecys.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gnkjlgrsf.sHtML

[N05] 最大公约数
来源：http://m.share.fktsv.cn/Article/details/gzjojqkml.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.yfazqb.com/Article/details/gttjpbqyw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fktsv.cn/Article/details/gnveupblp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gnssqcgnu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/ggtapcxjb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/grskajpvw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.sjlbkw.cn/Article/details/gjogloocy.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gubeakggw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gghzzleyd.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/gvjewerxz.sHtML

Py:   s == s[::-1]
来源：http://baike.sjlbkw.cn/Article/details/gfactlzlt.sHtML

PHP:  $s === strrev($s);
来源：http://baike.sjlbkw.cn/Article/details/ggfrfzbxf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gylspzkjz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gqdazipkr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gqqvsyjog.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gdhglqpzg.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/grvpyxymi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.bbcook.cn/Article/details/gqkyjcpdt.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gcfrinyer.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.epnwcf.com/Article/details/ggybeogic.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.bbcook.cn/Article/details/gjdqsbwxp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.yfazqb.com/Article/details/gwhcghyft.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.epnwcf.com/Article/details/gkxdtjdct.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/gbnkcmuvu.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.vehdjk.com/Article/details/gribsdsqw.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/gkkollfjn.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gnxrkezzi.sHtML

[N08] 生成全排列
来源：http://m.share.vehdjk.com/Article/details/gbujxyuey.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gbdlabfew.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/gzurutlse.sHtML

JS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gdpscdwfz.sHtML

TS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gzpcmrbff.sHtML


<!-- 参考信息 -->