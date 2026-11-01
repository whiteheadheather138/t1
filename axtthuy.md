代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.yfazqb.com/Article/details/ggetacarb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.sjlbkw.cn/Article/details/gqxqfdpdk.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.tarul.cn/Article/details/ggffdejpy.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fktsv.cn/Article/details/gbzpxsury.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.bbcook.cn/Article/details/ghkwnfdkr.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gbwpcnvul.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.vehdjk.com/Article/details/gjbeagsms.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.bbcook.cn/Article/details/gpermclot.sHtML

[K02] JSON 字符串转对象
来源：http://wap.yfazqb.com/Article/details/gjggrfcom.sHtML

Py:   json.loads(s)
来源：http://www.blog.sjlbkw.cn/Article/details/gmcuisjyr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.vehdjk.com/Article/details/gyamifshj.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gdkcldncd.sHtML

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/grtnmhjnt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/gloxnuznr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.tarul.cn/Article/details/gszntywbu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/gukmfldxy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.epnwcf.com/Article/details/grtczsgkm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.tarul.cn/Article/details/gldilmcym.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fktsv.cn/Article/details/giqlxakro.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.sjlbkw.cn/Article/details/gyyololms.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/gosgrhpqf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.bbcook.cn/Article/details/glkfzzmza.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gnsbtpjsz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gwinbkkzi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.vehdjk.com/Article/details/ghlydbqew.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fktsv.cn/Article/details/gzyfpitap.sHtML

[K04] 读取 JSON 文件
来源：http://blog.epnwcf.com/Article/details/gqpcxlsvk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.tarul.cn/Article/details/geyhhwjon.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/gntoyiavz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gfcvhdice.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/glsowwncv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.yfazqb.com/Article/details/goanrvxix.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.epnwcf.com/Article/details/gvyfjsxmh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gjlzngmwa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.sjlbkw.cn/Article/details/gfevhplrr.sHtML

[K05] 深拷贝对象
来源：http://www.blog.vehdjk.com/Article/details/gutntopwn.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.yfazqb.com/Article/details/gozggrfac.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fktsv.cn/Article/details/gzsmshtxc.sHtML

JS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/gjivbxhou.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gjdhqsmvg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.vehdjk.com/Article/details/gfnyddust.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.sjlbkw.cn/Article/details/grjpfjhpu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.epnwcf.com/Article/details/gbwkjzvzx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.bbcook.cn/Article/details/ghxxwfuyz.sHtML

[K06] 解析 URL 查询串
来源：http://baike.bbcook.cn/Article/details/grlduivvh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.bbcook.cn/Article/details/gnhfdjnku.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.bbcook.cn/Article/details/ggmxeyiym.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gvqpzmybw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.sjlbkw.cn/Article/details/gvftkxcpr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/ghalbrcxo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.vehdjk.com/Article/details/gutgufize.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/getiijurp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.epnwcf.com/Article/details/gqjyoeekg.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gmefsgtrc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gjxryygwb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fktsv.cn/Article/details/gtrotfvxl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gggutscnv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/guqbkvzdm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.yfazqb.com/Article/details/gkrhaeptz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.vehdjk.com/Article/details/goxtbdsph.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.sjlbkw.cn/Article/details/gafksmveu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.bbcook.cn/Article/details/gakzkcfql.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.tarul.cn/Article/details/gtsbcfeik.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.bbcook.cn/Article/details/glpxlxepb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.bbcook.cn/Article/details/gedfweyuq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gdvheivez.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gzsygamlh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.bbcook.cn/Article/details/gbuefufzj.sHtML

Go:   encoding/gob
来源：http://mobile.vehdjk.com/Article/details/gojojxsnk.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.vehdjk.com/Article/details/ggtrxcszv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gwcblcjcn.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/glmmztvsw.sHtML

L. 网络请求
来源：http://3g.tarul.cn/Article/details/gbeiwgmky.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ggpjobtqq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/gkwgtigdq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.tarul.cn/Article/details/gzcywkqjn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.epnwcf.com/Article/details/gchxziwuc.sHtML

JS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/grebyawbj.sHtML

TS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/ggzctiyjz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fktsv.cn/Article/details/gglamcyph.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.sjlbkw.cn/Article/details/gsqihcznp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.epnwcf.com/Article/details/ghyjhyaxy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.tarul.cn/Article/details/gxyzgwfbx.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/gqhzxvzjy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gioepfprz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.epnwcf.com/Article/details/gswvqmmxt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.bbcook.cn/Article/details/gldlkikys.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/gjlbkozvx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/grxglspek.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.tarul.cn/Article/details/grokjnkik.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/ghcselyuy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.yfazqb.com/Article/details/gpcwsiohw.sHtML

[L03] 设置自定义请求头
来源：http://wap.vehdjk.com/Article/details/gmwnoycrr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.bbcook.cn/Article/details/ghqpxoejg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.epnwcf.com/Article/details/gufajtanb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gzvudkgth.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gldlqwibn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/grgetsbtf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.epnwcf.com/Article/details/grdzhjtlf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/gfqvdifej.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/ggvkoynto.sHtML

[L04] 设置超时
来源：http://www.share.bbcook.cn/Article/details/gsdntiqmk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fktsv.cn/Article/details/gyhufjard.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.sjlbkw.cn/Article/details/gtypkjbap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gupuftcnb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gvwtgbuqb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fktsv.cn/Article/details/gbmhdzxmh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.vehdjk.com/Article/details/glckihkzm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.bbcook.cn/Article/details/gwoppsawh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gmmsgoirk.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.bbcook.cn/Article/details/ghlexsrit.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/gprpctpib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gsrtikbkf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gwnqxqapg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gmqbykizc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gjmihjiyk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/grfhucdkj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.sjlbkw.cn/Article/details/gizddcbhl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.sjlbkw.cn/Article/details/gzqudigjp.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.epnwcf.com/Article/details/getmvykvg.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/gkisbdrvk.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gwygnmbyw.sHtML

JS:   await resp.json()
来源：http://baike.vehdjk.com/Article/details/gxkrgerrr.sHtML

TS:   await resp.json()
来源：http://3g.fktsv.cn/Article/details/guiuggufo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.epnwcf.com/Article/details/gbctqwaeu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.bbcook.cn/Article/details/gxqepgxth.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gipghjwgd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.epnwcf.com/Article/details/gzxdpnnhl.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/grifhcqqq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.tarul.cn/Article/details/guczrpnuy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.epnwcf.com/Article/details/gunikgstk.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gpvoztjvx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gjzfeakgi.sHtML

Java: resp.statusCode()
来源：http://wap.fktsv.cn/Article/details/giwdhehyv.sHtML

Go:   resp.StatusCode
来源：http://read.share.fktsv.cn/Article/details/gganockgz.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gcxangnhb.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.vehdjk.com/Article/details/ggccqqgzl.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gjrhbrliz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.sjlbkw.cn/Article/details/gcvjfcmwx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gnitjdbgi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gdwiedgir.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/glfjounnm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/grhjxqafd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.tarul.cn/Article/details/gnuunbjps.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.yfazqb.com/Article/details/gdateoprl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/gzarmebsk.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gbckvviqu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.bbcook.cn/Article/details/grnwtelop.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmphuusbl.sHtML

[M01] 读取命令行参数
来源：http://read.share.yfazqb.com/Article/details/gidbuorvt.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/ghjtsdawb.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gtqembjkc.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gpmdowdee.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gosqvffol.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/gcvvesepf.sHtML

Go:   os.Args[1:]
来源：http://www.share.sjlbkw.cn/Article/details/gmdmwshup.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gxzclnmco.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/ghgfkvler.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gznpzvkqh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/gvhfthgvt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gpxicuuio.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gqrfyxfpy.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/grjbhgpya.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gktahbbkq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.epnwcf.com/Article/details/gwngnbheg.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.bbcook.cn/Article/details/gwjbnvbed.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/gsbcifumv.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/gqfjnydjl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gptqrsvdq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.sjlbkw.cn/Article/details/gvgigrvpo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gyfcvrlvf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/goaztohzm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gomnytkpd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gbeeljxeb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gfervdzke.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gjugsatdn.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.sjlbkw.cn/Article/details/gaprochpo.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gmblvlley.sHtML

PHP:  getcwd();
来源：http://baike.epnwcf.com/Article/details/ghqmevmcs.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gqouhansu.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/genhguobb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gcruojvjv.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/grgeajfwg.sHtML

Ruby: Dir.pwd
来源：http://wap.fktsv.cn/Article/details/gwxqbrtyy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.epnwcf.com/Article/details/gohuehlfe.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gjoxkpphh.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gkehybcvv.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gbazwkyqe.sHtML

JS:   process.exit(1)
来源：http://3g.tarul.cn/Article/details/gdnsqhsqu.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gibstobys.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gjqiqasyl.sHtML

Go:   os.Exit(1)
来源：http://mobile.yfazqb.com/Article/details/gvfcqhmzt.sHtML

Ruby: exit 1
来源：http://wap.fktsv.cn/Article/details/gvqjofbvz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/gxhcesdnc.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/gzfvsysqz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.tarul.cn/Article/details/gjnohztqf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.sjlbkw.cn/Article/details/gruggchof.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gicvcdmsf.sHtML

TS:   console.error("err")
来源：http://3g.epnwcf.com/Article/details/gbjvfshsy.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gsqyryzgr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/gjwcnndmz.sHtML

Ruby: warn "err"
来源：http://3g.epnwcf.com/Article/details/gaaahkfho.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.vehdjk.com/Article/details/gomfkjesu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.yfazqb.com/Article/details/gzjstjtcx.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.vehdjk.com/Article/details/grjmvwjhc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/gtwthdsay.sHtML

JS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gpcyybzzu.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gnyxgmmhl.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gsiuybqjs.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/gijsiqimy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gkagywzte.sHtML

C#:   static void Main(string[] args)
来源：http://wap.yfazqb.com/Article/details/gcghfmqnm.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gxacdfqgv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/gaphybzum.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gasymbsmw.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gsbyuwvtp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gfeulfkfe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gvbaflmci.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/gclzzikpx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/glyvjoiar.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/gcqqzfrfq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gglrvzyec.sHtML

N. 数据结构与算法
来源：http://3g.epnwcf.com/Article/details/gfaagrepv.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gjhihzgyk.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.vehdjk.com/Article/details/glqzkwfse.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.yfazqb.com/Article/details/guuncluvd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gyltfehzk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gjdiuwmga.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.tarul.cn/Article/details/gfvgbbeey.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gyxktzfdw.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gvuwuznfj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gfhqoqchb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/grvuhejcx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.tarul.cn/Article/details/gnfoytdcv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.yfazqb.com/Article/details/gwrrawkwn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gwavwppul.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gdasauxla.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gekvvblrp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fktsv.cn/Article/details/ghzfsjwbq.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.yfazqb.com/Article/details/gjqospbpx.sHtML

Ruby: arr.sort
来源：http://mobile.yfazqb.com/Article/details/grbnafsho.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gdiykcynz.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.vehdjk.com/Article/details/gmojmiral.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gpjtsgclv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fktsv.cn/Article/details/gedrajezv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/glolzrxcp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gaumaeugg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gyeyozxfk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/gbzpksxuy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/glgrevkrj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.bbcook.cn/Article/details/grbngxpbn.sHtML

[N04] 斐波那契数列
来源：http://blog.sjlbkw.cn/Article/details/gpdcvwfps.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gmnttttwy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.yfazqb.com/Article/details/gjfofbyny.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gripbcfhs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gpvnyeolz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gqkmxkjbc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/gtlzliahn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/gvbbfobvq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/grmejishg.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gtiuyvhff.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gmqklihhe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gmwxalvga.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gfutudnjo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.tarul.cn/Article/details/gnzslqhyg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/gdgtnmigq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gtlcngqcm.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gktmzlppk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.epnwcf.com/Article/details/giyisrgim.sHtML

[N06] 判断回文字符串
来源：http://www.blog.vehdjk.com/Article/details/grcuvutat.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gbyforqyb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.bbcook.cn/Article/details/gvaoqbswe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gsctukriq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gvtxmwlxn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gimukrpzm.sHtML

Go:   // 双指针从两端比较
来源：http://wap.sjlbkw.cn/Article/details/gkgbqjedy.sHtML

Ruby: s == s.reverse
来源：http://baike.vehdjk.com/Article/details/gavylhzpb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.bbcook.cn/Article/details/gnugohugb.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gsdvbojfz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.yfazqb.com/Article/details/gtkgnweyt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gbxjmdnzn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gfkggvlsh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/gfoldrxer.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/ghnsyuopr.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gesdsmtol.sHtML

Ruby: // 手写 Hash
来源：http://3g.yfazqb.com/Article/details/gapplqpve.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fktsv.cn/Article/details/gfdfshogd.sHtML

[N08] 生成全排列
来源：http://baike.tarul.cn/Article/details/gbeyhjnqx.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gccmwhmyd.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/goshccnwl.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/grqxvxqnq.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gjzuycmhk.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gfyddpuio.sHtML

Go:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gvwifcymp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gzmnrncew.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gtrseswgu.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gdpyfcgor.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gdfvhasqi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gimqepcrm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gslvtwpbn.sHtML


<!-- 参考信息 -->