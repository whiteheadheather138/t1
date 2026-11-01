代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.bbcook.cn/Article/details/guxubtykr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.yfazqb.com/Article/details/grukvjyou.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.epnwcf.com/Article/details/gyjvniydp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.yfazqb.com/Article/details/gevtsuolv.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gofemsjli.sHtML

K. JSON 与序列化
来源：http://wap.epnwcf.com/Article/details/gglpvbptr.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guxkvzrek.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.epnwcf.com/Article/details/ghegrpppg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gyriavvab.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fktsv.cn/Article/details/gkhqoilxo.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fktsv.cn/Article/details/gqnwtaidy.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.epnwcf.com/Article/details/gcyiabnbd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.tarul.cn/Article/details/gcxoffhly.sHtML

Go:   json.Marshal(obj)
来源：http://3g.sjlbkw.cn/Article/details/gmjkfhany.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fktsv.cn/Article/details/ggleysukc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.bbcook.cn/Article/details/gkinvnprr.sHtML

[K02] JSON 字符串转对象
来源：http://wap.vehdjk.com/Article/details/gbenlrunp.sHtML

Py:   json.loads(s)
来源：http://read.share.yfazqb.com/Article/details/gijlebnpk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.yfazqb.com/Article/details/gklcqlswi.sHtML

JS:   JSON.parse(s)
来源：http://read.share.sjlbkw.cn/Article/details/gnqhgkmod.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gygrblcik.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.tarul.cn/Article/details/gszctmbrg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fktsv.cn/Article/details/gfugqeqgo.sHtML

Ruby: JSON.parse(s)
来源：http://baike.sjlbkw.cn/Article/details/gonarvvua.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fktsv.cn/Article/details/gatflxgnz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.vehdjk.com/Article/details/gdkoghcxa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fktsv.cn/Article/details/gdtgnmovs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.bbcook.cn/Article/details/gjstctzpf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gvxaxnown.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.epnwcf.com/Article/details/gelvqqrgi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.tarul.cn/Article/details/gobrdqrfn.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.yfazqb.com/Article/details/gqmdjoxqe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.tarul.cn/Article/details/gubmryiom.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.yfazqb.com/Article/details/glywetubo.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.yfazqb.com/Article/details/gmsdplxan.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.yfazqb.com/Article/details/gbupsrxta.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fktsv.cn/Article/details/gogqhktlc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/gvdknxlvs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gwgsouqiv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/gyvzbsbop.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.sjlbkw.cn/Article/details/ghskaqahr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/gzdzykchf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.bbcook.cn/Article/details/gcvhtpyim.sHtML

[K05] 深拷贝对象
来源：http://wap.tarul.cn/Article/details/ggnkarpmo.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.tarul.cn/Article/details/gdhmtrqny.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fktsv.cn/Article/details/gdcjacvpk.sHtML

JS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gqnqhqmpd.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/gedlmjbue.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.epnwcf.com/Article/details/gjoohdgbz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fktsv.cn/Article/details/gwawawqok.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.sjlbkw.cn/Article/details/gzyayousi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.bbcook.cn/Article/details/gqnltenep.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/grnuqvkmr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.bbcook.cn/Article/details/glcxorjui.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/gutgbtjmr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.epnwcf.com/Article/details/gujyqvmnt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.sjlbkw.cn/Article/details/gajhcammr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.tarul.cn/Article/details/guozhgfkl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.tarul.cn/Article/details/girupjwtc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.vehdjk.com/Article/details/gyakeawfq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gkouzbrvh.sHtML

[K07] 进制转换
来源：http://read.share.sjlbkw.cn/Article/details/gicxeutew.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.tarul.cn/Article/details/gcamzjuab.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.bbcook.cn/Article/details/gdjocusjc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/glbrtotkm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.bbcook.cn/Article/details/gaeollhly.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.sjlbkw.cn/Article/details/gjuaoojgh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/giynhgzvn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/ggexiqvtr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.tarul.cn/Article/details/gtukakzaw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.tarul.cn/Article/details/gdyikuvuj.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.vehdjk.com/Article/details/gwxfrrris.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gtsdbiugu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/ggbxyjlgw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gjevfhruy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.sjlbkw.cn/Article/details/ggrkaqtxh.sHtML

Go:   encoding/gob
来源：http://3g.fktsv.cn/Article/details/gegnniiic.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.epnwcf.com/Article/details/gkeuagejm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.vehdjk.com/Article/details/ggabzfocz.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gxpyrxykv.sHtML

L. 网络请求
来源：http://blog.fktsv.cn/Article/details/gzcpqslip.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/griebigjj.sHtML

[L01] 发送 GET 请求
来源：http://read.share.vehdjk.com/Article/details/gwstvggkj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gpqbtvpad.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.yfazqb.com/Article/details/grempepzp.sHtML

JS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gsrzveyme.sHtML

TS:   await fetch(url)
来源：http://wap.bbcook.cn/Article/details/gejmwonwo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.tarul.cn/Article/details/gtqcpuxxh.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/glogazdtw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.yfazqb.com/Article/details/gtzsyzfux.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.yfazqb.com/Article/details/gjhnokffe.sHtML

[L02] 发送 POST JSON
来源：http://read.share.epnwcf.com/Article/details/gyfxfnmho.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.epnwcf.com/Article/details/gtezbunem.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/gfczjpftk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gcisqnwzy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gpzinkzvq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gfqfizqye.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.vehdjk.com/Article/details/gcaalwcxp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gevnbknrz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gbhpmxogb.sHtML

[L03] 设置自定义请求头
来源：http://3g.vehdjk.com/Article/details/gnqisgdes.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.yfazqb.com/Article/details/gnrlgcxtt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.sjlbkw.cn/Article/details/geyoicgif.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.yfazqb.com/Article/details/gyyaprwxc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gwpghxaze.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gggpkgiws.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/goajgmtvy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/gulorpajx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gpnioimkc.sHtML

[L04] 设置超时
来源：http://read.share.epnwcf.com/Article/details/gdpkthdyn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.tarul.cn/Article/details/gmdsstzxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.sjlbkw.cn/Article/details/gcbsykwdf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.sjlbkw.cn/Article/details/gplwiqlfp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fktsv.cn/Article/details/gmndhzbdv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/ggavkzpme.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gsbslzhxu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.epnwcf.com/Article/details/gasarxwmv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/ghwkcfynd.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.yfazqb.com/Article/details/gvrobmxcq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.epnwcf.com/Article/details/gyvmzgqfc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.bbcook.cn/Article/details/gzpofbsdl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.tarul.cn/Article/details/gtwmzczyx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gvokptgni.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.yfazqb.com/Article/details/gprkgxggz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/grmocerjf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/gjolddmrp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.epnwcf.com/Article/details/gquyoethx.sHtML

[L06] 解析响应为 JSON
来源：http://blog.vehdjk.com/Article/details/gjdmmqrpe.sHtML

Py:   resp.json()
来源：http://baike.bbcook.cn/Article/details/ggueftytz.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/ggzsdvznq.sHtML

JS:   await resp.json()
来源：http://3g.sjlbkw.cn/Article/details/gxwymadpi.sHtML

TS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gzucsuhrb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.epnwcf.com/Article/details/gdtpxahfs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gbpexahjf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gbgslxwpn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gfwevslqr.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.epnwcf.com/Article/details/gsyitceyj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/grnkssfnc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.sjlbkw.cn/Article/details/gamsxomgf.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gpmurytud.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/gqunkmulx.sHtML

Java: resp.statusCode()
来源：http://read.share.fktsv.cn/Article/details/gqghyfffw.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/ghbvhohkv.sHtML

Ruby: resp.code.to_i
来源：http://3g.sjlbkw.cn/Article/details/gzmklwman.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gbpgtoqfd.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.tarul.cn/Article/details/gebxswmua.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gdjchcart.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/gwjolvrlo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gwmbgyiwb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gxyhcjsoe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fktsv.cn/Article/details/grhzbredb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.yfazqb.com/Article/details/gynedftpe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/gmynqzjes.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.epnwcf.com/Article/details/gqhuhpogj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gvrloljuc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/ggepobcno.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gxonoazsb.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gxhomdpeu.sHtML

Py:   sys.argv[1:]
来源：http://www.share.vehdjk.com/Article/details/gkynmjwkn.sHtML

PHP:  $argv;  $argc;
来源：http://blog.yfazqb.com/Article/details/gfubmoaco.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gvwzbdaur.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/gqwasnmif.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/gqrpkjjgo.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/gwifxuecl.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gcrvajgte.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gribzfmxj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gbxpyrtss.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.tarul.cn/Article/details/gpztmnpti.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gudtoeqju.sHtML

JS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gjkyknwgx.sHtML

TS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gnyyidlrw.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.vehdjk.com/Article/details/glgsipnde.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.tarul.cn/Article/details/gswwdvzwk.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.epnwcf.com/Article/details/gdpczvfss.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gaokolooj.sHtML

[M03] 执行外部命令
来源：http://3g.vehdjk.com/Article/details/genuhasbb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gvntbwwni.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.yfazqb.com/Article/details/gbslqqiku.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.tarul.cn/Article/details/gxzshlcja.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.vehdjk.com/Article/details/gneftgvla.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gremyqnnh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.bbcook.cn/Article/details/gkcykqbxb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.tarul.cn/Article/details/gxirzhxnt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.epnwcf.com/Article/details/gvcoxussj.sHtML

[M04] 获取当前工作目录
来源：http://blog.epnwcf.com/Article/details/gnsiktuyk.sHtML

Py:   os.getcwd()
来源：http://blog.bbcook.cn/Article/details/gjdxmeltz.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/galmirztm.sHtML

JS:   process.cwd()
来源：http://wap.bbcook.cn/Article/details/ggypadahm.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gnhczeaze.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gbfgpqtgu.sHtML

Go:   os.Getwd()
来源：http://blog.fktsv.cn/Article/details/gfgtomxzw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/ggsufjstq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/goibcqbpt.sHtML

[M05] 设置退出码
来源：http://m.share.vehdjk.com/Article/details/gtllmmbkm.sHtML

Py:   sys.exit(1)
来源：http://baike.bbcook.cn/Article/details/ggzbrqksq.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/giyqtffbq.sHtML

JS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gxtzqgklo.sHtML

TS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gdnzityqn.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gwhsmdnlk.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/ggxbeicap.sHtML

Ruby: exit 1
来源：http://www.blog.sjlbkw.cn/Article/details/gpbujxkss.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gvsrfxttv.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gqmkdsxoa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.sjlbkw.cn/Article/details/gybzwtjyg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gylyflnje.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gzpsqqutu.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gsywwtwxn.sHtML

Java: System.err.println("err")
来源：http://wap.vehdjk.com/Article/details/gzdnywvua.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fktsv.cn/Article/details/gvxahnvez.sHtML

Ruby: warn "err"
来源：http://m.share.bbcook.cn/Article/details/gqiuxoema.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/glzffcuek.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/gvvgeffjg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gmyubkjxw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gvfgxpvxf.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gnyrrvevd.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gmbrlurcs.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/gjhxhfhto.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/gsxnkupts.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.yfazqb.com/Article/details/gnuzoteyx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gtysjndaf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.vehdjk.com/Article/details/gsevpsgwt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gqukwdngs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gixwidhoh.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gkszsqydq.sHtML

TS:   process.platform;  process.version
来源：http://m.share.epnwcf.com/Article/details/gwiungama.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gnxdubgom.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/gfxmyrlhz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/giqqpuxjp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/gkjenonuj.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gwxxwszwk.sHtML

N. 数据结构与算法
来源：http://wap.sjlbkw.cn/Article/details/gqangydsz.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gjlrjcobu.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gjnzocbaw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gmbssqxjt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fktsv.cn/Article/details/gjhkcgtrb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gwqzynrih.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gocopsqqy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gbishozay.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/getzpnzrp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/glqwtzlxy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gtoqrdxqk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.yfazqb.com/Article/details/gjlzvomkh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gcynoqbut.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gtanyauxe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.yfazqb.com/Article/details/gogmkjuvc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gmleqqxif.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.vehdjk.com/Article/details/gcbukyhko.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gerrywvtl.sHtML

Ruby: arr.sort
来源：http://mobile.epnwcf.com/Article/details/gwzdgznfe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/gseuhksmf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.yfazqb.com/Article/details/gouoehyzo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/guxflxnwi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.epnwcf.com/Article/details/ggtrbvdft.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gzqrgiaxs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gasgzwcdz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gmpjeruyg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.sjlbkw.cn/Article/details/grvumyruk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/gysjwvyeg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gpiuvqgas.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gnqkxvcql.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gdtizwfih.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gcyiizvtg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gokwvugkz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gqnocdafa.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/ghlufaadt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/ghotaxhee.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/glwqzfpye.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/giunqxart.sHtML

[N05] 最大公约数
来源：http://mobile.vehdjk.com/Article/details/gfpxidghi.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/ggazvmeko.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/ghirclwvm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gqthmqcwe.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/getqclrex.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gwapfukov.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/gzwolezjs.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gzycixydo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/gzzcggyja.sHtML

[N06] 判断回文字符串
来源：http://www.share.yfazqb.com/Article/details/gbzpthrmw.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gdlvysgls.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gtaezdqul.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gxpjnmaho.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/ggajnpirs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.sjlbkw.cn/Article/details/gkfalndba.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/gmyfaknpq.sHtML

Ruby: s == s.reverse
来源：http://mobile.tarul.cn/Article/details/gnlspmaym.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/genrgnzth.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.bbcook.cn/Article/details/gdnjmgzyk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/guchjdokw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/goqzxepdf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/gmyevfovf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gzfunagvy.sHtML

Java: // 手写 HashMap
来源：http://blog.bbcook.cn/Article/details/gvglxzncq.sHtML

Go:   // 手写 map[int]int
来源：http://blog.bbcook.cn/Article/details/gfrvcuyzc.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fktsv.cn/Article/details/gldpmwevf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/guadpumjv.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gkcicpcnp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.yfazqb.com/Article/details/gjqkgidxy.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.vehdjk.com/Article/details/ggeewswvc.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/ghkqmnyvt.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gitdekzmr.sHtML


<!-- 参考信息 -->