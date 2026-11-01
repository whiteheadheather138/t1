代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.yfazqb.com/Article/details/gnwvalvzc.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.tarul.cn/Article/details/gzbklookr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fktsv.cn/Article/details/gpuooguab.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.yfazqb.com/Article/details/giblqtvtz.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.epnwcf.com/Article/details/grmnzmbyh.sHtML

Py:   json.loads(s)
来源：http://3g.sjlbkw.cn/Article/details/grijevvwa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fktsv.cn/Article/details/gebodypbu.sHtML

JS:   JSON.parse(s)
来源：http://read.share.bbcook.cn/Article/details/gqvkezjoj.sHtML

TS:   JSON.parse(s)
来源：http://baike.yfazqb.com/Article/details/gqbfwwwae.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.vehdjk.com/Article/details/gebzbbxxr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.tarul.cn/Article/details/gufjxyjuv.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gtcqmdhfw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.yfazqb.com/Article/details/gyjgzratd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.vehdjk.com/Article/details/gwxvyvyip.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/githngqge.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gcojjqqgt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gvkqhuzyn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.bbcook.cn/Article/details/gbcozgshn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/glbiwuakc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.epnwcf.com/Article/details/grdkkjwnb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.bbcook.cn/Article/details/gisjciose.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gnkuhuupg.sHtML

[K04] 读取 JSON 文件
来源：http://3g.bbcook.cn/Article/details/gcxnuzwfh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.yfazqb.com/Article/details/grtjammcj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fktsv.cn/Article/details/gvgigctoh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fktsv.cn/Article/details/gviriiyhx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.tarul.cn/Article/details/ggigirzze.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/gszuwbfhr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.bbcook.cn/Article/details/gejuldglf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.yfazqb.com/Article/details/gbeakkbah.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.bbcook.cn/Article/details/gllodigci.sHtML

[K05] 深拷贝对象
来源：http://blog.bbcook.cn/Article/details/gyejspuzr.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.bbcook.cn/Article/details/gtuqvortv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.epnwcf.com/Article/details/ggqjjxius.sHtML

JS:   structuredClone(obj)
来源：http://www.share.bbcook.cn/Article/details/gnquwigyr.sHtML

TS:   structuredClone(obj)
来源：http://blog.sjlbkw.cn/Article/details/ggyaxwryz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.yfazqb.com/Article/details/gfyqlkftl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.bbcook.cn/Article/details/gwuqctqbq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.vehdjk.com/Article/details/gktwsxuho.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.vehdjk.com/Article/details/gxuxihzvb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.yfazqb.com/Article/details/gtdlsqrxy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/gsgepwrxj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/gkmjluyni.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.bbcook.cn/Article/details/gjifakyba.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gsvyxwwuz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.bbcook.cn/Article/details/gntyvxryv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.tarul.cn/Article/details/grxdpglak.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/gmwedsohs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.tarul.cn/Article/details/guyogkbfv.sHtML

[K07] 进制转换
来源：http://www.share.bbcook.cn/Article/details/gefyilshe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/grhmxtteb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.yfazqb.com/Article/details/gyygszimm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.epnwcf.com/Article/details/gdvxtuuxo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gifhwadfy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gcudekkcy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.yfazqb.com/Article/details/gxoveiqmz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.vehdjk.com/Article/details/gusruyrri.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fktsv.cn/Article/details/gpixmezax.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.tarul.cn/Article/details/ggqbgfhwv.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.epnwcf.com/Article/details/gpdlqnibn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gshopwvwc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gmitckhiq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/geiwxccao.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/grgciuwly.sHtML

Go:   encoding/gob
来源：http://mobile.bbcook.cn/Article/details/gtfnmuzvp.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.epnwcf.com/Article/details/gajcniqkc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gyalyxtpc.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gsntdvwge.sHtML

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/gbndgtrrm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/ghszmtttm.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gxehdsigm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fktsv.cn/Article/details/gfcbxgkes.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.sjlbkw.cn/Article/details/gwngculwc.sHtML

JS:   await fetch(url)
来源：http://m.share.sjlbkw.cn/Article/details/gcionigmp.sHtML

TS:   await fetch(url)
来源：http://3g.bbcook.cn/Article/details/gwtoxcitz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gevxfddgh.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gzgwhxckw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gbqsuhqwf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.sjlbkw.cn/Article/details/gweitqxdu.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.bbcook.cn/Article/details/gfbhktkva.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.bbcook.cn/Article/details/gwgatmtab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gvvhaztas.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gdxgshkpc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/ginemkqih.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gxceanejv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.vehdjk.com/Article/details/guxydrfla.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.yfazqb.com/Article/details/gilxwlnim.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/grksgoula.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gbnecunws.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.vehdjk.com/Article/details/geodoconu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/gmbtvhiqv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.epnwcf.com/Article/details/gquoqafjs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gffgvaehf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gdvkcgwje.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gsffuvmjr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.yfazqb.com/Article/details/gdziduwgp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.vehdjk.com/Article/details/gvctlksxd.sHtML

[L04] 设置超时
来源：http://mobile.sjlbkw.cn/Article/details/gmzpauyms.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/gggfshsln.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gdrzvaive.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gcdmrjhcq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.yfazqb.com/Article/details/gumvmmkss.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/gqpiarhtf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.sjlbkw.cn/Article/details/gqkkqdqtc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.bbcook.cn/Article/details/gsgnrilhe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gupxsmmbu.sHtML

[L05] 上传文件（multipart）
来源：http://baike.sjlbkw.cn/Article/details/gyculmfeh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/gcbywhqtz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.tarul.cn/Article/details/gjumwsudw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.bbcook.cn/Article/details/gopeilquj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gprghtusj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.vehdjk.com/Article/details/gwzfswrbx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/gtommrfoo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fktsv.cn/Article/details/gjpctdyjp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.yfazqb.com/Article/details/gbryhcvqk.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/gyktmkuxo.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/ggdrgfxab.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fktsv.cn/Article/details/gvtervyqz.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gdojazncx.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gyfpurmxk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.vehdjk.com/Article/details/gvmpmulcl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fktsv.cn/Article/details/ghujsejuq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gunacrhwn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gcmhrcosj.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.epnwcf.com/Article/details/gbmgbjqhy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/glsammwso.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.yfazqb.com/Article/details/gfxiocdsg.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.sjlbkw.cn/Article/details/gqxidqplp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.vehdjk.com/Article/details/ghxgwnjpv.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gbunnxnkz.sHtML

Go:   resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gpqudthtp.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gnwmozjds.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/ghmuvkytf.sHtML

[L08] 并发请求多个地址
来源：http://m.share.sjlbkw.cn/Article/details/gwxnwjsuj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.epnwcf.com/Article/details/ghuprgrss.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.sjlbkw.cn/Article/details/gmwkichyq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/guzhbpiqs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gknrotoce.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.sjlbkw.cn/Article/details/ginyejron.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fktsv.cn/Article/details/glrrdwvru.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gdthipqjq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gftrxujtc.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gywvuyzdh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.vehdjk.com/Article/details/goykthgxy.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gqvpmzzjl.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/gsmhcworq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.tarul.cn/Article/details/gidoaeqev.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gaxzvrvsx.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.vehdjk.com/Article/details/gffdtaocm.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/ghtvhaxjt.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gyaijhztk.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gykfllrus.sHtML

Ruby: ARGV
来源：http://www.share.yfazqb.com/Article/details/gnqqndumk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/ghczwluyc.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gbtfckves.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/ghzdaltry.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/geqhojmwo.sHtML

JS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/gnvqndnhz.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gqgmjjreg.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gzcuybwdm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gawbsmkur.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.bbcook.cn/Article/details/gbwqwytqf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/gahrzfayb.sHtML

[M03] 执行外部命令
来源：http://www.share.fktsv.cn/Article/details/gmtrxidvy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.yfazqb.com/Article/details/grsnaoyhf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/glrejoros.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gmyxxlkqs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gkbhpmuuf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/ggyfyawic.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/glabjhajq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gcdhrnfkh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/gfbgzstpf.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gaxjodydz.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gvlfegybz.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gsyodyeei.sHtML

JS:   process.cwd()
来源：http://www.blog.tarul.cn/Article/details/ghngdxmtq.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/giujcusqi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.epnwcf.com/Article/details/gtawgfvht.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gujnfbybm.sHtML

Ruby: Dir.pwd
来源：http://www.share.vehdjk.com/Article/details/gspzdavha.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.bbcook.cn/Article/details/gbgifdeqk.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/ghqeufhdj.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gdqrjkhvm.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gwcsgxjss.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gdjolphub.sHtML

TS:   process.exit(1)
来源：http://read.share.bbcook.cn/Article/details/guwxkyjny.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gncuyrbww.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gyavdgyri.sHtML

Ruby: exit 1
来源：http://mobile.epnwcf.com/Article/details/gjporlpas.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/gypfgvlkq.sHtML

[M06] 向标准错误输出
来源：http://www.share.tarul.cn/Article/details/geixzknkb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gmsykrqkn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.bbcook.cn/Article/details/grzqiruxk.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gaijyztpk.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gdeqbjpve.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/gauhzytzk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/gldaogvhk.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyhlwaci.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/gmdbdgrkq.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/gmeidrysg.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gqhlqpyvg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/gmdrmgjkp.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gnovotigy.sHtML

TS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/glctzbvys.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gtrdgnosa.sHtML

Go:   func main()
来源：http://blog.vehdjk.com/Article/details/gaojmmbem.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/gcfpzxfcg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.bbcook.cn/Article/details/gddbyufpw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gjvxfmpkv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gfxwqoszi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/ghtpmwzkx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gwrljrunk.sHtML

TS:   process.platform;  process.version
来源：http://mobile.yfazqb.com/Article/details/ghuedkugz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/grvyeinzf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.vehdjk.com/Article/details/gamjdpils.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.vehdjk.com/Article/details/gmvqcbhvc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gmfxcmiit.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gkxvslczj.sHtML

N. 数据结构与算法
来源：http://blog.vehdjk.com/Article/details/gsbzroqae.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gamhtxxzz.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.vehdjk.com/Article/details/gwvwhvjdi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gltsafcjy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gcyssexdk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gferkcfvq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gjucircia.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gqgjzmfel.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/gencjtiip.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gmclsdoob.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gxwqmroke.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.bbcook.cn/Article/details/gerdmrkvn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fktsv.cn/Article/details/gpdpzjaad.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/goibjeqkq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.vehdjk.com/Article/details/gvwcnphrp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gqbxnmtal.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/grkxeimdn.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gwhdqolee.sHtML

Ruby: arr.sort
来源：http://www.share.bbcook.cn/Article/details/gzjgakjum.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/gizntifrw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.sjlbkw.cn/Article/details/guqvnkztt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.bbcook.cn/Article/details/gdkraxkkw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/ggurludqj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gyswutevo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gkxgmodqi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gzpoiqfoq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgpwifef.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gvbhawljc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.bbcook.cn/Article/details/ghspvwpre.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/gzxacuyuv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gseanmnxa.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.tarul.cn/Article/details/gjoixoyrc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gjdhnhqot.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/gxjhabgcq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gcptgjnge.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/gwqthdyrf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gdnuodlou.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gtqnqyolu.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/geyiaxyxq.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.sjlbkw.cn/Article/details/ggliignfo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/ggpehqgjc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gjgzfddxp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gsiufqcgo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.yfazqb.com/Article/details/gnmzjsnek.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.vehdjk.com/Article/details/gooddlwwm.sHtML

Ruby: a.gcd(b)
来源：http://3g.vehdjk.com/Article/details/gdtlczgjx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fktsv.cn/Article/details/gtnwrmtwl.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gburshdqe.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gjwahrdwn.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gczvjyydv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gthtgrtie.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gmzzhjvdn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gopqvzyzx.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/gwqnpmnhq.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gftvytzrk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.tarul.cn/Article/details/gknwxiuhr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gvzpfcdsp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.bbcook.cn/Article/details/gtcyxgfud.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.bbcook.cn/Article/details/gkvfyjfje.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.vehdjk.com/Article/details/gxcqdstzb.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/grvoovszg.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gtjbmyiur.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/gdltkdagp.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.yfazqb.com/Article/details/ghnuctroi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gvbhsigwr.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/glhwjwktq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/grquhwjgt.sHtML

PHP:  // 手写递归交换
来源：http://baike.fktsv.cn/Article/details/gfmzyojtj.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/ggvufbqgk.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gdybepwzu.sHtML

Java: // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/glqtxoijk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gzcrqkphp.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.yfazqb.com/Article/details/gmxszhzlb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/ggublzhte.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/glnxvcpsg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/ghaktkfmu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/grmfhtlqu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gikhhdsjf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gomiowjsg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gwbgudteh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gwrunblxe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gcvrbwfov.sHtML


<!-- 参考信息 -->