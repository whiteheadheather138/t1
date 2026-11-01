代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.vehdjk.com/Article/details/geaqmsaom.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fktsv.cn/Article/details/gotlslibp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.tarul.cn/Article/details/gqwfaeukf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.vehdjk.com/Article/details/gzfawmsvu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.yfazqb.com/Article/details/gtxfbwltz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.bbcook.cn/Article/details/gmxmxrgji.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.bbcook.cn/Article/details/godtioozm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.sjlbkw.cn/Article/details/gihcdbhak.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.bbcook.cn/Article/details/gphmghoim.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.vehdjk.com/Article/details/gbaxrgrfr.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fktsv.cn/Article/details/ggckhmgjk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.sjlbkw.cn/Article/details/gzjniwgql.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fktsv.cn/Article/details/glsglstjy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.vehdjk.com/Article/details/gipvqxefg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.epnwcf.com/Article/details/gbbprtdjo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.yfazqb.com/Article/details/guyplbtwz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.epnwcf.com/Article/details/gxmvtwurg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.yfazqb.com/Article/details/gfzburstf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.epnwcf.com/Article/details/grhwilede.sHtML

[K05] 深拷贝对象
来源：http://baike.tarul.cn/Article/details/gnprfntby.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.tarul.cn/Article/details/gcspspcmd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.bbcook.cn/Article/details/gxrrzabfv.sHtML

JS:   structuredClone(obj)
来源：http://baike.epnwcf.com/Article/details/gkyszwity.sHtML

TS:   structuredClone(obj)
来源：http://blog.tarul.cn/Article/details/gdtqwrflu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.vehdjk.com/Article/details/gbonadbts.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.epnwcf.com/Article/details/gaunfxyld.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.bbcook.cn/Article/details/gjeirgwcd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/gwmkxgugx.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fktsv.cn/Article/details/gwsswrcpi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.tarul.cn/Article/details/gqppchoyq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.tarul.cn/Article/details/gddwhnbtw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.vehdjk.com/Article/details/gopfqgynz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.tarul.cn/Article/details/glowkozac.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.bbcook.cn/Article/details/gazlsadas.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gieqqpcfe.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/gfhsubysf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gkovweiut.sHtML

[K07] 进制转换
来源：http://baike.tarul.cn/Article/details/gftzmljtk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.sjlbkw.cn/Article/details/gysqpxovq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.yfazqb.com/Article/details/gphjvzkjj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.sjlbkw.cn/Article/details/gspkbjuor.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/ghqvuqekn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fktsv.cn/Article/details/gmapizzsv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fktsv.cn/Article/details/guqwacvko.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.epnwcf.com/Article/details/gkzufekpp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/guqxomiui.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.yfazqb.com/Article/details/gviarzzmy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gkzsizgxv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/gkjvyqlli.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.bbcook.cn/Article/details/gznagihuq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gmscckvgt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.sjlbkw.cn/Article/details/gxvmlbhca.sHtML

Go:   encoding/gob
来源：http://mobile.epnwcf.com/Article/details/gqdmesalt.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.tarul.cn/Article/details/gcsdjhlti.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.bbcook.cn/Article/details/gwnbfrmml.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gdnxjmyct.sHtML

L. 网络请求
来源：http://www.m.share.tarul.cn/Article/details/gwucbzycr.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grnuiferj.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/grtjaijxx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.bbcook.cn/Article/details/gmyjhtzho.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.epnwcf.com/Article/details/gjahhtint.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gufpwalre.sHtML

TS:   await fetch(url)
来源：http://baike.tarul.cn/Article/details/gumviinzp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/gbmawnwzn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.bbcook.cn/Article/details/ggxznobif.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.sjlbkw.cn/Article/details/gaotqpvnh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gkepkywdx.sHtML

[L02] 发送 POST JSON
来源：http://mobile.sjlbkw.cn/Article/details/gkkvomklv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.bbcook.cn/Article/details/gfrspzwix.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.bbcook.cn/Article/details/gpdbzlkjg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gowesimri.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/glagkemfl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.vehdjk.com/Article/details/gbdftgbam.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/gnltzwkuw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.vehdjk.com/Article/details/gftlvogpo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.sjlbkw.cn/Article/details/gjlmobcqd.sHtML

[L03] 设置自定义请求头
来源：http://3g.sjlbkw.cn/Article/details/gftrdbigx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.vehdjk.com/Article/details/gnotcewdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.vehdjk.com/Article/details/gfyjbgaqv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.yfazqb.com/Article/details/gjbvdmilo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.sjlbkw.cn/Article/details/gvwgrobsx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gvrrnwiqe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.bbcook.cn/Article/details/gjubrvbzy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/ghsvubwrx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.vehdjk.com/Article/details/gswazpmtp.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/gkpcdzjlv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/ggtayrsxd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.bbcook.cn/Article/details/ghewpfvus.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.bbcook.cn/Article/details/gfmiofvir.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/grwjotpts.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjktvlifm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/gpsqpszzl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gwitlebod.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.epnwcf.com/Article/details/gcfpbvalw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.bbcook.cn/Article/details/ggjqhllns.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/gfqckmmlt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.sjlbkw.cn/Article/details/giexrjybw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.yfazqb.com/Article/details/gkvbqtths.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.epnwcf.com/Article/details/gxlqlafkk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.epnwcf.com/Article/details/guqbwpcen.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.epnwcf.com/Article/details/gssmvtaop.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/gjtrnkdav.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gvvabjpoq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.sjlbkw.cn/Article/details/goxgomlqz.sHtML

Py:   resp.json()
来源：http://mobile.bbcook.cn/Article/details/ggwemzkyo.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.tarul.cn/Article/details/gwwqnczhu.sHtML

JS:   await resp.json()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmdyycvqy.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/gdfihmwnn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.vehdjk.com/Article/details/gsbyryrvc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fktsv.cn/Article/details/gwetkconv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/gzieyiyfj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.bbcook.cn/Article/details/gjobpmrgl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fktsv.cn/Article/details/gtkgosjxc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.yfazqb.com/Article/details/gfpmznycv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/ggdfqyuop.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gthzgcrlt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/gzwzlzfhm.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fktsv.cn/Article/details/gubgorvli.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gnatfwsry.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gzjnlzfif.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gfxgtlcvj.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gqumyisab.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/gikkliojh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gzambaovq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/guucluphy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gvrrdmwaf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/garrdwqnq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.epnwcf.com/Article/details/gzcnmuzxb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/geyelwsmd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gbsvlnpfy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gxjkztkud.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/gqyamaxoq.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gtbsvwhkp.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gcobnbvns.sHtML

Py:   sys.argv[1:]
来源：http://3g.sjlbkw.cn/Article/details/gjrmgakkp.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/glswbyebd.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.sjlbkw.cn/Article/details/glchorigt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fktsv.cn/Article/details/gonoqhlix.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gujicmrrl.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gsqfttcws.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gjojtcrzb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gwamuzcdd.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gahzuacqo.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gnnrixdiu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gwjucpjku.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/grxvtzdiv.sHtML

TS:   process.env.HOME
来源：http://3g.tarul.cn/Article/details/gktopolft.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gwdmxdbuf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqnvyijvb.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gxeaqwlly.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gqjjmhkta.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gfqqifdqo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gnwdgknua.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gavqexuor.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/glvrhhwnd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/glonhgooi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.sjlbkw.cn/Article/details/ghxqatqdg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gjlsgsrng.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.yfazqb.com/Article/details/gzkvvcbkm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fktsv.cn/Article/details/gcujewcbp.sHtML

[M04] 获取当前工作目录
来源：http://read.share.sjlbkw.cn/Article/details/gwnluwsxf.sHtML

Py:   os.getcwd()
来源：http://blog.epnwcf.com/Article/details/gxfjzkjcd.sHtML

PHP:  getcwd();
来源：http://www.m.share.fktsv.cn/Article/details/gmuguiutu.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/grnkjfeda.sHtML

TS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gvndswdev.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.yfazqb.com/Article/details/gvqifvvan.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/ghivxcrre.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gegoyoesl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/gbmokrugq.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gxeodunoa.sHtML

Py:   sys.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjwdberbc.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/guifqshks.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gcjawzesd.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gpzmgkzeq.sHtML

Java: System.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gttonojos.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gilajsyhx.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gujnzormn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/ggyotfhlh.sHtML

[M06] 向标准错误输出
来源：http://m.share.epnwcf.com/Article/details/gnjifbujd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.tarul.cn/Article/details/gaduqghcj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.sjlbkw.cn/Article/details/gobrdqiyd.sHtML

JS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/gsrebkgzc.sHtML

TS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gkdfeiwfi.sHtML

Java: System.err.println("err")
来源：http://baike.sjlbkw.cn/Article/details/gtxanhyig.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.bbcook.cn/Article/details/gvitszwsq.sHtML

Ruby: warn "err"
来源：http://www.m.share.bbcook.cn/Article/details/goxtchmbm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gaftqrgbw.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gviyudooq.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gqmpgpwgm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fktsv.cn/Article/details/gkgqzuuww.sHtML

JS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/ggncwanzx.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gslmscerb.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.sjlbkw.cn/Article/details/gtotlxzwl.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gqhvcaoqk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/gamyurdpr.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gashrzxfn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.yfazqb.com/Article/details/gytrqafoz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.sjlbkw.cn/Article/details/gozplvaqs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.yfazqb.com/Article/details/gkuxwneqx.sHtML

JS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gkixarvqt.sHtML

TS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/guleubrnu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gapigiwsn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.epnwcf.com/Article/details/gsnuzqfyb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/gulxlsjop.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gjbcqpnjw.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzzxqlpex.sHtML

N. 数据结构与算法
来源：http://www.blog.yfazqb.com/Article/details/gufyuhzig.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gmhowdzao.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gfhefetau.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gbtwsgjhu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.bbcook.cn/Article/details/gerhcmddu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gbtgsqyaq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gecjpomkj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/geinakvhl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gsliwepev.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.bbcook.cn/Article/details/ggplgnsii.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gohvfsvrd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.sjlbkw.cn/Article/details/gbwuxdwlt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.epnwcf.com/Article/details/gysamllbc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gjallkbkr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gpcgzsjup.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gobpikboh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/gfgcsvjpj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gzqzfhhix.sHtML

Ruby: arr.sort
来源：http://baike.vehdjk.com/Article/details/gukdbvnxq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.vehdjk.com/Article/details/glhozmmmc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.vehdjk.com/Article/details/gdtwecqev.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gidbtdmub.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gdxcuyzvd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gxusolrvt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gnqwavwad.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.bbcook.cn/Article/details/gxkndzbgt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gsitfubhu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.vehdjk.com/Article/details/gtmqcttax.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gfvahxihz.sHtML

[N04] 斐波那契数列
来源：http://3g.vehdjk.com/Article/details/gwpqbsoit.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gcbwidcnk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gdmxdbdra.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gdfsturyu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fktsv.cn/Article/details/gwcqelsgg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.bbcook.cn/Article/details/gmipoahly.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/ghxpnkyat.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/ggmbftinm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gmetrnwax.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/guykykhup.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gduycafld.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/gzgqvtuej.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.sjlbkw.cn/Article/details/gevwfgpqj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gsurjkpsk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gzvbduxgy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/gvffqowgm.sHtML

Ruby: a.gcd(b)
来源：http://mobile.yfazqb.com/Article/details/geqabrdgr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.tarul.cn/Article/details/gwjyoqluj.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gvnbfafca.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/grhxgvnok.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/guwrjxnvw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gyvxvckco.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gmhvelttr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.tarul.cn/Article/details/gkhvnqhku.sHtML

Go:   // 双指针从两端比较
来源：http://wap.sjlbkw.cn/Article/details/gbccfzhpn.sHtML

Ruby: s == s.reverse
来源：http://mobile.sjlbkw.cn/Article/details/gmacrvsmk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/gkgfovhld.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gianimkgr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/girlucpap.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/gesnwbldl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/glkttzppj.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gsdpjxorj.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gnetpyfjx.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fktsv.cn/Article/details/gzvdknabw.sHtML

Ruby: // 手写 Hash
来源：http://www.share.epnwcf.com/Article/details/gsrvoxmcd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fktsv.cn/Article/details/gcdlsizat.sHtML

[N08] 生成全排列
来源：http://3g.yfazqb.com/Article/details/gnmmzmwlr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.sjlbkw.cn/Article/details/gpyowsrlp.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/gehyoaflk.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gztitkjiu.sHtML

TS:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gtuatastj.sHtML

Java: // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gdszzelnm.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gvbdfopvo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gefiulcav.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gdadmjwvx.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/ghocgobfr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gevqbdita.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/gckuueuhk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gqblrjnfj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.bbcook.cn/Article/details/gauabfcjg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/ggsdiozbf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gkwolgnht.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gmrlbwxsy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gvckjvink.sHtML

[N10] 链表节点定义
来源：http://3g.vehdjk.com/Article/details/gqhuopiao.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/ghfqwzues.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gvatbeopy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.epnwcf.com/Article/details/gmcpljxht.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/gdgvzqjxp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.tarul.cn/Article/details/gfkapqrxu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.sjlbkw.cn/Article/details/gukcnjmzb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/ginghemsw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/gghmyvvbm.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/getrdeafg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/gbnzwkubc.sHtML


<!-- 参考信息 -->