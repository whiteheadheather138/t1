代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.m.share.tarul.cn/Article/details/gusfpjouk.sHtML

Py:   json.loads(s)
来源：http://m.share.vehdjk.com/Article/details/gsvmycezl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.vehdjk.com/Article/details/gqxnjmtie.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.vehdjk.com/Article/details/guwnespcy.sHtML

TS:   JSON.parse(s)
来源：http://3g.fktsv.cn/Article/details/gerjfewjv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gjmdqxnas.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.bbcook.cn/Article/details/gkzchpcoc.sHtML

Ruby: JSON.parse(s)
来源：http://3g.vehdjk.com/Article/details/gmynitbgq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.epnwcf.com/Article/details/gxyacvhfk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/ghvgktcrg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.yfazqb.com/Article/details/glckxkdvp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.sjlbkw.cn/Article/details/gpizbotza.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.vehdjk.com/Article/details/gpddwloqz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.yfazqb.com/Article/details/grnkesojz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/gjwnczrsl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.sjlbkw.cn/Article/details/gnnawwmsx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.epnwcf.com/Article/details/gkjotndcp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.epnwcf.com/Article/details/gufufsruw.sHtML

[K04] 读取 JSON 文件
来源：http://3g.epnwcf.com/Article/details/grxabrokt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.tarul.cn/Article/details/gogdgrkdo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gardhqhru.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gouugskth.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.tarul.cn/Article/details/gwmhwangg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.tarul.cn/Article/details/ghjdwckrr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.tarul.cn/Article/details/gaxjkvczh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/gjbhhqiox.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.bbcook.cn/Article/details/giqgenink.sHtML

[K05] 深拷贝对象
来源：http://read.share.yfazqb.com/Article/details/ggpvwbrod.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fktsv.cn/Article/details/gspwegtus.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.tarul.cn/Article/details/gcdcnzhcg.sHtML

JS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gilghvmhq.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fktsv.cn/Article/details/gfralibru.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.sjlbkw.cn/Article/details/gxbcqngmp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.sjlbkw.cn/Article/details/gcsqmixug.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.tarul.cn/Article/details/gvfponmdm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.bbcook.cn/Article/details/gpsgpztbk.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gosvznklr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.tarul.cn/Article/details/gdfgcpxod.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.bbcook.cn/Article/details/gphwlasbu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gpwueygjw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gsrcxmbtm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.epnwcf.com/Article/details/gkrelzgpd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.bbcook.cn/Article/details/gyvddeksm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fktsv.cn/Article/details/gzjxjedbt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.bbcook.cn/Article/details/grdvtrcmk.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/gvchqzyzm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gvqnwfczc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.tarul.cn/Article/details/gohoiatfd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/giemlqzyu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.epnwcf.com/Article/details/gwhpsabbu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.tarul.cn/Article/details/goxzdgzpp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fktsv.cn/Article/details/gbinnupov.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gzapsliyn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gyjbewijw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.yfazqb.com/Article/details/glscqopwt.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gnfjdyjtz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.bbcook.cn/Article/details/gtieqryyi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fktsv.cn/Article/details/gsraejrch.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.sjlbkw.cn/Article/details/goyymwjyx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.vehdjk.com/Article/details/glmatphkw.sHtML

Go:   encoding/gob
来源：http://baike.epnwcf.com/Article/details/goilxlfvs.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.bbcook.cn/Article/details/gjwrmbjwg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gyrgetixh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grtsjaluw.sHtML

L. 网络请求
来源：http://www.blog.epnwcf.com/Article/details/gybmryned.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gitsfusyk.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fktsv.cn/Article/details/ghwwfamgy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.vehdjk.com/Article/details/gjqdcexvr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/giulcrkgs.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/grwksydbk.sHtML

TS:   await fetch(url)
来源：http://baike.fktsv.cn/Article/details/gcbcmnjxw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.epnwcf.com/Article/details/gvpujuoyg.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gpgbpsxjh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.sjlbkw.cn/Article/details/gphayyjoo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.sjlbkw.cn/Article/details/gxmmavyan.sHtML

[L02] 发送 POST JSON
来源：http://www.share.yfazqb.com/Article/details/gcsfmsjee.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/glqpabeka.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.epnwcf.com/Article/details/gonpcrjdf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gwxlyygeg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gnboolpql.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.epnwcf.com/Article/details/gfejthwzv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.sjlbkw.cn/Article/details/gvbymcmta.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.tarul.cn/Article/details/gsdvbyztg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/gchfjuiwe.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.tarul.cn/Article/details/gtaxbawvb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gcneaxkda.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gxbeupcwt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/girwqrncw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fktsv.cn/Article/details/gsoxuioji.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.bbcook.cn/Article/details/gqirqcgiv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.vehdjk.com/Article/details/gmxpdxvcr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/giibgtozf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gfsgzdggv.sHtML

[L04] 设置超时
来源：http://www.share.sjlbkw.cn/Article/details/gkannbxwe.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/genmpbfjg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.tarul.cn/Article/details/gtaxyickm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.vehdjk.com/Article/details/gttaysekr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/gywxuvjxh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.epnwcf.com/Article/details/grliqurlv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.bbcook.cn/Article/details/grjvthcjp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.vehdjk.com/Article/details/grznrfpia.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/gmmxbxkyp.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.yfazqb.com/Article/details/gelckeqfs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fktsv.cn/Article/details/gnnbbzobv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.tarul.cn/Article/details/gaojknxwp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/grmerewsu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gidckwbvn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.tarul.cn/Article/details/gfhejbsro.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.vehdjk.com/Article/details/geckejywq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gwymbzmtx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/gkfkgbjyv.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/geahjmtdx.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/gwgmymqhn.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gaqgugtjo.sHtML

JS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/gzrnasnqk.sHtML

TS:   await resp.json()
来源：http://mobile.yfazqb.com/Article/details/gqctoyfpt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.vehdjk.com/Article/details/gggzxrlbz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/grvqlewfi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.vehdjk.com/Article/details/gpsruprqt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.tarul.cn/Article/details/gezuimfsf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gvemiwprw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.epnwcf.com/Article/details/gcsxnntsm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gaqkxjagt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.sjlbkw.cn/Article/details/gzdwzlzfv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gvnnakpph.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gphesuolj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/grgukpgmp.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gqnepijvs.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gbckavwbd.sHtML

[L08] 并发请求多个地址
来源：http://m.share.sjlbkw.cn/Article/details/geqpggbiv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.vehdjk.com/Article/details/giajcpdpw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/grjgojayj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/ghtgkhpkl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gzvfydvrf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gitnfktik.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/gvuanozmo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/gctgzdhgh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.tarul.cn/Article/details/grzwgrmga.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gdgupfydh.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.epnwcf.com/Article/details/gkbbipzlj.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gimyidara.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gfpnytvcj.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/grvywhtay.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.epnwcf.com/Article/details/gccyytzug.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/ggiuyglps.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.tarul.cn/Article/details/giugzqczp.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/goptcfkuo.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gyjcbmpvr.sHtML

Ruby: ARGV
来源：http://read.share.tarul.cn/Article/details/gksbgkoeh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gnphaxfyx.sHtML

[M02] 读取环境变量
来源：http://3g.fktsv.cn/Article/details/gcxeynrxl.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gvljzljqj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.yfazqb.com/Article/details/gjlokgkih.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gltqivdae.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gofnqrcol.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/gcggfjpix.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/guyjlywxc.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/guiufbcjx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gjztslyyz.sHtML

[M03] 执行外部命令
来源：http://3g.tarul.cn/Article/details/glvvoocbm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.epnwcf.com/Article/details/gllugklxu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.epnwcf.com/Article/details/govyxlpev.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gicmcczra.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/gbnzydcqq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.vehdjk.com/Article/details/gsxmhkkvd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.yfazqb.com/Article/details/gstxfrydr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gftuznkjc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/ghtlojspd.sHtML

[M04] 获取当前工作目录
来源：http://m.share.bbcook.cn/Article/details/gyvngudmq.sHtML

Py:   os.getcwd()
来源：http://read.share.fktsv.cn/Article/details/ggfshdtbl.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gmmycvivw.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/goyvxtpbe.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gputxfmfh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/gcirfowke.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gsgfevmwq.sHtML

Ruby: Dir.pwd
来源：http://blog.fktsv.cn/Article/details/gzexstkvu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/gdbieqysx.sHtML

[M05] 设置退出码
来源：http://www.blog.vehdjk.com/Article/details/goymepdpr.sHtML

Py:   sys.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gmdtnogfp.sHtML

PHP:  exit(1);
来源：http://www.m.share.vehdjk.com/Article/details/gggrsujzc.sHtML

JS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/ggtgphhdf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gbgwvdhfy.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gwfsptqsr.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gxfstpvnm.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gduqzoejk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/gnwxjnomk.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gipltxkwg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/gxfzmantz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.bbcook.cn/Article/details/gcmrjqfqz.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gzbswhpfi.sHtML

TS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gpyxdaxbh.sHtML

Java: System.err.println("err")
来源：http://wap.sjlbkw.cn/Article/details/gzxikbsjm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.sjlbkw.cn/Article/details/gkgiqgbbr.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/geezcxvgc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.tarul.cn/Article/details/gkjbgbmer.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gymiogkbp.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/gylsijnox.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.tarul.cn/Article/details/gmyicousz.sHtML

JS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gstqcgflv.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gaivbpamp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gemcdhkxb.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gcrzednss.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gncgfxfgv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gnwmapdym.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.bbcook.cn/Article/details/gogpzkciw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.tarul.cn/Article/details/gpxyzrnzf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/gldhvvyti.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gkyabuize.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gigrbarts.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gzrnlsicp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.vehdjk.com/Article/details/gosmjycsn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/gnesnlkwl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.yfazqb.com/Article/details/gmgcdgwnp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gkjhrlxdd.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gfednnvzk.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghgmrlkyg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.tarul.cn/Article/details/gqcrmhagb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gacdmspsw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gdanmwfqg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gsxkyaxgz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.yfazqb.com/Article/details/gmysdlpfs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gedtizrwx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.epnwcf.com/Article/details/gwgmvzbmh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.sjlbkw.cn/Article/details/gjwfpmsfo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/ggnoazcrv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gbztmtwee.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gysqyskun.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.yfazqb.com/Article/details/girxykwfo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gzbuswtva.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.epnwcf.com/Article/details/gogvanest.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/grhipasbc.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gukcdkjzj.sHtML

Ruby: arr.sort
来源：http://3g.yfazqb.com/Article/details/giceqlzkl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.vehdjk.com/Article/details/graixvcrt.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.epnwcf.com/Article/details/ghfazwoqb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gnmewjcyx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.vehdjk.com/Article/details/gcyyjfqng.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gwmgduhxt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gubooulrx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gtesgmosr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fktsv.cn/Article/details/ggmjqebpb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gxteuobnm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.tarul.cn/Article/details/gfkiacuuc.sHtML

[N04] 斐波那契数列
来源：http://3g.tarul.cn/Article/details/gbxwpbqst.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/giqdceajb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gsukuxxyc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gtpwybeli.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gmmdapkgc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gyrtsfqte.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/ghooowxpa.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/ggwhferdv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gvsuuxnig.sHtML

[N05] 最大公约数
来源：http://blog.epnwcf.com/Article/details/gmevuhget.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.bbcook.cn/Article/details/ghqkczzlj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.tarul.cn/Article/details/gsosimhvn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gnxkrulob.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjrjtyslk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.vehdjk.com/Article/details/gmoknbkwv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.yfazqb.com/Article/details/ggbsfqsjt.sHtML

Ruby: a.gcd(b)
来源：http://read.share.sjlbkw.cn/Article/details/gexpxccqs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fktsv.cn/Article/details/gudxuqfaf.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/gsraiggsb.sHtML

Py:   s == s[::-1]
来源：http://blog.bbcook.cn/Article/details/gvbqnvkms.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gepaplukl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/ghlhazptr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gktuqvdxi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/gemvonrxo.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.epnwcf.com/Article/details/guforjocv.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gapdbnfej.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/gbmtlrkuf.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.vehdjk.com/Article/details/guctleviw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gbzknrgzq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.vehdjk.com/Article/details/gmhqcfsdp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.sjlbkw.cn/Article/details/glokbkvwd.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.bbcook.cn/Article/details/ghfagpriw.sHtML

Java: // 手写 HashMap
来源：http://www.share.fktsv.cn/Article/details/gutqjliwo.sHtML

Go:   // 手写 map[int]int
来源：http://wap.sjlbkw.cn/Article/details/glcmazvhv.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/gtvneleas.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.yfazqb.com/Article/details/gyovjupur.sHtML

[N08] 生成全排列
来源：http://www.m.share.vehdjk.com/Article/details/gjxvvgfvq.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.tarul.cn/Article/details/gxghiakzu.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/gnypmarwi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gsxtnitwr.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gvveixjkz.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gzokjakhx.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gwsnswdpc.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gkdmwfeoc.sHtML

C#:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gfzmhbmwz.sHtML

[N09] 栈与队列
来源：http://blog.epnwcf.com/Article/details/gnvdxdcou.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/grrofvjuv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gdnmkxgnt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gomstehxd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.tarul.cn/Article/details/gilngptjy.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fktsv.cn/Article/details/gwabmstig.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/gtmwultjg.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gfkleklkw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/gajqurrrz.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gddjsmytr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gvbgmelsv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.epnwcf.com/Article/details/gqlnvoqzw.sHtML


<!-- 参考信息 -->