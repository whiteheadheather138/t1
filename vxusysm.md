代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.blog.yfazqb.com/Article/details/guwbxgenr.sHtML

Py:   json.loads(s)
来源：http://wap.epnwcf.com/Article/details/gzflesudj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.bbcook.cn/Article/details/gtpdpyqei.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.epnwcf.com/Article/details/gxxpavfwg.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.bbcook.cn/Article/details/gipegogzr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.epnwcf.com/Article/details/gpokqithg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.yfazqb.com/Article/details/guxiirfag.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.bbcook.cn/Article/details/gbpsoqqlu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/gewvanobm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fktsv.cn/Article/details/gogupiajc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.vehdjk.com/Article/details/gulkpdioi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.epnwcf.com/Article/details/gzcnewnzl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.tarul.cn/Article/details/gnwqdtcqf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gytbtiupb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fktsv.cn/Article/details/gqgmxeapd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.bbcook.cn/Article/details/gepuxqkcm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.bbcook.cn/Article/details/gbncvckyz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fktsv.cn/Article/details/gewhiioys.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.yfazqb.com/Article/details/gmkiynkyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.sjlbkw.cn/Article/details/gofyjauir.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.epnwcf.com/Article/details/gzmdmciui.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/ghecvzvyf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.yfazqb.com/Article/details/gengjfziy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.yfazqb.com/Article/details/ggaeqfzjs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gndwpfafv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fktsv.cn/Article/details/gmbfyrpwu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.sjlbkw.cn/Article/details/glkoemhzj.sHtML

[K05] 深拷贝对象
来源：http://blog.sjlbkw.cn/Article/details/grdtxmpeq.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.vehdjk.com/Article/details/gyskpjtzj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gftkjtzug.sHtML

JS:   structuredClone(obj)
来源：http://3g.fktsv.cn/Article/details/gtztnhgpm.sHtML

TS:   structuredClone(obj)
来源：http://blog.bbcook.cn/Article/details/giaqtoagf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/gqwvrzgom.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.vehdjk.com/Article/details/gankexron.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fktsv.cn/Article/details/gcqebzaxo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fktsv.cn/Article/details/gsnavxgjc.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.epnwcf.com/Article/details/gewtjkkqi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.yfazqb.com/Article/details/gykrvwwcx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.yfazqb.com/Article/details/guvimncst.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.sjlbkw.cn/Article/details/geqnlpcud.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/giygcyekv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.epnwcf.com/Article/details/gyeycvkoo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gavchyhhf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fktsv.cn/Article/details/grrxnlrik.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/gasguqdwf.sHtML

[K07] 进制转换
来源：http://m.share.sjlbkw.cn/Article/details/gonafczoi.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.tarul.cn/Article/details/gcjtxrjtt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fktsv.cn/Article/details/gaoxgstkt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/gyruwgvvi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fktsv.cn/Article/details/gcyuojeis.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gbvupsqrc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.bbcook.cn/Article/details/gdvachdmk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.bbcook.cn/Article/details/gizluvbrp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gxizeeqct.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/gmhveiytc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gkmrvcmqe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.sjlbkw.cn/Article/details/gzinqovme.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.sjlbkw.cn/Article/details/glpzeaxwg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.yfazqb.com/Article/details/gyhogfviy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.bbcook.cn/Article/details/gzczcsvfh.sHtML

Go:   encoding/gob
来源：http://read.share.yfazqb.com/Article/details/gpgeducen.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.sjlbkw.cn/Article/details/gpygkkvmh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.yfazqb.com/Article/details/gouldhhph.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqmqzpkch.sHtML

L. 网络请求
来源：http://www.blog.tarul.cn/Article/details/gbcbfmeuy.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqvsfianm.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gvhmhljee.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.tarul.cn/Article/details/gbaaiyhbm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/gyrfzgyuk.sHtML

JS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gzfgynvyb.sHtML

TS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gzsmtaeoe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.yfazqb.com/Article/details/geobvxrxb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.bbcook.cn/Article/details/gmgwibvwl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.vehdjk.com/Article/details/gzvpgnzwm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/gbiboxeak.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gfxhwfsvq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.epnwcf.com/Article/details/gwgkcoksu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.tarul.cn/Article/details/gkpsdvkni.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gjqubixxl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.epnwcf.com/Article/details/ghbzangvt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gbdmhrihs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.yfazqb.com/Article/details/gmmirvozx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.sjlbkw.cn/Article/details/gbvrhftnd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/garkxurrl.sHtML

[L03] 设置自定义请求头
来源：http://blog.tarul.cn/Article/details/gbbmocufd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.sjlbkw.cn/Article/details/gfajirkzu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.bbcook.cn/Article/details/guqvabyav.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gqcfmoeef.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gliwislgf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fktsv.cn/Article/details/gzbztlwmv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/grbossaly.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.tarul.cn/Article/details/ggcckdamx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/ghpavmmii.sHtML

[L04] 设置超时
来源：http://www.m.share.vehdjk.com/Article/details/gjirplgrv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.tarul.cn/Article/details/geuovhkgr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.tarul.cn/Article/details/gznvgwukp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/ggmweonhq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gnwgjacln.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.bbcook.cn/Article/details/gdgaxwaij.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.sjlbkw.cn/Article/details/gqmuzmjbr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.yfazqb.com/Article/details/gnmxvrzuk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.epnwcf.com/Article/details/gbzmgskzf.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fktsv.cn/Article/details/gnueckzqk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.vehdjk.com/Article/details/gbfvffyav.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/geokrnqtz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.yfazqb.com/Article/details/gkcddfmnv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fktsv.cn/Article/details/gufolfydh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.yfazqb.com/Article/details/gybqogobl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.vehdjk.com/Article/details/grtrhnzks.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.yfazqb.com/Article/details/gsvwrawhf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.bbcook.cn/Article/details/gvqktswvm.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gxarleopv.sHtML

Py:   resp.json()
来源：http://blog.epnwcf.com/Article/details/gdpruhurd.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/gabuzcsvn.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gngtngssk.sHtML

TS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/glsgjhiyg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.tarul.cn/Article/details/gvsinxriq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.vehdjk.com/Article/details/gobusdgae.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.bbcook.cn/Article/details/ggrnkmjzd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gpyhwnswf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gewxbqeyk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.yfazqb.com/Article/details/gyzyodhdo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fktsv.cn/Article/details/gljxhwijf.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gdsutswjl.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gphpselbf.sHtML

Java: resp.statusCode()
来源：http://mobile.fktsv.cn/Article/details/gbksbbben.sHtML

Go:   resp.StatusCode
来源：http://www.blog.sjlbkw.cn/Article/details/gnwmilnpu.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fktsv.cn/Article/details/gsuksbbzy.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/glhfqngtj.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/grcogevsh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gbyqnmzkk.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.vehdjk.com/Article/details/gqsgvcnfk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.bbcook.cn/Article/details/glyzibuaq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fktsv.cn/Article/details/gyixplcqf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.vehdjk.com/Article/details/gxcngnvpu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.vehdjk.com/Article/details/gmjwsoytn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.sjlbkw.cn/Article/details/gdrgxsubn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gcylzcgrx.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glczysjim.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.tarul.cn/Article/details/grjqjgqdc.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxowlhqvt.sHtML

[M01] 读取命令行参数
来源：http://m.share.fktsv.cn/Article/details/gpfbqtibd.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gvzrtktui.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/gdbsmzopw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gxvblpivn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.epnwcf.com/Article/details/gnjyxplqo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gkppupklu.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gfpsvtogq.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gyhyrfpxj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gmjdwhllx.sHtML

[M02] 读取环境变量
来源：http://blog.sjlbkw.cn/Article/details/gfpuvvbhq.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gklloqegh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.bbcook.cn/Article/details/gzajbkvyg.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/glrrssxng.sHtML

TS:   process.env.HOME
来源：http://mobile.epnwcf.com/Article/details/gnhyzgybs.sHtML

Java: System.getenv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gpynjldrs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/ghpsodnxt.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/ghrgsbjms.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/gfjhohonf.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gbnyeclzs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gjqlzhlna.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gqauekxzv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gxpdeiguo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gyyrhujhe.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/ggfunpwib.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.yfazqb.com/Article/details/gjumwaset.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/gfjahmeie.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.tarul.cn/Article/details/gmorlfwig.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gzqjfojfl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gwfafdkay.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/ghsvokewa.sHtML

JS:   process.cwd()
来源：http://www.share.yfazqb.com/Article/details/ggyjacomk.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gyynvljds.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.vehdjk.com/Article/details/gjviglvji.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gumxptugd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gpgwvcayd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.bbcook.cn/Article/details/gsujgxggm.sHtML

[M05] 设置退出码
来源：http://mobile.bbcook.cn/Article/details/gmkkclqwc.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/geozjjrne.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gfonnsdcd.sHtML

JS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gpzlcceot.sHtML

TS:   process.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gydnpziuh.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gneulydsx.sHtML

Go:   os.Exit(1)
来源：http://mobile.fktsv.cn/Article/details/gufouykxz.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gsgniixcu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/gdrcgyiui.sHtML

[M06] 向标准错误输出
来源：http://www.blog.epnwcf.com/Article/details/gemulabwd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gyfjsohtm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.yfazqb.com/Article/details/ghdjrtpez.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/ghvmcykko.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gtutzrktg.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gtlpkvsqh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gheietham.sHtML

Ruby: warn "err"
来源：http://baike.yfazqb.com/Article/details/gbpjlvwyu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/gvkalxudg.sHtML

[M07] 判断是否为主入口
来源：http://www.share.bbcook.cn/Article/details/gpvbejzjc.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.epnwcf.com/Article/details/gquemgvcl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.bbcook.cn/Article/details/gptfswipp.sHtML

JS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/gnzycodzd.sHtML

TS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gqxsnamyy.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fktsv.cn/Article/details/gnkrtsjvp.sHtML

Go:   func main()
来源：http://mobile.bbcook.cn/Article/details/gfrndbkdt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gbgtyqxqd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gzkesiadd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/gxfwomosx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gcayriluv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gchexghkw.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gdquyecpt.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gexgjwgah.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fktsv.cn/Article/details/ggmhuevcy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gtuffqmtu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gmgvrwlli.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.epnwcf.com/Article/details/goudpsiyx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gyedopqve.sHtML

N. 数据结构与算法
来源：http://blog.sjlbkw.cn/Article/details/ggixbwece.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gbaihnmbi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gnnqwmlnw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.bbcook.cn/Article/details/gvrnfejpd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.epnwcf.com/Article/details/gaensdcso.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gtxdgdhfg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gmknbweoe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/gqxnghpow.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/graiinjjt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gteoxusxz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gyacagnxt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gyqtwjvhb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gajykcvop.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.bbcook.cn/Article/details/glifxvqsk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gpyuqrkgq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/ggrozonec.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/gyhgtetlo.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gbhtmnluf.sHtML

Ruby: arr.sort
来源：http://www.blog.bbcook.cn/Article/details/gbcuwxnao.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gvlnjitia.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gvevuxzra.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gajwigrnp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gwujpgsxf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.epnwcf.com/Article/details/gahokepuk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/giptqyyne.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.vehdjk.com/Article/details/gglcfkpcd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/gjojkpips.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gthhkmliu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/gatercakg.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/gtrupovys.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/grdqdvnaw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/gtjvnqmbv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/groxabedh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gwvrhpmgw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.sjlbkw.cn/Article/details/gahqbpfyp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gdmolmwpx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gtkbrbwzh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gnbfreyhg.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gjhcdfzuu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fktsv.cn/Article/details/gzchrpxgi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gjeoftjst.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.sjlbkw.cn/Article/details/gloouoqrb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gsewthsrw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/gndrmmnpz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/gedvhilws.sHtML

Ruby: a.gcd(b)
来源：http://blog.epnwcf.com/Article/details/gqvhofddc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/geuwoqfpo.sHtML

[N06] 判断回文字符串
来源：http://wap.bbcook.cn/Article/details/gxqzhdaza.sHtML

Py:   s == s[::-1]
来源：http://blog.vehdjk.com/Article/details/grobdnufv.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.tarul.cn/Article/details/gvbfigutp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gvoecwwre.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.yfazqb.com/Article/details/gdxjkurmh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/grkcjylos.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gbfdtjycf.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/gozvtgeke.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.vehdjk.com/Article/details/gjbtyjryh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.tarul.cn/Article/details/gcxohrpep.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.vehdjk.com/Article/details/gsrergscv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fktsv.cn/Article/details/gsrjhffil.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.bbcook.cn/Article/details/gfmrpjprc.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gfayzozwd.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gdmilnhcu.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.vehdjk.com/Article/details/gwzhpcyzp.sHtML

Ruby: // 手写 Hash
来源：http://read.share.bbcook.cn/Article/details/geymrnosv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gdhvbgxrp.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gqnspkjpv.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fktsv.cn/Article/details/geyzlsbex.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fktsv.cn/Article/details/gkmyqwxku.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gubehacfa.sHtML

TS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gynorxbkr.sHtML

Java: // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gihnblton.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gikhoadys.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gvkvhhpmy.sHtML

C#:   // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/ggxjhrqzd.sHtML

[N09] 栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/grecxeebp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gkrvnguyx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.tarul.cn/Article/details/gdaujylln.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gpsomvqkd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gtpshoycj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.bbcook.cn/Article/details/gpccihdjl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gbqebjijh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gmleuxsux.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gyiiddoiz.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/gxnxigdtm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gjibpriko.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/grdkwfaoe.sHtML


<!-- 参考信息 -->