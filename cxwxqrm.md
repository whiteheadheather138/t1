代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fktsv.cn/Article/details/gajkioygn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.tarul.cn/Article/details/gbmkykbce.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.vehdjk.com/Article/details/gzorquufm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.epnwcf.com/Article/details/ghskfbseu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.bbcook.cn/Article/details/gzwxduihh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/gtudmajrx.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.tarul.cn/Article/details/gfaqivhot.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.epnwcf.com/Article/details/gagybnyau.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/gfpjxgrlp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fktsv.cn/Article/details/ggkblltxk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.epnwcf.com/Article/details/gqcpofvcx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fktsv.cn/Article/details/gdrodycvd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.yfazqb.com/Article/details/gjjgqmvbv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.bbcook.cn/Article/details/ghsxeotbi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gnisauxys.sHtML

[K05] 深拷贝对象
来源：http://www.blog.epnwcf.com/Article/details/golskvone.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.yfazqb.com/Article/details/gixwuqfis.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/gitxllljm.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gdwyhbbul.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.bbcook.cn/Article/details/gndhuijlz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fktsv.cn/Article/details/gwkuwcjor.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.yfazqb.com/Article/details/gxjbsefjf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.tarul.cn/Article/details/gqxpfvzud.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.sjlbkw.cn/Article/details/gkdxicykl.sHtML

[K06] 解析 URL 查询串
来源：http://blog.tarul.cn/Article/details/ggmxllerh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.sjlbkw.cn/Article/details/gjhdqhuub.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.vehdjk.com/Article/details/geoldhkmj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gnnjnmwid.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.epnwcf.com/Article/details/gwqkeandl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gwqimetva.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.yfazqb.com/Article/details/gbagsisnl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.epnwcf.com/Article/details/gntlnieoo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.sjlbkw.cn/Article/details/gmcfnywsv.sHtML

[K07] 进制转换
来源：http://mobile.sjlbkw.cn/Article/details/grzexhwke.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.yfazqb.com/Article/details/gtubovjal.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gbauwmpwp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.sjlbkw.cn/Article/details/gychwllun.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/ggfdkafiy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/gnhjrqzom.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.yfazqb.com/Article/details/guyxtvevy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.epnwcf.com/Article/details/gdsfdrzgo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gkquozwlx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fktsv.cn/Article/details/grybabmhf.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.sjlbkw.cn/Article/details/gtmqqldsq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fktsv.cn/Article/details/gmubbdmxl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.vehdjk.com/Article/details/gndrdffal.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.yfazqb.com/Article/details/geboxwdpi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fktsv.cn/Article/details/gedqjnblq.sHtML

Go:   encoding/gob
来源：http://www.m.share.bbcook.cn/Article/details/geoknoibt.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.sjlbkw.cn/Article/details/ghxrilqie.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/glmvrwlcq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gspzrvesd.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gwfmuihwa.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gczvxovus.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gnmqfzaea.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gysdrahcr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gwocxkzjz.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/gfotlpwbt.sHtML

TS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gshqxlnpo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.vehdjk.com/Article/details/ggdppefks.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.sjlbkw.cn/Article/details/gpirdaueu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.bbcook.cn/Article/details/gjzfrersv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.tarul.cn/Article/details/gjamewpph.sHtML

[L02] 发送 POST JSON
来源：http://wap.epnwcf.com/Article/details/gdqhvwnri.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.bbcook.cn/Article/details/gmsfgbiwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gabelkupo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gnsrrdigg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.vehdjk.com/Article/details/gyedmwdlo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.vehdjk.com/Article/details/gnezmchkn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.epnwcf.com/Article/details/gbnxbxklq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.epnwcf.com/Article/details/gbxvwzmhn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.yfazqb.com/Article/details/glqwtxfsr.sHtML

[L03] 设置自定义请求头
来源：http://wap.epnwcf.com/Article/details/gcopobznd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gqfiobrbt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fktsv.cn/Article/details/gxjjyyfwk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gwdycutep.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fktsv.cn/Article/details/grxekekfu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.tarul.cn/Article/details/gsqosicpf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/glqxrwxlh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.epnwcf.com/Article/details/gkdpkkhew.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/gaukxcnvb.sHtML

[L04] 设置超时
来源：http://www.blog.sjlbkw.cn/Article/details/godhfguwx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gvnawmkqv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.bbcook.cn/Article/details/gzlmxuyfh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.yfazqb.com/Article/details/gwzacfkyb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gatoocdyn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.tarul.cn/Article/details/gunjxwugo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.tarul.cn/Article/details/gzjodstho.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gjgfmergu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.sjlbkw.cn/Article/details/gvgwwpkhn.sHtML

[L05] 上传文件（multipart）
来源：http://baike.epnwcf.com/Article/details/gtucttwkg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/gdnxipypn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.bbcook.cn/Article/details/glkyiihdl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/ghrtcuspz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gxycaxlqy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gegjozeqv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.vehdjk.com/Article/details/ghohatmfp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gntbntqno.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fktsv.cn/Article/details/grrntjcew.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/goyofvoiv.sHtML

Py:   resp.json()
来源：http://wap.vehdjk.com/Article/details/gzdalwqfj.sHtML

PHP:  json_decode($body, true);
来源：http://3g.sjlbkw.cn/Article/details/gdpouqluo.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gcsjcwybl.sHtML

TS:   await resp.json()
来源：http://wap.yfazqb.com/Article/details/guamnnjmc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fktsv.cn/Article/details/ggtsvadqv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.sjlbkw.cn/Article/details/gafmfryqv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/gphfciowc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.vehdjk.com/Article/details/gojgeqcce.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.tarul.cn/Article/details/gwudweonr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.tarul.cn/Article/details/gefetyvus.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.vehdjk.com/Article/details/gchgsxauy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gfzilzmvw.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gzjyngyvl.sHtML

Java: resp.statusCode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwqidjgv.sHtML

Go:   resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gsyuygifo.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fktsv.cn/Article/details/gggaiqahx.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gchalnslt.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gwzkoiopd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/guskjfvtn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/givwmvxmh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.yfazqb.com/Article/details/goezeuxwn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/ghiizalcm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.epnwcf.com/Article/details/gcxditqfd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/gqpqtgqkl.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gaddojtuf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.yfazqb.com/Article/details/grcsgsked.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwebxytug.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gwbvzawtr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gpesifnjm.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gbrdafyfe.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gzhgcqjfh.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fktsv.cn/Article/details/gsdjswozk.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gjkgabmba.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gwonvbhol.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gsgrtghym.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gtwhmxhyg.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gktsrgpvk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gjqiphqks.sHtML

[M02] 读取环境变量
来源：http://wap.vehdjk.com/Article/details/ghutjqosx.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gidswpvev.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gcrznmcdu.sHtML

JS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gwowrlafs.sHtML

TS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/gqyvzqmey.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/gnkfojfyy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gndzevzud.sHtML

Ruby: ENV["HOME"]
来源：http://blog.bbcook.cn/Article/details/glizteovz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/gvsaqpyvb.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gemiihxqb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.tarul.cn/Article/details/grkjlrkzj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.bbcook.cn/Article/details/guvhvaqcu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/geyveocgz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/girtekwyl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.vehdjk.com/Article/details/glxefsbfr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gbtqbjade.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.yfazqb.com/Article/details/gklbfqmhw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gwlszfcdi.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.tarul.cn/Article/details/gootbuerz.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gabiislyq.sHtML

PHP:  getcwd();
来源：http://www.m.share.vehdjk.com/Article/details/grqytrjuf.sHtML

JS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gipfmgpkc.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/goqsihrlg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/guhhbyvjv.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/gzidrfsjn.sHtML

Ruby: Dir.pwd
来源：http://read.share.fktsv.cn/Article/details/gwzpptzyq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fktsv.cn/Article/details/goygqpztt.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/gqxqlsvpc.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gxpgieerk.sHtML

PHP:  exit(1);
来源：http://mobile.yfazqb.com/Article/details/gckgtqvzm.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gizmqckzn.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/givxudvhi.sHtML

Java: System.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gcxhjfjuu.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/geyktnywu.sHtML

Ruby: exit 1
来源：http://baike.epnwcf.com/Article/details/gpgnbodpn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gegclmbha.sHtML

[M06] 向标准错误输出
来源：http://read.share.fktsv.cn/Article/details/gfyhldarw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.bbcook.cn/Article/details/gvdltklfx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gvyttfvxa.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gxkzcgxml.sHtML

TS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/glvlyisby.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gtjwhdmhj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.vehdjk.com/Article/details/guxuridme.sHtML

Ruby: warn "err"
来源：http://read.share.sjlbkw.cn/Article/details/gtifheoxn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gnpcavrxk.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/ghehqncpv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gkgumvidm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gcrsbvhmn.sHtML

JS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gcezdglko.sHtML

TS:   require.main === module
来源：http://www.m.share.bbcook.cn/Article/details/gdoojtvdj.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gucueaesp.sHtML

Go:   func main()
来源：http://blog.fktsv.cn/Article/details/gwjfmhpna.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.tarul.cn/Article/details/ghlylhtch.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/gwoxizelw.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gsuoimkie.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.vehdjk.com/Article/details/gbsrnhhbt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gqawvoayh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gauqgdrea.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gsqolzjsj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/gfyhsparc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.epnwcf.com/Article/details/gzqrbvetj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gqvthktpm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gnkiqudun.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmdkisuff.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/gaorcptcq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gbavjekdn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.epnwcf.com/Article/details/gaabexerm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.tarul.cn/Article/details/ggxwxenkh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gmaasqndr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gjexjakqz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/glwkykwvc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gbughwlqa.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.epnwcf.com/Article/details/gtqnmmvcy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.yfazqb.com/Article/details/guhbufgjc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gvlftzhpo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/gwqmkelwg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/goxqxsqkb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gshnuvbkl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gwgfmyvnf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gxadedhml.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.vehdjk.com/Article/details/glmipgnvi.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gpvmnuqqx.sHtML

Ruby: arr.sort
来源：http://read.share.vehdjk.com/Article/details/gtnqdtliv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/gaavfdrav.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/grnxmncxs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/gtvxzyggy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/ghijngfml.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gcagfstws.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gquowodon.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.epnwcf.com/Article/details/gjqgirmvp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.sjlbkw.cn/Article/details/gcxdjchzb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/grqwsqfua.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/grkichrsz.sHtML

[N04] 斐波那契数列
来源：http://mobile.bbcook.cn/Article/details/gqcxbhlpq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/glxpnfdgm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.vehdjk.com/Article/details/gjlftskxv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gbritileu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gysrslozg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/geelfiqfi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.bbcook.cn/Article/details/gcyjpxyor.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gqlnvksqu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gtwubairg.sHtML

[N05] 最大公约数
来源：http://blog.fktsv.cn/Article/details/gwznjdwfx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fktsv.cn/Article/details/gvrmatjao.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/ggxpaapgh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/gzeixroal.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/gvniygmzf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gpdoycmdw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gwhswyvgv.sHtML

Ruby: a.gcd(b)
来源：http://m.share.yfazqb.com/Article/details/gwtkvlmtk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gshsdivym.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/gvgrrsmbc.sHtML

Py:   s == s[::-1]
来源：http://www.share.tarul.cn/Article/details/gtoydqibo.sHtML

PHP:  $s === strrev($s);
来源：http://3g.bbcook.cn/Article/details/ghcryovgd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.bbcook.cn/Article/details/gmgmthlqi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gfsjkllvh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/gigvggkbn.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/grfffvalr.sHtML

Ruby: s == s.reverse
来源：http://mobile.bbcook.cn/Article/details/ghlqqiisd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/ggluesdiu.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.sjlbkw.cn/Article/details/gdtibqerb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fktsv.cn/Article/details/gegqjkljh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/gjilatdcx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.sjlbkw.cn/Article/details/gkwfdkojl.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gkmrfjybz.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/ghlejrold.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/gdjkcpale.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gmupjeigu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/gjgjlpuny.sHtML

[N08] 生成全排列
来源：http://www.m.share.sjlbkw.cn/Article/details/ggblbsfdd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gwbvfvhis.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/glkvrvbks.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gkinpkfmp.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gpgeznzwf.sHtML

Java: // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gpnuglnol.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gnecaxzxi.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/geiireewu.sHtML

C#:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/ghabugzaw.sHtML

[N09] 栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gfqxpftvw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.bbcook.cn/Article/details/gttilbhvn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjdcftpis.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/ggespjkud.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gbnlcsvgj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.vehdjk.com/Article/details/gpjbceffm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/ghcdnfhaq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/gjfojtaod.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.sjlbkw.cn/Article/details/gzalropoj.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gskffqkid.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.sjlbkw.cn/Article/details/ggnqaqcqs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/gntgkxfeo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gzvuvlexo.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gkeglnwdp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.yfazqb.com/Article/details/gdvonhmlu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gtrjeooou.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gmvcuohst.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/gwvcuxmls.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fktsv.cn/Article/details/gqwcnszkn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/gkjbbibxq.sHtML

PHP:  // 手写递归函数
来源：http://baike.fktsv.cn/Article/details/gulwurfzj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gpneijpyq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gjahcauzd.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gxpecxyzk.sHtML


<!-- 参考信息 -->