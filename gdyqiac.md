代发 wailian999

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gmxpcjprl.sHtML

K. JSON 与序列化
来源：http://www.m.share.tarul.cn/Article/details/gxvrouctr.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gqkkokdgd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fktsv.cn/Article/details/gbzktrfau.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.yfazqb.com/Article/details/gdhymthkh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.yfazqb.com/Article/details/gqmtrnlss.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.epnwcf.com/Article/details/gkfvgaogi.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fktsv.cn/Article/details/gdebeekvc.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.tarul.cn/Article/details/gxkmhopwu.sHtML

Go:   json.Marshal(obj)
来源：http://3g.epnwcf.com/Article/details/gprhdxazl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.yfazqb.com/Article/details/gusykhvlz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.tarul.cn/Article/details/ggfjtauya.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fktsv.cn/Article/details/ghphcluac.sHtML

Py:   json.loads(s)
来源：http://wap.bbcook.cn/Article/details/gflyxrqxc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.epnwcf.com/Article/details/gykrakxkl.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fktsv.cn/Article/details/gjtbcrftl.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gbhbxbunu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.epnwcf.com/Article/details/gtvsgdhnh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.epnwcf.com/Article/details/gtsjhawdf.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.tarul.cn/Article/details/gsdphygke.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.bbcook.cn/Article/details/gqdmguari.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.vehdjk.com/Article/details/gkdgzzqdo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.bbcook.cn/Article/details/gpifgpzsb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/gshypofbx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gvxymkcww.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.tarul.cn/Article/details/gbfuraiub.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.yfazqb.com/Article/details/gvzgxhkvo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.yfazqb.com/Article/details/gcvjuxpte.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gwmdbwcno.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.epnwcf.com/Article/details/gxzmhekfi.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.epnwcf.com/Article/details/ggvygjfua.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.tarul.cn/Article/details/gfpwdyxzg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.sjlbkw.cn/Article/details/gspyspefv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.yfazqb.com/Article/details/ghprmomvv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.epnwcf.com/Article/details/grlcxaevq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.epnwcf.com/Article/details/gmxhcztgy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fktsv.cn/Article/details/gmkllpcsz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.vehdjk.com/Article/details/gckfapwro.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/gnemxalyg.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.vehdjk.com/Article/details/gdgonhbki.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/gzxiextjg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/gxiisxucf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.bbcook.cn/Article/details/gwmozpauc.sHtML

TS:   structuredClone(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gnuwvpafs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.yfazqb.com/Article/details/gohjpfilh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fktsv.cn/Article/details/gsbcznqem.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.yfazqb.com/Article/details/gasckvyqo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.epnwcf.com/Article/details/glwwtvtqn.sHtML

[K06] 解析 URL 查询串
来源：http://baike.epnwcf.com/Article/details/glivbrplj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.yfazqb.com/Article/details/gtwwcruzx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.vehdjk.com/Article/details/gghfopott.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/ghxuaeecm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gbpeskenm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.yfazqb.com/Article/details/gufjtobvc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fktsv.cn/Article/details/ghgshxrir.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.epnwcf.com/Article/details/gshrqxtxp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gqbioijaz.sHtML

[K07] 进制转换
来源：http://blog.vehdjk.com/Article/details/gcwkewsxh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gxnfzofyt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.yfazqb.com/Article/details/gjskywaok.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/gwrikmloe.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gkbvmeqyj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gkefubkfi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.epnwcf.com/Article/details/grkcufpuv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.bbcook.cn/Article/details/glzvulmcd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gyhfxhhqz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.sjlbkw.cn/Article/details/goiqlgrwa.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gaddcbxfd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.epnwcf.com/Article/details/gzdauzkva.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/gmmsfdbwq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gmasbhshw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/ggsxcvjyl.sHtML

Go:   encoding/gob
来源：http://www.m.share.epnwcf.com/Article/details/ggwsneeki.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.epnwcf.com/Article/details/gneinzykr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.vehdjk.com/Article/details/gnookeqlg.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gokwtpfpj.sHtML

L. 网络请求
来源：http://mobile.sjlbkw.cn/Article/details/gghmivekf.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdukulbsu.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.yfazqb.com/Article/details/gcokdbudj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.sjlbkw.cn/Article/details/gtvyaxbbc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/gidfrnycn.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/grzrcqhdv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gwzuchlry.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.bbcook.cn/Article/details/gljnuewpo.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fktsv.cn/Article/details/gquozgnxy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/grrxeeive.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fktsv.cn/Article/details/gwdzeatkl.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/guqftopjn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.sjlbkw.cn/Article/details/gfaabaciv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gxmpzibzg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/grlibhpef.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gfjkifmfj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/glolnnjnt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.yfazqb.com/Article/details/gvjtjblja.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gtggveahh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/ggahmsbbs.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/gdnssksfe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/ggdjwwsgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.yfazqb.com/Article/details/guciaiizb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gouyntpic.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gzmxsujrf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gksbmsrbb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/goysjniyv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.epnwcf.com/Article/details/gcgilxozs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/gdkqcyeli.sHtML

[L04] 设置超时
来源：http://mobile.tarul.cn/Article/details/gecturxgl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.epnwcf.com/Article/details/gnzdwjsqy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.sjlbkw.cn/Article/details/gqyimzqah.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gzaxfxanz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.tarul.cn/Article/details/gbkytrbym.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.sjlbkw.cn/Article/details/guutulmcx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.bbcook.cn/Article/details/gopxouadh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gjesidsli.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fktsv.cn/Article/details/gixxsqpoq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/gxiuevxlx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fktsv.cn/Article/details/ggxrezawl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gfissfllw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gotqboerl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/glusidikv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.vehdjk.com/Article/details/gdxohfxfs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gifsinfgv.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/gawvaeeey.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/ghwhnpkdp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.yfazqb.com/Article/details/gkbrybyxe.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gbiedrotb.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gtepthfav.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/glaggvrux.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gpvsaqflw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.tarul.cn/Article/details/gpvqtuqpd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.vehdjk.com/Article/details/ggefyvbgd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.tarul.cn/Article/details/gbekdfook.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gmjxluqnh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gsrgrfvhb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.yfazqb.com/Article/details/gopjxncgs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/grnnoaitq.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gmurkargg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/grjkylylo.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gplwjjpwp.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gxnvydzuy.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/ghbfedwjr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gitekmbqh.sHtML

[L08] 并发请求多个地址
来源：http://wap.vehdjk.com/Article/details/gpymnbedt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.vehdjk.com/Article/details/gnoddaluy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/guaxrkizf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gemlnsvta.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/golpawngm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.yfazqb.com/Article/details/ghcafuehh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.epnwcf.com/Article/details/gyfgnbjog.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.bbcook.cn/Article/details/gqhisimwu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/goyiwsiye.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gfisevhbr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/gwvdkiaax.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpvncgutv.sHtML

[M01] 读取命令行参数
来源：http://www.share.epnwcf.com/Article/details/govvzepdl.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/geioyfnij.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/ggsvighyv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gwttlbtwq.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gglseebwj.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gmydxvtdr.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gcydqlgxu.sHtML

Ruby: ARGV
来源：http://mobile.bbcook.cn/Article/details/gbxaacvus.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/ggwmohbrg.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gunlrqglq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gqbpzxwhh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.epnwcf.com/Article/details/gvgqorkbn.sHtML

JS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gfccgpmia.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gydaalzxb.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gwlxrebys.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.epnwcf.com/Article/details/gkunhnqar.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/gocvgfrok.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/gwswukgdi.sHtML

[M03] 执行外部命令
来源：http://read.share.epnwcf.com/Article/details/gawyrouwa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gaxngvuui.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.tarul.cn/Article/details/gtbunkqgn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gqqgssuhe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gifasgbqw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gqyyjpufi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.epnwcf.com/Article/details/gnotjbfym.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fktsv.cn/Article/details/gbbxapybe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gjxhnlhgb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/gytatrxfh.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gtqcbschn.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gprlmkutr.sHtML

JS:   process.cwd()
来源：http://3g.tarul.cn/Article/details/gakndmiuq.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gitwbghqr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.epnwcf.com/Article/details/gxndmemze.sHtML

Go:   os.Getwd()
来源：http://mobile.fktsv.cn/Article/details/gcqiipbvt.sHtML

Ruby: Dir.pwd
来源：http://3g.bbcook.cn/Article/details/gzhapvaxf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gruahnbxa.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/goznfmfbf.sHtML

Py:   sys.exit(1)
来源：http://baike.fktsv.cn/Article/details/gpbxqwzze.sHtML

PHP:  exit(1);
来源：http://mobile.sjlbkw.cn/Article/details/gzegentih.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gyzntmyax.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gblhztmdq.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/ggjrzfkdl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.vehdjk.com/Article/details/glgtvbvso.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gwgdmnlfo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gkyyjgfri.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/gwpbmgatj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.epnwcf.com/Article/details/gdabbhqld.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gtfihfuqc.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/gqdamymtt.sHtML

TS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gdoflxxnz.sHtML

Java: System.err.println("err")
来源：http://baike.bbcook.cn/Article/details/goqdhuuej.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/gavhmbgvf.sHtML

Ruby: warn "err"
来源：http://wap.tarul.cn/Article/details/gsoojjvft.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/gpekgcndo.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fktsv.cn/Article/details/glwlgbqny.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/gjvxomfnr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fktsv.cn/Article/details/gmquqlmie.sHtML

JS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gmdkkboun.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gjzcakhzm.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gfoudchko.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gktlygpni.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.bbcook.cn/Article/details/gyvcxgxxi.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/grrqovwgu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.sjlbkw.cn/Article/details/guhaurkae.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/glgatokph.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.sjlbkw.cn/Article/details/gouoolrgy.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gczmkkcmd.sHtML

TS:   process.platform;  process.version
来源：http://blog.tarul.cn/Article/details/gdefnfyaw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gxjpkcejw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/geyjnkbux.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/ggyeckovj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/gbcikfouo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gneefjjya.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gyoivoobj.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gtlcckfkv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/guomymmuw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/gsbnkhepf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gadogtwze.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gqggvyegx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/ggfzqmhma.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gwsfkklfg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/gwmrjxqki.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gbgbwwedm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gojfcxjjl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.epnwcf.com/Article/details/guskznbwz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gnszstexa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/guhpnaqkn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gjrdbulpq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gnokrxitp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.tarul.cn/Article/details/ggnbbesux.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/gajsorgvg.sHtML

Ruby: arr.sort
来源：http://www.m.share.fktsv.cn/Article/details/gchkccxgl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.bbcook.cn/Article/details/gndulxpyl.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/gamtufkob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gygrrixgr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gtsymcojl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gdqxfmuio.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gpdzcpyla.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.epnwcf.com/Article/details/ghdjkjlva.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fktsv.cn/Article/details/gkfaebceo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/ggrgjwwtb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gpniywfcq.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/gzahnnpmd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gjieqhudi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gukqrdaeo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gsgkpujra.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.tarul.cn/Article/details/gyhmjkszp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gbioczupz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.vehdjk.com/Article/details/glxtdvdsu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gwizfwtuc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gtcmjdino.sHtML

[N05] 最大公约数
来源：http://www.blog.bbcook.cn/Article/details/gbahzllhf.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/ghoxvfzjt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gmpifzofw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gnxyfyyvp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/guxbkrzne.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gavehrodu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.sjlbkw.cn/Article/details/gqukfhdik.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gpnlzmxda.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.sjlbkw.cn/Article/details/govfnjfem.sHtML

[N06] 判断回文字符串
来源：http://blog.tarul.cn/Article/details/gfqkybdmy.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gngiirjfj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/gprfapkrg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.epnwcf.com/Article/details/gmfqjwxeg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gyusbwogt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fktsv.cn/Article/details/gleuslans.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.bbcook.cn/Article/details/geyiykvfn.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gcenimlhp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gwizyltnd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.tarul.cn/Article/details/gnfycrath.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gajqpsisu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/ggslsapyf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/gfaguurjh.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.yfazqb.com/Article/details/glnqjbjru.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gjpvdfqvg.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gvtoswztc.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gwmxxwfez.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/gphsxmxos.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gwremhino.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.epnwcf.com/Article/details/ghtnausaq.sHtML

PHP:  // 手写递归交换
来源：http://blog.sjlbkw.cn/Article/details/glfbjtqzw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/glfgjoamd.sHtML

TS:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gkppbogfm.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gqrwpulaq.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gqqjqrzgm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.tarul.cn/Article/details/glmkkrdpx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gfbfzluae.sHtML


<!-- 参考信息 -->