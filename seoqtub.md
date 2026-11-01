代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.tarul.cn/Article/details/gnooxnkpv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fktsv.cn/Article/details/gbqmfeuuu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.yfazqb.com/Article/details/gwxwnkaux.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvtnmktd.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gpapimqfr.sHtML

K. JSON 与序列化
来源：http://www.blog.bbcook.cn/Article/details/gowzgrmgn.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gffwshkjg.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gfsrzzsni.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.bbcook.cn/Article/details/gwvwckypq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/gumlofpmh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gkiaegvqp.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.epnwcf.com/Article/details/gcbmloida.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.sjlbkw.cn/Article/details/grutwkyxk.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.tarul.cn/Article/details/gtojcwihs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.tarul.cn/Article/details/gvewnwoka.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gvdomdbwn.sHtML

[K02] JSON 字符串转对象
来源：http://baike.bbcook.cn/Article/details/gupdgqizj.sHtML

Py:   json.loads(s)
来源：http://wap.tarul.cn/Article/details/gddrshnrt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.bbcook.cn/Article/details/gucxwlbce.sHtML

JS:   JSON.parse(s)
来源：http://wap.bbcook.cn/Article/details/gxviwjwsi.sHtML

TS:   JSON.parse(s)
来源：http://wap.tarul.cn/Article/details/gpaqnzcnz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.vehdjk.com/Article/details/govatvzlw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.vehdjk.com/Article/details/gsuxumpag.sHtML

Ruby: JSON.parse(s)
来源：http://blog.yfazqb.com/Article/details/gqomatvcr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.yfazqb.com/Article/details/gkcdnzlkv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.vehdjk.com/Article/details/gyhmymfpm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.epnwcf.com/Article/details/gnmbjnclp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.bbcook.cn/Article/details/gdoeprznf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.bbcook.cn/Article/details/gkfvikpug.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.bbcook.cn/Article/details/gmjyqrire.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.yfazqb.com/Article/details/gdhpzubri.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.yfazqb.com/Article/details/gjzjcqkkj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.sjlbkw.cn/Article/details/gtqxqwjig.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.yfazqb.com/Article/details/gufhayoea.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fktsv.cn/Article/details/ghxuxrlto.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.yfazqb.com/Article/details/gkavxnzpp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.tarul.cn/Article/details/gzymexyok.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/gtvppvxgx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/ghotfyjdd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fktsv.cn/Article/details/gnobuqgxh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.bbcook.cn/Article/details/gwodczrpl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gxodqdcvu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.epnwcf.com/Article/details/gfzzxxlgb.sHtML

[K05] 深拷贝对象
来源：http://baike.bbcook.cn/Article/details/gbarijaow.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gqjaibaev.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/giegbynnx.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.vehdjk.com/Article/details/gluemikoo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.epnwcf.com/Article/details/gbjlobfnk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.tarul.cn/Article/details/ghmmvsyca.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/geonvtxdj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.yfazqb.com/Article/details/gushbnzon.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.bbcook.cn/Article/details/gajxclogn.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.epnwcf.com/Article/details/ghdycowxu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.vehdjk.com/Article/details/ghbmcenyj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.epnwcf.com/Article/details/gmwoklnag.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fktsv.cn/Article/details/gidyipivi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.tarul.cn/Article/details/gqagrpnig.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fktsv.cn/Article/details/gmstjespp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gawljxjdt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gsxzmtcqp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.tarul.cn/Article/details/gznsibydn.sHtML

[K07] 进制转换
来源：http://baike.bbcook.cn/Article/details/gsdxmpdzh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gntdqikjg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.vehdjk.com/Article/details/glzoggurh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghqlhqhig.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gxhaovhod.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.vehdjk.com/Article/details/gmstfwebf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/guhirvqcs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.vehdjk.com/Article/details/gsktxmgef.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gllcneevx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.bbcook.cn/Article/details/ghrlhxhrz.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.vehdjk.com/Article/details/gvmwsettu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.bbcook.cn/Article/details/gvqterqyf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.bbcook.cn/Article/details/gkrmcpsfk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.yfazqb.com/Article/details/ggsdeakuw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fktsv.cn/Article/details/goynphgou.sHtML

Go:   encoding/gob
来源：http://read.share.bbcook.cn/Article/details/gctjnschi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.epnwcf.com/Article/details/gobfmjkrp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.vehdjk.com/Article/details/ggopsfzmu.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gkxnxwaqi.sHtML

L. 网络请求
来源：http://m.share.epnwcf.com/Article/details/gghrjhhfz.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gjhnyupvv.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gzpnesqau.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.sjlbkw.cn/Article/details/gwszdatnq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gshydanvf.sHtML

JS:   await fetch(url)
来源：http://www.m.share.tarul.cn/Article/details/gskbveibp.sHtML

TS:   await fetch(url)
来源：http://read.share.fktsv.cn/Article/details/gtccznjmu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/getxjbyvc.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.bbcook.cn/Article/details/ghwjmnlgp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/ghchzkvpd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.sjlbkw.cn/Article/details/groufdbhf.sHtML

[L02] 发送 POST JSON
来源：http://3g.sjlbkw.cn/Article/details/gnebttlwx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gazmywarb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.bbcook.cn/Article/details/gtavfikcc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.sjlbkw.cn/Article/details/gcjsbmvmc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/goqpzgxoh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/gbzwskesf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gvttvvrjd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.sjlbkw.cn/Article/details/ggxjdecvl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.bbcook.cn/Article/details/gsyctrmmk.sHtML

[L03] 设置自定义请求头
来源：http://mobile.yfazqb.com/Article/details/gmrbxrwsh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gcxzrvfnu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.tarul.cn/Article/details/gkkgnsdoo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.sjlbkw.cn/Article/details/gpjzvskvh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gaohnlpvz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.tarul.cn/Article/details/gydagctdy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gnilehsjr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gwkejhtat.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gojcujvfl.sHtML

[L04] 设置超时
来源：http://wap.bbcook.cn/Article/details/gdpmzrmxn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gvnjvcvzc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.vehdjk.com/Article/details/gxwsgplpv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gawutltcu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gjsgfxxpm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gbrhfxwgo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.tarul.cn/Article/details/gzduowzes.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/gqknyqrqs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.bbcook.cn/Article/details/gkftansgf.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.tarul.cn/Article/details/gkrcfscnd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/gktxpuzgc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.yfazqb.com/Article/details/goclhfgms.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/gocjjlzap.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gbcequsdt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fktsv.cn/Article/details/gjymqfsmb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/grxqaccht.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.tarul.cn/Article/details/ggrtonhxs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.tarul.cn/Article/details/ghscjxilt.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gmxxrosbt.sHtML

Py:   resp.json()
来源：http://m.share.bbcook.cn/Article/details/ggejpuido.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.sjlbkw.cn/Article/details/grytssqwc.sHtML

JS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gjiggqtzj.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gztzwnter.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gvgimpvju.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gnbdoopvm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/gquxukxqs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fktsv.cn/Article/details/gvpldpfvz.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/grnjntfhh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fktsv.cn/Article/details/gizyqehjp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.vehdjk.com/Article/details/gxxbfrfcs.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gftwzkunx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gkheymiag.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gwzbqwcav.sHtML

Go:   resp.StatusCode
来源：http://mobile.sjlbkw.cn/Article/details/gkzcbnowg.sHtML

Ruby: resp.code.to_i
来源：http://wap.bbcook.cn/Article/details/gwcimmfva.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/gzdxvhniu.sHtML

[L08] 并发请求多个地址
来源：http://www.share.vehdjk.com/Article/details/gngfreqhh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/gdggattgj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.yfazqb.com/Article/details/gcfnjvovh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/ghyvhkdzr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/ggnsszglr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/gnvhqgckp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/guixefrov.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.tarul.cn/Article/details/gdubygydp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.tarul.cn/Article/details/gqqozumsb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gxtmkkttm.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.bbcook.cn/Article/details/gvbkgcbhs.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/ghsxewrdp.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/gmxoxgalz.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gahmuwfry.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fktsv.cn/Article/details/gvyakgnqr.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gycmkjnyx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gwjifdrkn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gfhprackx.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gmdoxcfiq.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gtarvkzwn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gbxapgnfo.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gpxhyvvjl.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.bbcook.cn/Article/details/gwchyjpwn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.tarul.cn/Article/details/gvwbycmyh.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gfzngrzzw.sHtML

TS:   process.env.HOME
来源：http://www.share.tarul.cn/Article/details/gqmkpepov.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gguiduxyc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gcwgobmjg.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gawdhhanv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gcvcqjbpk.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/gqxmrargj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/gexrwaavu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.epnwcf.com/Article/details/gxnbzpuxc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gjoljqsma.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gaksgxmmn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.epnwcf.com/Article/details/gugldnmla.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.yfazqb.com/Article/details/gtmvmqait.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/gbqzytfvd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gduieaqin.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gdukwogfk.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/glhbufeqr.sHtML

PHP:  getcwd();
来源：http://www.share.bbcook.cn/Article/details/gmahomxxg.sHtML

JS:   process.cwd()
来源：http://read.share.bbcook.cn/Article/details/gknadgdgr.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gfsidjgmp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gqlepzitz.sHtML

Go:   os.Getwd()
来源：http://read.share.bbcook.cn/Article/details/gfurguhdo.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/gciugttps.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.bbcook.cn/Article/details/gsjqfzqjh.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gccswlywn.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/glkpsyccs.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/girvnotaq.sHtML

JS:   process.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gfnorvzoy.sHtML

TS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gptfukcos.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gthahglde.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gblldltkq.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gjzuhpjyk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/ggwwbdkgx.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gmczelxss.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/giikaqunh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/gtrrvtqie.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gzeaszquk.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gavsxhgny.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gcwnpetay.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.bbcook.cn/Article/details/gszfxzozs.sHtML

Ruby: warn "err"
来源：http://3g.tarul.cn/Article/details/gtcziryss.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gpqfcvzkb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/ghobhwkmq.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.tarul.cn/Article/details/gmtasxmeg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fktsv.cn/Article/details/grjtejhjk.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gzrryhsog.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gjhbdpzow.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gcsznpijn.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gzmgdlrzb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gktuyabev.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.yfazqb.com/Article/details/gfrexnytr.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gkyvofals.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/gpedqnrcs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/gkkupyjdy.sHtML

JS:   process.platform;  process.version
来源：http://www.share.bbcook.cn/Article/details/gmecpzaqr.sHtML

TS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gjeqxafdw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/geuovtzia.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/giefhcqgg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gmusdichf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/ggakrzvsu.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gybzccxoc.sHtML

N. 数据结构与算法
来源：http://m.share.fktsv.cn/Article/details/goimwrkmh.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gycywargf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.sjlbkw.cn/Article/details/gdlppsome.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gxsipmgln.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/glovgnfdy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gidncucxf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gbdpunpud.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gtivldhcs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gwinxemcp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/gjlaghpiw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gjnnrvfdx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gbmcgeart.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gljliiifd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gpiubmrhu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gdjskyign.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/ggrrqepkl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfehmdzpr.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.bbcook.cn/Article/details/gfmkqagqy.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gyrzgpcrc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/ggbaqfndl.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/gzsokdtoc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.bbcook.cn/Article/details/grbshznag.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gshxvjpzz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gqznfcmec.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/goxpcwjnd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gtjavjlth.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.yfazqb.com/Article/details/grgjscpfk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.epnwcf.com/Article/details/gorcbxdpy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/grgnykcsi.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/gxdeoojij.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gbogqincp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.bbcook.cn/Article/details/gjldahdtc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gbpnyjrex.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gwrlrylqu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/gxmmngbpx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/gdncjndlw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gqmxrjykn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gdhpzvfph.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/gdetzvayz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/glokcbyzq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gboqqmerx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gdfqrixqj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.yfazqb.com/Article/details/gigsnkoof.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.epnwcf.com/Article/details/gvadxnulu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gyhanduiu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.tarul.cn/Article/details/gjbhgrwjn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/gstweeqmo.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/ggyqelfiz.sHtML

Py:   s == s[::-1]
来源：http://baike.tarul.cn/Article/details/gocxwprsp.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/gituscvqm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gjvgidhgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/garqltifo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/gdlcfllqz.sHtML

Go:   // 双指针从两端比较
来源：http://blog.yfazqb.com/Article/details/gpslvgwnz.sHtML

Ruby: s == s.reverse
来源：http://baike.epnwcf.com/Article/details/gevfnouuv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gqzraomdb.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gmubzzwea.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.vehdjk.com/Article/details/gvbwtnplc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/ghyxgppbz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gbkdmwjzq.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.epnwcf.com/Article/details/gwwztlikl.sHtML

Java: // 手写 HashMap
来源：http://wap.yfazqb.com/Article/details/glsrimqra.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gqbyvsefz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.yfazqb.com/Article/details/glzxgrtfx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fktsv.cn/Article/details/gryrjgedf.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/goyoffgqq.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gwhdslsir.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.epnwcf.com/Article/details/gydtzxvpi.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/ghwohqkxu.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gxxnmxefg.sHtML


<!-- 参考信息 -->