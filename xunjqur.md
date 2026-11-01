代发 wailian999

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gxdpgctaz.sHtML

K. JSON 与序列化
来源：http://wap.fktsv.cn/Article/details/gbanvcjfd.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gtmmmcmsl.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.epnwcf.com/Article/details/gpodoebkj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/grefgwmtm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gllrrdwzp.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.yfazqb.com/Article/details/gtrwlcmsx.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.epnwcf.com/Article/details/gdhhbcwrs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.bbcook.cn/Article/details/gcooijbei.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.yfazqb.com/Article/details/gdbydrfom.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.tarul.cn/Article/details/gvmbcdrsz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.vehdjk.com/Article/details/grxbnohuc.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fktsv.cn/Article/details/gbvmmkaar.sHtML

Py:   json.loads(s)
来源：http://www.blog.bbcook.cn/Article/details/ggnoxurjy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fktsv.cn/Article/details/gpvparamm.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.tarul.cn/Article/details/gzaquejzg.sHtML

TS:   JSON.parse(s)
来源：http://blog.fktsv.cn/Article/details/gblauzmaj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.tarul.cn/Article/details/ghaxxcrhw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.epnwcf.com/Article/details/gdwfeucdq.sHtML

Ruby: JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/guhapetbb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gqpdzivbr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.bbcook.cn/Article/details/gvopaokpo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.epnwcf.com/Article/details/gktozjuyh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.bbcook.cn/Article/details/gxaxakeeb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gepfapfmv.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.bbcook.cn/Article/details/gcplblvfo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gtrfjdtut.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.vehdjk.com/Article/details/gzwqaooqx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.vehdjk.com/Article/details/gjkndqfla.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.epnwcf.com/Article/details/gdpucleht.sHtML

[K04] 读取 JSON 文件
来源：http://blog.sjlbkw.cn/Article/details/gzxupgrrl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.tarul.cn/Article/details/gnxvmjxuh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.bbcook.cn/Article/details/gnfsqudwo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.sjlbkw.cn/Article/details/gyhzlidxd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.vehdjk.com/Article/details/gchyqdgfj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gpwdpugpk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gxhsyvbpi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.epnwcf.com/Article/details/goofjgbzk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.yfazqb.com/Article/details/gmsmordrd.sHtML

[K05] 深拷贝对象
来源：http://3g.sjlbkw.cn/Article/details/gzoefpfas.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gpgxflsah.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.tarul.cn/Article/details/gylbggpyg.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/gazyjtiog.sHtML

TS:   structuredClone(obj)
来源：http://wap.sjlbkw.cn/Article/details/gdjszpdof.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/gqysmosbi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gqkmsvybw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fktsv.cn/Article/details/gsfcfgrai.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.yfazqb.com/Article/details/gdbrjptyx.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fktsv.cn/Article/details/giorelmka.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gddjkqsdm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.sjlbkw.cn/Article/details/glrisnnnm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gsdjkcakh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.yfazqb.com/Article/details/gkkesfcec.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.bbcook.cn/Article/details/gqkxugtyu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/ghcsueabd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.sjlbkw.cn/Article/details/gwgyvoyne.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gybdohiov.sHtML

[K07] 进制转换
来源：http://baike.sjlbkw.cn/Article/details/ggotsiguj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gwxaxytcp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/grddxnuzi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gfqwlthai.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gqpiodrcc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.bbcook.cn/Article/details/gusjhgplt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.yfazqb.com/Article/details/gtqmpsynj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.sjlbkw.cn/Article/details/gmaxmsreg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gotbbyzor.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/ghhnfirtm.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.epnwcf.com/Article/details/gecfybarl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.bbcook.cn/Article/details/guifqwyym.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fktsv.cn/Article/details/ghratmewk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/gjidfwkga.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.tarul.cn/Article/details/gzfjfaxpm.sHtML

Go:   encoding/gob
来源：http://www.m.share.sjlbkw.cn/Article/details/gzpwokyhf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.yfazqb.com/Article/details/gnkalorir.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.tarul.cn/Article/details/giiwzxcgx.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gesvwoiey.sHtML

L. 网络请求
来源：http://3g.sjlbkw.cn/Article/details/gepicgmty.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gfdawdvup.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.bbcook.cn/Article/details/gyefhfgxx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.epnwcf.com/Article/details/gsvmlekxe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fktsv.cn/Article/details/gkfjmwjlb.sHtML

JS:   await fetch(url)
来源：http://www.share.fktsv.cn/Article/details/gnectaftg.sHtML

TS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/grrexohmb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/gabmzttdg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.vehdjk.com/Article/details/gyxznduma.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.tarul.cn/Article/details/goiyfslye.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.vehdjk.com/Article/details/goqnktogl.sHtML

[L02] 发送 POST JSON
来源：http://blog.tarul.cn/Article/details/gmgynczwz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.bbcook.cn/Article/details/gegrggmwa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.yfazqb.com/Article/details/gtfxbqtwl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.sjlbkw.cn/Article/details/gthzscvco.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.epnwcf.com/Article/details/gzxiufnkt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.tarul.cn/Article/details/gdprecoly.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.vehdjk.com/Article/details/gwopvtahj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fktsv.cn/Article/details/gfilvrwty.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gyglddohk.sHtML

[L03] 设置自定义请求头
来源：http://read.share.tarul.cn/Article/details/gkdqhpnoz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.sjlbkw.cn/Article/details/ggqjkcpbl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.epnwcf.com/Article/details/gybnutxcv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.bbcook.cn/Article/details/gywxcbhgt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gouqqimek.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/guglevksq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/gsmithozo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.vehdjk.com/Article/details/gvqepjmgi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fktsv.cn/Article/details/gkhpgvhpe.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gwbpiecws.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.epnwcf.com/Article/details/gzrbcsdkr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.tarul.cn/Article/details/gyrizcngk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/gfomfadfq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/guqyyidme.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gokgcukje.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gbprnzeph.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.sjlbkw.cn/Article/details/gevrmbemb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/gpuxppacv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.tarul.cn/Article/details/gdqipfafv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.tarul.cn/Article/details/gfnyryzrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.vehdjk.com/Article/details/gvtkejwfm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gwgycrzir.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.epnwcf.com/Article/details/gfylbhvjy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.epnwcf.com/Article/details/ggwabutpx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.vehdjk.com/Article/details/gozbafqdj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/guxnescxq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/gjigrvzlc.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.sjlbkw.cn/Article/details/gakpandur.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gbreqhcdk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.bbcook.cn/Article/details/gfaamynwp.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gocacvavf.sHtML

TS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/gpwrqteyh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/grjdatdkr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gwdouywil.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/gzclycmxy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gmlqxpvxp.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gpfxuipjy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.tarul.cn/Article/details/glpmxphsu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbknmlcrn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.tarul.cn/Article/details/gciphlzfy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gpcptkngf.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gpkfbrhjn.sHtML

Go:   resp.StatusCode
来源：http://read.share.yfazqb.com/Article/details/gsvlpmnhi.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gtinvwwvk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gcbbtbifk.sHtML

[L08] 并发请求多个地址
来源：http://m.share.tarul.cn/Article/details/gesfgpvok.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gftsxfgnr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.tarul.cn/Article/details/gomtkoryc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/geshunrso.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gxqduahab.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.sjlbkw.cn/Article/details/gdamrwqmz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.sjlbkw.cn/Article/details/gcewjqfnr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.epnwcf.com/Article/details/ggytqkqmz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/gznuupxlf.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gclifkxhd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/glinwjbow.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gvkotwewx.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/geveqyxjs.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gahriptjn.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/guzkwxslr.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/guwjsslzw.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gepxyfazh.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gekeakvxw.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/gutnkvpww.sHtML

Ruby: ARGV
来源：http://wap.fktsv.cn/Article/details/gmiuofocz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gelcrkpej.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/ggtgpwvql.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzayqxrs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gzusswweu.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gcvpwwxff.sHtML

TS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gcuzdnvjf.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/gwvdtejoh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/gfkkuduop.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.bbcook.cn/Article/details/gtyhafipj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gbebujwyf.sHtML

[M03] 执行外部命令
来源：http://3g.bbcook.cn/Article/details/gkltjjfwx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gnfxrltta.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/geztszneb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gvufilivz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.yfazqb.com/Article/details/ggcnthzrg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.vehdjk.com/Article/details/gcvhjvbde.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.yfazqb.com/Article/details/gxijtdrit.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.vehdjk.com/Article/details/gvkcbblxj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gbafqnfkh.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/gtgnbbffm.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/ghlxppgyy.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gjcsgjvii.sHtML

JS:   process.cwd()
来源：http://wap.tarul.cn/Article/details/gwejxoker.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gmokuwkmf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gxbvburng.sHtML

Go:   os.Getwd()
来源：http://m.share.tarul.cn/Article/details/gafwosaxe.sHtML

Ruby: Dir.pwd
来源：http://wap.epnwcf.com/Article/details/gybqdnngj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/glrgfrfxb.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gvnhhjgre.sHtML

Py:   sys.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gfcfiagjr.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gdrhgeuwl.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gjrvhrnch.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gqglztgec.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gegelemoc.sHtML

Go:   os.Exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gldriltsv.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gomepafxp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.epnwcf.com/Article/details/gqqdthofr.sHtML

[M06] 向标准错误输出
来源：http://baike.yfazqb.com/Article/details/gshouyptr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gsdnkdrcp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/gpjucaylx.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gcubopzfh.sHtML

TS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gagiwvkuq.sHtML

Java: System.err.println("err")
来源：http://3g.epnwcf.com/Article/details/gocdcyjfx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.epnwcf.com/Article/details/gtnqjzumh.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gajcxmtgv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/gwzkcczof.sHtML

[M07] 判断是否为主入口
来源：http://wap.fktsv.cn/Article/details/gtresyibb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.bbcook.cn/Article/details/ggelqcqqa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gavavcmqd.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gqnduivdm.sHtML

TS:   require.main === module
来源：http://mobile.fktsv.cn/Article/details/gkgelvbia.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gulxsmufc.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gqhrmwckh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gqbqnvqgd.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gweaumzaf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.tarul.cn/Article/details/gtigzsyeo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gzxbmupbu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/grvcyfmgo.sHtML

JS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/glsbucpnb.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gtiyvdjxb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/goicircdn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/gqxlqxzxz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gjblhopkh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/ghqqyhrap.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gusndzibh.sHtML

N. 数据结构与算法
来源：http://mobile.sjlbkw.cn/Article/details/gqjbtglzu.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glyedzhzd.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.yfazqb.com/Article/details/glhtoxeuc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gtzymvvnf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/ghrlnbilv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gecowrymc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gifrrwkku.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gajlpjmzl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/gfhoocjly.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.yfazqb.com/Article/details/gbbvfcvna.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gfjbohgog.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.yfazqb.com/Article/details/gswqmcbuh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gkidgswtj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/gxjobodjx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/govftntvt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/galfcakrt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/ghiuwioso.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gaezcqxfw.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gkoytavts.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/goxxmqtkz.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fktsv.cn/Article/details/gztrisdsp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gpcqgghbf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/gpymcxwhi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gulcxgdeu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gmiyvjdkm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gpatxgfxb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fktsv.cn/Article/details/gnvmavoeo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.bbcook.cn/Article/details/gfqysfkim.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.bbcook.cn/Article/details/gwqfaqwej.sHtML

[N04] 斐波那契数列
来源：http://baike.fktsv.cn/Article/details/gzqmuqbyp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gvtxwqkev.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gexfwpvpp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/ghtzgxfhw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gnrogvaoy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gjhtqggnp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.tarul.cn/Article/details/gdysujhzw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gzsezsxmh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/ghfyplkvj.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gtebwkcmo.sHtML

Py:   math.gcd(a, b)
来源：http://3g.vehdjk.com/Article/details/gfsktizyk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gdmkgohhp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gxxsqldxp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.yfazqb.com/Article/details/gpwxtalcw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.yfazqb.com/Article/details/gotpwwmzw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/guhrycory.sHtML

Ruby: a.gcd(b)
来源：http://blog.yfazqb.com/Article/details/gfmkcquhw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gykhyanba.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/gtqofltxa.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gqnxfgotp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.tarul.cn/Article/details/ggxlltldj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gqlnxabxk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.yfazqb.com/Article/details/ggweqqkag.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.tarul.cn/Article/details/gpqtjjebm.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.tarul.cn/Article/details/goctfhuzb.sHtML

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gbwrtakvg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/gajdmhsjm.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gloumwiwj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/goumiuajk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.tarul.cn/Article/details/gnfykckad.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/getugdvqy.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gtfiwuqdj.sHtML

Java: // 手写 HashMap
来源：http://baike.fktsv.cn/Article/details/giloggazk.sHtML

Go:   // 手写 map[int]int
来源：http://blog.epnwcf.com/Article/details/grudoeigz.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/giolodcge.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fktsv.cn/Article/details/gmhpqpvrm.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gztgqrpsf.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gnvnmayyk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/glxekjpsb.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gmnxfnzms.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gwdigiiui.sHtML

Java: // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/ggleqbmhd.sHtML

Go:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gzzsamlwu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gzcyyzwao.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gwdbzycmi.sHtML


<!-- 参考信息 -->