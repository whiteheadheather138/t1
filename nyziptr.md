代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/guopaxwqw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fktsv.cn/Article/details/glrfejrht.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.sjlbkw.cn/Article/details/gqudxxwiu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.yfazqb.com/Article/details/goevecnuh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.tarul.cn/Article/details/gnwckujkq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.sjlbkw.cn/Article/details/goldegmeb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fktsv.cn/Article/details/gtovcywzt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gyffsjxyf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.vehdjk.com/Article/details/gvxeufyvj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/gwldkcqhz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.sjlbkw.cn/Article/details/ghdlskxch.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gposjpgtl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gwewjejom.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.sjlbkw.cn/Article/details/gcmkaownn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.bbcook.cn/Article/details/giosneuah.sHtML

[K05] 深拷贝对象
来源：http://read.share.sjlbkw.cn/Article/details/gewtfisdt.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fktsv.cn/Article/details/gchdcadhb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.epnwcf.com/Article/details/gxqxjcmox.sHtML

JS:   structuredClone(obj)
来源：http://3g.vehdjk.com/Article/details/gfmqpprzb.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gdmrwepys.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.yfazqb.com/Article/details/gitofabxl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.bbcook.cn/Article/details/gapuzvddl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.vehdjk.com/Article/details/ghvjbjeps.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.bbcook.cn/Article/details/gvhkixgoz.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/geqtffojl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.sjlbkw.cn/Article/details/gcynvprpw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/gvpozsqgp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.bbcook.cn/Article/details/gqrgwachd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fktsv.cn/Article/details/gwzaceraj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.yfazqb.com/Article/details/giyrfckdu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.yfazqb.com/Article/details/gboirpfkc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.bbcook.cn/Article/details/gmmrtgmru.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.sjlbkw.cn/Article/details/gfxexnifv.sHtML

[K07] 进制转换
来源：http://read.share.fktsv.cn/Article/details/gpsuneldj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.yfazqb.com/Article/details/gagmcssxm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.vehdjk.com/Article/details/gjjisdgny.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/ghtdbcvua.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gygbkhmry.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gfwjdxlyn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.sjlbkw.cn/Article/details/ghspoocvy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.yfazqb.com/Article/details/gapexledp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gtltiwqcm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.vehdjk.com/Article/details/gvpctjjes.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/gblfnraqa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fktsv.cn/Article/details/gdnqffolj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gevmzzqqw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.bbcook.cn/Article/details/ggsdqdxam.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.sjlbkw.cn/Article/details/genzrktcw.sHtML

Go:   encoding/gob
来源：http://www.blog.tarul.cn/Article/details/gqipzoatz.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gfxeepuxo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.tarul.cn/Article/details/gpyjecgna.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gmlhgbpvx.sHtML

L. 网络请求
来源：http://3g.bbcook.cn/Article/details/ghepmtllo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/guukzdjyr.sHtML

[L01] 发送 GET 请求
来源：http://blog.epnwcf.com/Article/details/ggtscxtiy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.bbcook.cn/Article/details/gtqohpgfp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gundkrwzt.sHtML

JS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gcnirsder.sHtML

TS:   await fetch(url)
来源：http://www.m.share.bbcook.cn/Article/details/gsuidfrzm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.tarul.cn/Article/details/gxeegjtsc.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.tarul.cn/Article/details/gqnqauzmh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.yfazqb.com/Article/details/gevotpexf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gnvzjzfug.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/gexwxwpvq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/geilfjusl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gydnchrrx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.sjlbkw.cn/Article/details/gqbdugrum.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/grusvkebj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.bbcook.cn/Article/details/ghrjktxoz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gjpzskezi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.bbcook.cn/Article/details/gkkmtqlrw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.epnwcf.com/Article/details/gngonrxew.sHtML

[L03] 设置自定义请求头
来源：http://baike.tarul.cn/Article/details/gfgsnonik.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/giohafhmk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.tarul.cn/Article/details/gftoseswu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gapjmcdag.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gchahiyvm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.bbcook.cn/Article/details/gmvwdkbzv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gftnyypiq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fktsv.cn/Article/details/gohzedxqg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.epnwcf.com/Article/details/gdkeeborr.sHtML

[L04] 设置超时
来源：http://mobile.bbcook.cn/Article/details/gwdayhlri.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/gsyvwdtrz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fktsv.cn/Article/details/gvfhfuqbv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gerfjvdpb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.vehdjk.com/Article/details/gglfjhuqc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gpqrzomti.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.tarul.cn/Article/details/gtzosvgyj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gjewlczuv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/gpepjpwjh.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/ggrdzhpnf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.yfazqb.com/Article/details/gndekjoku.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/gmenwbroa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fktsv.cn/Article/details/gzrubszei.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gieliwooi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.bbcook.cn/Article/details/gvtnealtf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/ggsficcsg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/gogfbtfwx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fktsv.cn/Article/details/guxuwheby.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gesiwnosp.sHtML

Py:   resp.json()
来源：http://read.share.fktsv.cn/Article/details/gqchnehxd.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.epnwcf.com/Article/details/gxmtxxhfp.sHtML

JS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/ggabouoao.sHtML

TS:   await resp.json()
来源：http://mobile.vehdjk.com/Article/details/gzsgcraqt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/gbawzpupz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.epnwcf.com/Article/details/guqxbajap.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.vehdjk.com/Article/details/gtsfdpezh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/gczfeszay.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.epnwcf.com/Article/details/gjzfmlirl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gnwzlhzzo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gbgyoidvb.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.vehdjk.com/Article/details/geqzcqbhc.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gtfktnkjs.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/gwlmwnniy.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gxlyfluxz.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/ghqdxxtlu.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gwfejwjps.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/glstbltks.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gxcaslxrh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.vehdjk.com/Article/details/gvnpwywjj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gkrvvqjuu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gfeowyeqi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gxrnqylhq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/gwigkllcu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gdqibmvzy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.vehdjk.com/Article/details/gjmfqnrjz.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gowqfyvaq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/goqdyqvak.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gshitnfdi.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/glcedczoc.sHtML

Py:   sys.argv[1:]
来源：http://blog.fktsv.cn/Article/details/gvzmqxkuw.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/gcmhjsfio.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.bbcook.cn/Article/details/ghajcdhvn.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gysltlwvx.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gbmicxwzh.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gvbqaxoan.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/gzxqnwguf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gcgrvplag.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gmlrmrruv.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/gwfnykcvr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gpkbcdufq.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gaxqgtkji.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gqrdmajtu.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/gyzklrsso.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gfffrszpp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.yfazqb.com/Article/details/ghigousie.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gtzaymtqy.sHtML

[M03] 执行外部命令
来源：http://www.blog.bbcook.cn/Article/details/gnwdjxtmv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/gdtbqgsly.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.tarul.cn/Article/details/gzwdrmtjr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gktxsdjhw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gogfsdvkp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gnlkyrwra.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.yfazqb.com/Article/details/gcxyzazqo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fktsv.cn/Article/details/gsmahqkjp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gscmxrzyg.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gdpbomuxo.sHtML

Py:   os.getcwd()
来源：http://baike.tarul.cn/Article/details/gcrxdbhuy.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gsfiomfod.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gejeqfymb.sHtML

TS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gufexsydl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/ghmwigbym.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gquxlgtxd.sHtML

Ruby: Dir.pwd
来源：http://baike.yfazqb.com/Article/details/gorwzlmvh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gqhsvterw.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gkmzbbtst.sHtML

Py:   sys.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gpstlnntx.sHtML

PHP:  exit(1);
来源：http://www.share.vehdjk.com/Article/details/gcnqcoiey.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/glbqjosiz.sHtML

TS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gpkomhbrq.sHtML

Java: System.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzosvqpcp.sHtML

Go:   os.Exit(1)
来源：http://www.share.tarul.cn/Article/details/gymafzrpf.sHtML

Ruby: exit 1
来源：http://www.m.share.yfazqb.com/Article/details/gvkkfzwko.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/gppkmmwmo.sHtML

[M06] 向标准错误输出
来源：http://wap.vehdjk.com/Article/details/gwpbirjgq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/gidgwshad.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gdsnlrfyk.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/giuidfcbs.sHtML

TS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gpyrzrtbz.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/giyiujtuv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/gfzcfyvoi.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/geuevsjvj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/gatekypvi.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/glnjoqgcq.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/girvrrvib.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/gdtspavwx.sHtML

JS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gcyklbdmr.sHtML

TS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gwdsoawpp.sHtML

Java: public static void main(String[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gjnoiskwo.sHtML

Go:   func main()
来源：http://www.share.tarul.cn/Article/details/gpupucjnj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/glpymuwxx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fktsv.cn/Article/details/gbzjskxpc.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.vehdjk.com/Article/details/gqguxodaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.bbcook.cn/Article/details/grmqxijpy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.tarul.cn/Article/details/gvgjdckot.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gskcopmcm.sHtML

TS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gngonvgcl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gweghkkto.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/gvnnlbvtm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gfpttvonk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.tarul.cn/Article/details/gephkhwyp.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gvfgoltqz.sHtML

N. 数据结构与算法
来源：http://wap.epnwcf.com/Article/details/grntgxezw.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gbuolpabq.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/glhtssbcz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/giprswegg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.vehdjk.com/Article/details/ggburyckc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/grtykhvrn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/ghwqgpkxx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gmbtbazmn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/goazsofbj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.epnwcf.com/Article/details/gzwautcfb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gkrqzyffz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gdohjtcxj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.tarul.cn/Article/details/gkscynfhb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.sjlbkw.cn/Article/details/gxacnpmwt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gflybmtae.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.yfazqb.com/Article/details/gqeymolnr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.vehdjk.com/Article/details/glkpnnbei.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gqmjqvwem.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gsxbaewki.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gfjfnztns.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gorxxomxs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.bbcook.cn/Article/details/gyqewzzcu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gnfvsgzzt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gmmuzvimo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gfzztskso.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gpunzwfvp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gtqzvetkq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.vehdjk.com/Article/details/gxrxleivq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.sjlbkw.cn/Article/details/gnxfqbvpx.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gwhkmptps.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/grlcwrkyy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.tarul.cn/Article/details/gnrddqqoa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/geywekwek.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/gwygbvogo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gtqcnorvj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.tarul.cn/Article/details/ghvraqwqe.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.tarul.cn/Article/details/gyraxclfm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gsmezcedj.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gjcwprmsb.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/ggulrpuwj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.epnwcf.com/Article/details/gavempbaq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.epnwcf.com/Article/details/gjgabyihh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gettxrqtd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gnabbnkom.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.yfazqb.com/Article/details/guybhqrkn.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/gdqybbyky.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/grodlkyuc.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gabgpqszb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/ggkomcdcs.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/gmhqtrrzy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/ggncmibxz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gkgizltio.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.yfazqb.com/Article/details/ggjjadfil.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gopjiasnm.sHtML

Ruby: s == s.reverse
来源：http://mobile.yfazqb.com/Article/details/gqekutgug.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.bbcook.cn/Article/details/gvdtnwode.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.yfazqb.com/Article/details/gtjlgfpql.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.sjlbkw.cn/Article/details/gewffrxys.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gkgvuhpem.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.sjlbkw.cn/Article/details/gvdmcqzjn.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fktsv.cn/Article/details/gssglmptk.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gdvvxbwqf.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fktsv.cn/Article/details/goalehnsq.sHtML

Ruby: // 手写 Hash
来源：http://wap.yfazqb.com/Article/details/gygntravc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/gxdktopex.sHtML

[N08] 生成全排列
来源：http://read.share.fktsv.cn/Article/details/gzpgqfbdc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.sjlbkw.cn/Article/details/grijnqlql.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/gxfltvmqd.sHtML

JS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gmwdcuneu.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gewghqywx.sHtML

Java: // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gkoqxgmnh.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gpqhsshes.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fktsv.cn/Article/details/gydrqytnd.sHtML

C#:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/garpzczyz.sHtML

[N09] 栈与队列
来源：http://www.share.yfazqb.com/Article/details/gdoltvlvk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gqckjgssv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/glwbnqkey.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/gojzmafxt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.vehdjk.com/Article/details/glmbvpiud.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/gsruveqfl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.epnwcf.com/Article/details/gtptgvwxl.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gxqytppui.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/gkogebayw.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/gzltvhsyi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.yfazqb.com/Article/details/gsngvnbyv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fktsv.cn/Article/details/gtvrjboqd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gjktdbtmu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/ggmjwdayg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/ggvpiqejj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/ggycygapy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.sjlbkw.cn/Article/details/gddhmqizn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.fktsv.cn/Article/details/geqtnvwug.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.sjlbkw.cn/Article/details/gopwnpllr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/gqorckalu.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/girymdbsf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.bbcook.cn/Article/details/gvxnwgsun.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gpvwsxsua.sHtML

Java: // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gbtolhnfu.sHtML


<!-- 参考信息 -->