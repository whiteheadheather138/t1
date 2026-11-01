代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gioaybzie.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gqbxbbwzv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fktsv.cn/Article/details/gjzmaqblo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fktsv.cn/Article/details/gsxqgxorw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.yfazqb.com/Article/details/glewutngl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fktsv.cn/Article/details/gbfdalodl.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fktsv.cn/Article/details/genglkjoo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.yfazqb.com/Article/details/gboimmoxh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.vehdjk.com/Article/details/gpaoaxohe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.vehdjk.com/Article/details/goyoqufig.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/genleryfo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fktsv.cn/Article/details/gfiduasuf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.vehdjk.com/Article/details/gnyiqcwws.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.yfazqb.com/Article/details/glhlhggxe.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.sjlbkw.cn/Article/details/gelwiugsu.sHtML

[K05] 深拷贝对象
来源：http://read.share.vehdjk.com/Article/details/gngchfstz.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.yfazqb.com/Article/details/gttjtacfa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.bbcook.cn/Article/details/gdztpbdsx.sHtML

JS:   structuredClone(obj)
来源：http://www.share.vehdjk.com/Article/details/gecjpuxll.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/geddmlnhk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.tarul.cn/Article/details/gkpipbcwn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.tarul.cn/Article/details/gowetvmft.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.tarul.cn/Article/details/gzjurxnbi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.bbcook.cn/Article/details/gqcgwnjgy.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/gkpbrdnyu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gkpexxnkp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.tarul.cn/Article/details/gsgeilrcd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.yfazqb.com/Article/details/gsfafqiop.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fktsv.cn/Article/details/giqbsjjik.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.vehdjk.com/Article/details/gmhbvlgch.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.bbcook.cn/Article/details/gjlopktnb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.yfazqb.com/Article/details/gvdwblqer.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.epnwcf.com/Article/details/guyfqphgg.sHtML

[K07] 进制转换
来源：http://www.share.sjlbkw.cn/Article/details/gaxtpjgko.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.vehdjk.com/Article/details/gbhrjueeg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.tarul.cn/Article/details/gpojcmjem.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gtfjwqbnu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.epnwcf.com/Article/details/grmbbrcxy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.vehdjk.com/Article/details/gnabwhehu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.tarul.cn/Article/details/gznwravgk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fktsv.cn/Article/details/gueopkbjp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.vehdjk.com/Article/details/gtymslrmq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.bbcook.cn/Article/details/gjaygtqmv.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.bbcook.cn/Article/details/gpyfuvmox.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.yfazqb.com/Article/details/gbvpoznjf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.sjlbkw.cn/Article/details/gspusvcdc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.epnwcf.com/Article/details/gmkwhgddi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.sjlbkw.cn/Article/details/gzzgmakzl.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gtuxqwjtl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.sjlbkw.cn/Article/details/gmgcbdyjn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/ggnobfgpm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gitxanuwd.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gvfcibmwj.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gnqaathts.sHtML

[L01] 发送 GET 请求
来源：http://baike.epnwcf.com/Article/details/gleodzkxy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fktsv.cn/Article/details/gfnnjgcii.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.bbcook.cn/Article/details/grubsyoms.sHtML

JS:   await fetch(url)
来源：http://blog.epnwcf.com/Article/details/gkainwyge.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gxzotivsm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.bbcook.cn/Article/details/gotuajctz.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.tarul.cn/Article/details/goqjuqbij.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.epnwcf.com/Article/details/gkkfifbic.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.yfazqb.com/Article/details/gpmxgqihr.sHtML

[L02] 发送 POST JSON
来源：http://wap.bbcook.cn/Article/details/gedtqngax.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.yfazqb.com/Article/details/gibuzjvjo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.sjlbkw.cn/Article/details/gkmnjakgb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/guonvspad.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fktsv.cn/Article/details/gcxpatpmu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.yfazqb.com/Article/details/gnwgoljpt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fktsv.cn/Article/details/gztqrmmel.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.sjlbkw.cn/Article/details/gdnpvpxti.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.vehdjk.com/Article/details/gdctjeczt.sHtML

[L03] 设置自定义请求头
来源：http://baike.sjlbkw.cn/Article/details/gyqyvppkt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fktsv.cn/Article/details/gkdkjkwfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.bbcook.cn/Article/details/gfvmcllke.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/gjjstkmzt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.sjlbkw.cn/Article/details/gtxghlhqe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fktsv.cn/Article/details/gskfpedxa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gqhmcdneo.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/gzritjnwq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fktsv.cn/Article/details/gmaaizdfx.sHtML

[L04] 设置超时
来源：http://3g.yfazqb.com/Article/details/gfpafrrzy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.sjlbkw.cn/Article/details/gfrklejhm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.yfazqb.com/Article/details/gtjfhzipb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.epnwcf.com/Article/details/gichbikku.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.yfazqb.com/Article/details/gzysqegmy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.tarul.cn/Article/details/glkeeehuw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/ghorxvpyq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.vehdjk.com/Article/details/gsvicefic.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gechurivl.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gjwpfccfp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.bbcook.cn/Article/details/gdopyngfv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.yfazqb.com/Article/details/gniziaxsu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.yfazqb.com/Article/details/gogintpbc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.tarul.cn/Article/details/gqfnqlbpz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/gkxfprzvh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gacpxvwhf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.vehdjk.com/Article/details/gknhtmhgy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/glegkrqob.sHtML

[L06] 解析响应为 JSON
来源：http://3g.epnwcf.com/Article/details/gnhkpyicp.sHtML

Py:   resp.json()
来源：http://baike.fktsv.cn/Article/details/gvamdgacc.sHtML

PHP:  json_decode($body, true);
来源：http://baike.vehdjk.com/Article/details/gxnmasuhh.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gbcdkisuu.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/guopoikxd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/ggfvfihiy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/gqsgmwxzo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.vehdjk.com/Article/details/gjlikzoib.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.epnwcf.com/Article/details/gcuvobylr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.sjlbkw.cn/Article/details/gmrlwjfzk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/gmbyquxol.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.tarul.cn/Article/details/gelzdlmwc.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.sjlbkw.cn/Article/details/gwoksylyu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.vehdjk.com/Article/details/geisjoqml.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gkgheionr.sHtML

Go:   resp.StatusCode
来源：http://3g.sjlbkw.cn/Article/details/glaedesdi.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fktsv.cn/Article/details/gupapzwpz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gxgateaxl.sHtML

[L08] 并发请求多个地址
来源：http://m.share.yfazqb.com/Article/details/gqttmbask.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gncffcniq.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gluhkhesz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gckccbzme.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gocklrmti.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.sjlbkw.cn/Article/details/gggbdprzi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/gknsfiihj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gzwajbwnt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.sjlbkw.cn/Article/details/gthfrqsla.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gwlvcbpqk.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fktsv.cn/Article/details/gbkskjnru.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gzpyjmwkb.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/guwvfiedm.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fktsv.cn/Article/details/gwusalend.sHtML

PHP:  $argv;  $argc;
来源：http://baike.sjlbkw.cn/Article/details/gerofpmfd.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gvxfjfznx.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/gbiuqszci.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gsfpkbejp.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/gsfjnkdah.sHtML

Ruby: ARGV
来源：http://www.share.yfazqb.com/Article/details/guaejpvbq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gmcagsxqj.sHtML

[M02] 读取环境变量
来源：http://blog.tarul.cn/Article/details/gefpmcdnv.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gaadyjbcq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gryaivret.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gktccueec.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/glhvjskap.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/guoxxpdsb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcivoehqi.sHtML

Ruby: ENV["HOME"]
来源：http://blog.sjlbkw.cn/Article/details/ghatdtpzw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gitcqpgsa.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/glnhjzduk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gktoctrat.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gqlaxuewq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fktsv.cn/Article/details/gyqpfsnfj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gybmyjaus.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gmpggcpev.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.tarul.cn/Article/details/gscpquugc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fktsv.cn/Article/details/gkmbsjnky.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.sjlbkw.cn/Article/details/gjdpcrjky.sHtML

[M04] 获取当前工作目录
来源：http://mobile.vehdjk.com/Article/details/guwsctdyf.sHtML

Py:   os.getcwd()
来源：http://blog.tarul.cn/Article/details/gjglbvizp.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/girjayisx.sHtML

JS:   process.cwd()
来源：http://baike.tarul.cn/Article/details/gkukzompk.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gudilziwu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gvcpzfuro.sHtML

Go:   os.Getwd()
来源：http://read.share.sjlbkw.cn/Article/details/gnthbiyqz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gxkglsxfv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.yfazqb.com/Article/details/gdithzlxu.sHtML

[M05] 设置退出码
来源：http://blog.epnwcf.com/Article/details/gowydgwfb.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/gbnpjuppn.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gdivfetjs.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjfyiplff.sHtML

TS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gxyedywwy.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gnwagfkzt.sHtML

Go:   os.Exit(1)
来源：http://wap.vehdjk.com/Article/details/gmuckdmzd.sHtML

Ruby: exit 1
来源：http://blog.sjlbkw.cn/Article/details/gqbsfvfym.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.bbcook.cn/Article/details/gdkkiorje.sHtML

[M06] 向标准错误输出
来源：http://blog.yfazqb.com/Article/details/gsltzmjjc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtdfjvxjg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/ggdptfvjn.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gefxydrde.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gmgnwayri.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gfmzsdxxv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.vehdjk.com/Article/details/gagqyhhvk.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gtbatqrpw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.yfazqb.com/Article/details/gexghhuzu.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/gvadfrbrz.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gdfstatwd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.yfazqb.com/Article/details/goravtcev.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gogdsbglh.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gilicyhpj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gfxgdmsja.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/gnkliejwj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.epnwcf.com/Article/details/gzgcuzxxz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gxrxzcicx.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gwgtpepum.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkwcfcogc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/gfbfxagha.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/grehyngot.sHtML

TS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/gmnuemtyk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/gtaccdxpv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/grlfwxuvd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.yfazqb.com/Article/details/gsbrnirwk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gxjewzjoj.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gyqzjluwh.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/gcquyvpde.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gczzswpzg.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.vehdjk.com/Article/details/gwebtqtkg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gvwzrzgmc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fktsv.cn/Article/details/gowyczhuq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/ghdimlbjo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gbaqpmhfl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gzhxsmnpo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gsfephnfc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmxekqeuz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gwjicweya.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gyjnknfqk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fktsv.cn/Article/details/gjjkhmkmb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.tarul.cn/Article/details/gechloyvx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/grglapora.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/gwbpofrmp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.vehdjk.com/Article/details/gayeahhzx.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gqndrdzrq.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/guyuwvfof.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gpiwoqbmn.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fktsv.cn/Article/details/gefqmxifq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gtnqkmeyy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.yfazqb.com/Article/details/gzxalrhgz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gomygastr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.bbcook.cn/Article/details/gouppzodc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.tarul.cn/Article/details/gqrkmfqui.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.vehdjk.com/Article/details/gatnmlqgg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gcdbwewch.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.vehdjk.com/Article/details/gmxclvqse.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/gsrowbvrh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.vehdjk.com/Article/details/gvxkxugvz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gytmvkdac.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gpgmziyed.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/ggvshgcmv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gwtjuehev.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/gxxchztao.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gometmggt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/ggfsyojih.sHtML

[N05] 最大公约数
来源：http://read.share.bbcook.cn/Article/details/gqauejkrt.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fktsv.cn/Article/details/gxtvjzwsj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/gpkaoymeq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.bbcook.cn/Article/details/ghceoyhqz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/giqqakvwf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fktsv.cn/Article/details/gnlokklol.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.sjlbkw.cn/Article/details/gpofjfhsx.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.vehdjk.com/Article/details/ggudyzgin.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gpcmzitcl.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.epnwcf.com/Article/details/gzdvifyeb.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gypzbuovz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.yfazqb.com/Article/details/ghirjybms.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/ghogzpqor.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.vehdjk.com/Article/details/gnycuzsly.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gujgzgani.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.yfazqb.com/Article/details/gpaovgmtv.sHtML

Ruby: s == s.reverse
来源：http://m.share.yfazqb.com/Article/details/gwnordcnf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gacsqxtjm.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.epnwcf.com/Article/details/gjzywfkfm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gocaettyh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gudlohnru.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.tarul.cn/Article/details/ggnuvmicr.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/ghqdxsdgb.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gakxynhjh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/gvprowfop.sHtML

Ruby: // 手写 Hash
来源：http://mobile.sjlbkw.cn/Article/details/gxgwigbeq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.sjlbkw.cn/Article/details/gzmyrxopy.sHtML

[N08] 生成全排列
来源：http://mobile.yfazqb.com/Article/details/guqozpzgs.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/glgitsaaz.sHtML

PHP:  // 手写递归交换
来源：http://blog.tarul.cn/Article/details/gtlxnwdls.sHtML

JS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gayolejyz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gcopwjsuu.sHtML

Java: // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/grtoyyxej.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gcqmrudar.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/googzltne.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gtosqnvqt.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gucyiyhnn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gzdbhomdp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gooqynthe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gwpcmbtdy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.epnwcf.com/Article/details/gfycavkiv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gonmaieus.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.bbcook.cn/Article/details/ghnxwfhbk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gxxlvgeoa.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.epnwcf.com/Article/details/gipdtbvyk.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gwjhtyevp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.vehdjk.com/Article/details/gckjxzhfc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gdoycdmca.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/gygolkooz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gfkmqpleu.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/gsvwjwpbv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fktsv.cn/Article/details/gspnedkru.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gqazeeudk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.epnwcf.com/Article/details/gqqxvekvm.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/gcpncdemw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.sjlbkw.cn/Article/details/gykrnfcsu.sHtML

PHP:  // 手写递归函数
来源：http://3g.yfazqb.com/Article/details/gwetbrvcn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gmaegekbb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gtthkhaai.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/givretdfx.sHtML


<!-- 参考信息 -->