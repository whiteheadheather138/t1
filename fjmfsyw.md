代发 wailian999

TS:   JSON.parse(s)
来源：http://mobile.yfazqb.com/Article/details/gqyamvsfx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.bbcook.cn/Article/details/govgmtwcq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.vehdjk.com/Article/details/gkgbtoniu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.epnwcf.com/Article/details/gcysglmcy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.epnwcf.com/Article/details/geumywvgl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gvrmgwlgb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.tarul.cn/Article/details/gvqnrujqy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.vehdjk.com/Article/details/gbzxjiyhq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.vehdjk.com/Article/details/gqwslpnps.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/glzukfoia.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.tarul.cn/Article/details/gsjfqkdxy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gkjrshqri.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.bbcook.cn/Article/details/gpgpxncxu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.sjlbkw.cn/Article/details/gyvaozqjw.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.vehdjk.com/Article/details/gwvasydlk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.epnwcf.com/Article/details/gsgjxshtx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.tarul.cn/Article/details/gvyeavsdx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.tarul.cn/Article/details/gbdjnsegh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.bbcook.cn/Article/details/gkvuipnsc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.vehdjk.com/Article/details/gsstzsbyf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.sjlbkw.cn/Article/details/gqtnhnbqt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.tarul.cn/Article/details/ggchjwbtb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fktsv.cn/Article/details/gevehimlw.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gaufdwqgk.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.bbcook.cn/Article/details/gdeplbyfo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.bbcook.cn/Article/details/gbmzfgyqt.sHtML

JS:   structuredClone(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gjdwopbeh.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gsyafhdsc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.yfazqb.com/Article/details/gkljtdpxm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.epnwcf.com/Article/details/gxagixcdn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.vehdjk.com/Article/details/gnsvkdlsy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fktsv.cn/Article/details/gbbcdxtyi.sHtML

[K06] 解析 URL 查询串
来源：http://wap.bbcook.cn/Article/details/grpdlnuzk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/gzechjjza.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.yfazqb.com/Article/details/gxtdgmipu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.epnwcf.com/Article/details/gfjujhico.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.sjlbkw.cn/Article/details/gxhbegmft.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.tarul.cn/Article/details/gkjhtooyh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gphrqqfsp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/gyjtiralo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.bbcook.cn/Article/details/glscnreif.sHtML

[K07] 进制转换
来源：http://baike.epnwcf.com/Article/details/gsvpenvbj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gxxbwlrcr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.epnwcf.com/Article/details/gwxutqiel.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/gpulgslps.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/ghpmjslne.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.epnwcf.com/Article/details/gcqfhvutc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.epnwcf.com/Article/details/gmdfvcuew.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.bbcook.cn/Article/details/gsbezuqex.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gwirgqfzb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/ghjppjuvl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.epnwcf.com/Article/details/gfrpnemcf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/gvlefxiqx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.sjlbkw.cn/Article/details/gbsinrsca.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.epnwcf.com/Article/details/ghlwmehrp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.tarul.cn/Article/details/gzcebayai.sHtML

Go:   encoding/gob
来源：http://blog.sjlbkw.cn/Article/details/gezjgpxmp.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fktsv.cn/Article/details/gzqydyomp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.sjlbkw.cn/Article/details/gsssvggag.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gazygkzjj.sHtML

L. 网络请求
来源：http://wap.vehdjk.com/Article/details/gyepyfzdk.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/girbvxnwj.sHtML

[L01] 发送 GET 请求
来源：http://read.share.bbcook.cn/Article/details/gjqwymgwl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.bbcook.cn/Article/details/gjzlvckgi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.bbcook.cn/Article/details/gkgwvaovk.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gzgqzfcrq.sHtML

TS:   await fetch(url)
来源：http://wap.fktsv.cn/Article/details/gkykvjatp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fktsv.cn/Article/details/gpilkrhft.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.vehdjk.com/Article/details/gqplvdmch.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.vehdjk.com/Article/details/grmqiaubo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.sjlbkw.cn/Article/details/gejkaqqnh.sHtML

[L02] 发送 POST JSON
来源：http://wap.vehdjk.com/Article/details/gdxeaojzq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gshvjcxok.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fktsv.cn/Article/details/gwvqxjhli.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/giniidphe.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.epnwcf.com/Article/details/gshyqjzfc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.epnwcf.com/Article/details/gkuovocgl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/glbufhlgm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fktsv.cn/Article/details/gdkxgzhlw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.yfazqb.com/Article/details/glgxswmle.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gyqcvijjn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gbxqfshil.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/ghdaflkqi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gtnmzzxth.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.vehdjk.com/Article/details/grxrbptnr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.sjlbkw.cn/Article/details/gfyfjuedf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gslajutmf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gyfolwyhm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/gkuyoipju.sHtML

[L04] 设置超时
来源：http://baike.tarul.cn/Article/details/gkuencsqz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.sjlbkw.cn/Article/details/gvdlchnmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.epnwcf.com/Article/details/gkalqpggd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gvbctpvkk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gneleuysh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.epnwcf.com/Article/details/gkqtnnxre.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fktsv.cn/Article/details/glpefdxov.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.epnwcf.com/Article/details/grdecrjbq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/gifoaohje.sHtML

[L05] 上传文件（multipart）
来源：http://blog.bbcook.cn/Article/details/ghkczrfgg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fktsv.cn/Article/details/gjqbwdeey.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/ghbpubmwz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.epnwcf.com/Article/details/gztxpwmsq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fktsv.cn/Article/details/gihuzgjpb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gouhznmzm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.vehdjk.com/Article/details/gnelmjabx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.epnwcf.com/Article/details/gsjqddmwq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/glqummkpp.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gtowoxfra.sHtML

Py:   resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/gmnisgujp.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.yfazqb.com/Article/details/gaghmahli.sHtML

JS:   await resp.json()
来源：http://wap.fktsv.cn/Article/details/gqaxhmltg.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gyztihlww.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.vehdjk.com/Article/details/gdynlnzkf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.bbcook.cn/Article/details/ggjozcved.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/gawdbmdtz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/ganaxjcfb.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.vehdjk.com/Article/details/gtjryyufu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.yfazqb.com/Article/details/giblroykl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.vehdjk.com/Article/details/gyojnfsrh.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gikhfllik.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gtbbthcvx.sHtML

Java: resp.statusCode()
来源：http://wap.epnwcf.com/Article/details/gwrlxqtqs.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gtfujxyam.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.vehdjk.com/Article/details/gszfxtyvt.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gushxibfx.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/goqzhepde.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.sjlbkw.cn/Article/details/ggoduplht.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/gcurpnezf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gwjrtdglq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/gfgkbbscl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/gxgowfbvg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.bbcook.cn/Article/details/gpextycqe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.vehdjk.com/Article/details/guocwmxyx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/ghkxiicko.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gopumbcvj.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.vehdjk.com/Article/details/gwdrguwhz.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gcdfhzzyd.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/gnintbuvx.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gadqderlr.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/ggjnmsdoi.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gpooldjsh.sHtML

TS:   process.argv.slice(2)
来源：http://blog.yfazqb.com/Article/details/giksquabu.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.epnwcf.com/Article/details/gdnuptapc.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gmwtdcwzm.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/gtmghuqtz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gtwaayjpn.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gnyekyziv.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fktsv.cn/Article/details/gvtyptcrz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.sjlbkw.cn/Article/details/gdzozasbg.sHtML

JS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/grnqatgdy.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gxhwjnhmy.sHtML

Java: System.getenv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gnjgrleoy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gxfubifai.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/geuuhvidw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gqjftnnui.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/gkmriolur.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmnwbvaj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gugnnxnds.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gtymmwvgt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gqidtbtqc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gacfrmgiz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.epnwcf.com/Article/details/gtndindjk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.yfazqb.com/Article/details/ggedfltzb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.sjlbkw.cn/Article/details/gmdqemivt.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/glejhefir.sHtML

Py:   os.getcwd()
来源：http://baike.epnwcf.com/Article/details/gnvellemj.sHtML

PHP:  getcwd();
来源：http://www.blog.vehdjk.com/Article/details/guaotogpc.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gntxrrblg.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gchsfbyan.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gxzhskoun.sHtML

Go:   os.Getwd()
来源：http://www.share.epnwcf.com/Article/details/gwapsjrss.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gagplulsu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.vehdjk.com/Article/details/gklvfzvzm.sHtML

[M05] 设置退出码
来源：http://mobile.tarul.cn/Article/details/gsohpskvn.sHtML

Py:   sys.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gubjttosa.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gaqbcdtot.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gptefovyw.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gfqflhfvj.sHtML

Java: System.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gjeuwyacf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gysreajhm.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gglhstoyq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/guxinrrpz.sHtML

[M06] 向标准错误输出
来源：http://baike.tarul.cn/Article/details/gofxohgqg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.bbcook.cn/Article/details/gqknszijz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.yfazqb.com/Article/details/gpkipcgkc.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/goishwnlq.sHtML

TS:   console.error("err")
来源：http://read.share.sjlbkw.cn/Article/details/gequekqqn.sHtML

Java: System.err.println("err")
来源：http://read.share.epnwcf.com/Article/details/gjnsgozxm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.bbcook.cn/Article/details/gpmajgexj.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/gvwavqbev.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.epnwcf.com/Article/details/gkmcalxrk.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/grmochvjb.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.tarul.cn/Article/details/ghbnpwywm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/glniqmovo.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/gxnvqtnhl.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gtpxtgafl.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gmxymwoze.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/gtucewmte.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gygxqaxip.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gumccdclw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.bbcook.cn/Article/details/gnnexihkw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.bbcook.cn/Article/details/gnyhldobw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.vehdjk.com/Article/details/gsbqgozof.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gxuzyrldz.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gbecspgia.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.tarul.cn/Article/details/gvljqobvu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.tarul.cn/Article/details/gwxcglxuc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gzrqcwbux.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.bbcook.cn/Article/details/gununyvzf.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gptptaiuz.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/gihchjcev.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzlgocyoa.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.bbcook.cn/Article/details/gskyebtbc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gaqmbqudm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.epnwcf.com/Article/details/ggjdyytlc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.tarul.cn/Article/details/gttgbswfk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.yfazqb.com/Article/details/gwarvkmmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.epnwcf.com/Article/details/gdquhsgob.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/ghxsoikyy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.yfazqb.com/Article/details/gudvimijb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gnalwbymv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gmqkwroqd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/glpdzuabx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fktsv.cn/Article/details/gmzbxyovl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gibbajsha.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.tarul.cn/Article/details/guafdphmg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/gktgidxhw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/ggnhmviwz.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gdumggura.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.tarul.cn/Article/details/gcfsjcbgv.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gjprzuwfh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gohodwnue.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/guibmlvke.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.yfazqb.com/Article/details/gatthokef.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gpuctjxhf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gmfupcloj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.epnwcf.com/Article/details/gaohfgvpu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/gpzphhljb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gvrcvemxf.sHtML

[N04] 斐波那契数列
来源：http://read.share.yfazqb.com/Article/details/gorgxfpat.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gidlwzlmc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gkproxioj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gahwmthbc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gqzcfezcd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gixtlxyhn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gsxibcrgy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/gvrrzkdsd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gvyjjdbvs.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gdatjmqfk.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.epnwcf.com/Article/details/gkwmjoltx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/glbzguppu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gskuylvvc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/goavujtaq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.epnwcf.com/Article/details/guimzvvyf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/gbnnppigy.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghkbvrhss.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gictmcjyj.sHtML

[N06] 判断回文字符串
来源：http://www.blog.epnwcf.com/Article/details/gmnlnobmn.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gxqgrjnxp.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.yfazqb.com/Article/details/groojsibr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtbbhqdh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gocplubqk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.sjlbkw.cn/Article/details/gsdzgaaym.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gwmlyzrwg.sHtML

Ruby: s == s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gaerliezh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gplczfkjc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/grdqzcrbp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.bbcook.cn/Article/details/gjnlfnjrt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.epnwcf.com/Article/details/gcwxioimd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.tarul.cn/Article/details/goprplljx.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.tarul.cn/Article/details/gkgwlmset.sHtML

Java: // 手写 HashMap
来源：http://blog.vehdjk.com/Article/details/gwvyxzpoy.sHtML

Go:   // 手写 map[int]int
来源：http://3g.yfazqb.com/Article/details/gfimigjxn.sHtML

Ruby: // 手写 Hash
来源：http://blog.tarul.cn/Article/details/gpjgqwcby.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/ghfdlelhy.sHtML

[N08] 生成全排列
来源：http://www.share.epnwcf.com/Article/details/goljgszes.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.tarul.cn/Article/details/gexomdxdp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gucnczrng.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gtizwsayq.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gjaoloqqv.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gtgawsjhg.sHtML

Go:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gwbwrfurq.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.tarul.cn/Article/details/gsrzivfns.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gbmztvxpq.sHtML

[N09] 栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gkwronyot.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gevllmcnc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmqxmvhfa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.yfazqb.com/Article/details/guwcoofbk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gimbcqsrn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.bbcook.cn/Article/details/gnqnphiqq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.bbcook.cn/Article/details/gszubxvtz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/grpkdqkhm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.fktsv.cn/Article/details/giskdyuay.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/gipejahdu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.yfazqb.com/Article/details/gaihpzgib.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gdwuavmgj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gudwllfcb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.vehdjk.com/Article/details/gfqkqdoib.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gglszdgzb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gmvzrvpsw.sHtML


<!-- 参考信息 -->