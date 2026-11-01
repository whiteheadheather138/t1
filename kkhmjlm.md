代发 wailian999

TS:   JSON.parse(s)
来源：http://baike.tarul.cn/Article/details/gwwtjeejs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.sjlbkw.cn/Article/details/ggcldnlfe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.sjlbkw.cn/Article/details/gmramhuyf.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.yfazqb.com/Article/details/gjdzhpmoc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.bbcook.cn/Article/details/gsgvmgral.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.bbcook.cn/Article/details/gnydaqpck.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.tarul.cn/Article/details/gljoyktfm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gnxwvzfjs.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gjsgalonw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.yfazqb.com/Article/details/gelltfjfh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.yfazqb.com/Article/details/gbosadffk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.bbcook.cn/Article/details/goxqbwfsd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.epnwcf.com/Article/details/gwgoggblk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.vehdjk.com/Article/details/gwjfxaidg.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.epnwcf.com/Article/details/gtehvthqr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fktsv.cn/Article/details/gghbflawk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.bbcook.cn/Article/details/gupyqytwk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gleopieob.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.bbcook.cn/Article/details/gviikemma.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.bbcook.cn/Article/details/gihduzjpa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.yfazqb.com/Article/details/gaxifsjdb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fktsv.cn/Article/details/gcuhlvhtt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gqkxefpak.sHtML

[K05] 深拷贝对象
来源：http://m.share.yfazqb.com/Article/details/gcfzezkjd.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.epnwcf.com/Article/details/gicrmumhr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.sjlbkw.cn/Article/details/gspgurhzp.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fktsv.cn/Article/details/gwuzqtzcq.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fktsv.cn/Article/details/gmmvpjint.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fktsv.cn/Article/details/gvxtccnyp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fktsv.cn/Article/details/ggovoovdu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.sjlbkw.cn/Article/details/gshweuqtv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.yfazqb.com/Article/details/gpawjykqi.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.epnwcf.com/Article/details/gjlayzquz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.tarul.cn/Article/details/glqdtotls.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.epnwcf.com/Article/details/gwtejnzry.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gxbpyvrbe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.sjlbkw.cn/Article/details/gvbrpeyae.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gcznrtadz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/gevmcahgk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggijddiub.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.epnwcf.com/Article/details/gelurjjxo.sHtML

[K07] 进制转换
来源：http://www.m.share.vehdjk.com/Article/details/gcmonfwts.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.vehdjk.com/Article/details/ghovpbyec.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.yfazqb.com/Article/details/gxnfhikrx.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gnsdhsrhd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gpcdwauxt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/ggyccdkiu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.vehdjk.com/Article/details/gueefmfrp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.epnwcf.com/Article/details/gnxholofv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gtaywcgin.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fktsv.cn/Article/details/gnciodprw.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.tarul.cn/Article/details/gnnbwpurj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.epnwcf.com/Article/details/gegwezzyj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gsxrqmago.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gouxdkgaw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/gzlkonwau.sHtML

Go:   encoding/gob
来源：http://m.share.sjlbkw.cn/Article/details/gbcddhfee.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.tarul.cn/Article/details/gbxwvgplw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.sjlbkw.cn/Article/details/gwnkvbnqi.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grvpzlaph.sHtML

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/ghthvzsyr.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gsfpxouqi.sHtML

[L01] 发送 GET 请求
来源：http://3g.tarul.cn/Article/details/gmljuadmu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gfvbewbga.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.yfazqb.com/Article/details/gdimvbxbi.sHtML

JS:   await fetch(url)
来源：http://mobile.yfazqb.com/Article/details/gvzqxvtij.sHtML

TS:   await fetch(url)
来源：http://baike.vehdjk.com/Article/details/gbcvgnmpm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.tarul.cn/Article/details/garnmzetn.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fktsv.cn/Article/details/ghufnzgvy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gtreajlti.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/gajqncnws.sHtML

[L02] 发送 POST JSON
来源：http://blog.bbcook.cn/Article/details/guvcfngty.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgjygzgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.yfazqb.com/Article/details/gorjbmqdq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.tarul.cn/Article/details/gdrwgnnwa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gnsqidwtl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.epnwcf.com/Article/details/gppcsrrno.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gnoyfmrsz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.sjlbkw.cn/Article/details/gvmflblkb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.tarul.cn/Article/details/gceqitesu.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gsvfwfamq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fktsv.cn/Article/details/gxoxydlrd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.tarul.cn/Article/details/gzaoacatx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.tarul.cn/Article/details/ghqyzgrkv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/gfiuddruh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.yfazqb.com/Article/details/gzqffjtbq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gkntgfbeu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.vehdjk.com/Article/details/gsfhkvhwd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.sjlbkw.cn/Article/details/ghgkxodyz.sHtML

[L04] 设置超时
来源：http://m.share.tarul.cn/Article/details/gpjrknvon.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/gqmhugoga.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.bbcook.cn/Article/details/ghexkkadj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gaysqgqbm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/grgaafkmh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.vehdjk.com/Article/details/gneuymwyh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.vehdjk.com/Article/details/glzxtbzby.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fktsv.cn/Article/details/gwtwixwfs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/gtcbkojbv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/gcfkguvwr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.sjlbkw.cn/Article/details/gtphfvkdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.epnwcf.com/Article/details/ggdycvoto.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/glbwqdrjn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.vehdjk.com/Article/details/gaiufrusl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gxhfddkpl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/gkqabxljb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.tarul.cn/Article/details/gbsrsmnjm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/grhnqklsg.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/giiffuetu.sHtML

Py:   resp.json()
来源：http://www.share.fktsv.cn/Article/details/glcqvfjrl.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fktsv.cn/Article/details/gmudwjqrv.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/ggdxhrmen.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gamafirih.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fktsv.cn/Article/details/guizoblfs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.bbcook.cn/Article/details/gexvmakux.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/ghvwprcbl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.yfazqb.com/Article/details/ggvghuglv.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gxlqhydol.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gkpxtebch.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gbdqnilda.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gwkndplzb.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/ghytaklit.sHtML

Java: resp.statusCode()
来源：http://blog.bbcook.cn/Article/details/gyduxtaev.sHtML

Go:   resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gqttysequ.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/grlovivqt.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gpybsnbbi.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gobvgzqfv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.epnwcf.com/Article/details/gcikivzqw.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gignjnefl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.tarul.cn/Article/details/gnaeapjyg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gftvfevuo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gmbmshonk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.vehdjk.com/Article/details/gjfvwywkb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.sjlbkw.cn/Article/details/gnvxuwmij.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gordviuiy.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gqodfksxr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.tarul.cn/Article/details/gvnlmuzni.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gzxznbwic.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gthaxehdq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.vehdjk.com/Article/details/gllrwfwze.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/gwhssweyv.sHtML

JS:   process.argv.slice(2)
来源：http://wap.sjlbkw.cn/Article/details/gelcclcka.sHtML

TS:   process.argv.slice(2)
来源：http://wap.vehdjk.com/Article/details/gfjagcfnt.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/gsetwojta.sHtML

Go:   os.Args[1:]
来源：http://www.share.epnwcf.com/Article/details/gpzocjsqz.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/grmwmzbrm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/galxupalt.sHtML

[M02] 读取环境变量
来源：http://3g.yfazqb.com/Article/details/gqrehjewl.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.yfazqb.com/Article/details/geqpajuwq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.sjlbkw.cn/Article/details/gsznvdjod.sHtML

JS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/glmxaczfc.sHtML

TS:   process.env.HOME
来源：http://blog.fktsv.cn/Article/details/gjyoubdfr.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gxifilfyb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/ghgtulrsm.sHtML

Ruby: ENV["HOME"]
来源：http://wap.epnwcf.com/Article/details/gwlmhrqxu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.epnwcf.com/Article/details/grebapeng.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gzdrshwsv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.bbcook.cn/Article/details/gdbnjjzoh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.tarul.cn/Article/details/gwbmgzymp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gybyofwkk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/girvqvgkn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gqyagbkzm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.sjlbkw.cn/Article/details/gnwywyxny.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.sjlbkw.cn/Article/details/gcocddauu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.tarul.cn/Article/details/ggxvzgque.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.yfazqb.com/Article/details/gthrrrjsb.sHtML

Py:   os.getcwd()
来源：http://www.share.tarul.cn/Article/details/ggpyqwolm.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/getzionsg.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gsjwffdgt.sHtML

TS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/ghteoibus.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/gluttoxwi.sHtML

Go:   os.Getwd()
来源：http://www.share.sjlbkw.cn/Article/details/ggdxhqtxs.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gxrmquhjl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.tarul.cn/Article/details/gypngixbc.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gykrbtgua.sHtML

Py:   sys.exit(1)
来源：http://wap.vehdjk.com/Article/details/gwwwiasmp.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gobwiiyms.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gmiphzuio.sHtML

TS:   process.exit(1)
来源：http://wap.fktsv.cn/Article/details/gqsfqmjdv.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/ghutwclid.sHtML

Go:   os.Exit(1)
来源：http://blog.vehdjk.com/Article/details/gslilgwss.sHtML

Ruby: exit 1
来源：http://blog.vehdjk.com/Article/details/gbnppdozr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.epnwcf.com/Article/details/ghtgujpop.sHtML

[M06] 向标准错误输出
来源：http://read.share.epnwcf.com/Article/details/gcpkfctkv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.yfazqb.com/Article/details/gkqiwlzua.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/gtfcllnxn.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/ggvqgqjul.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gizaugbba.sHtML

Java: System.err.println("err")
来源：http://www.blog.yfazqb.com/Article/details/gaimpfbzm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.yfazqb.com/Article/details/gcgzadqwh.sHtML

Ruby: warn "err"
来源：http://read.share.epnwcf.com/Article/details/gpuuvplwi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.yfazqb.com/Article/details/gyjhntjpy.sHtML

[M07] 判断是否为主入口
来源：http://m.share.sjlbkw.cn/Article/details/gmjgyvojz.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.sjlbkw.cn/Article/details/golrmeonk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/grlulytqp.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gaiwzaxum.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gwmeznzxo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/giucmwmwg.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gmufxdcxw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gdnrxddke.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.tarul.cn/Article/details/gychaymvv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.vehdjk.com/Article/details/gbkvhrrli.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gidmozgkl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gkruohxjn.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gvosaagrc.sHtML

TS:   process.platform;  process.version
来源：http://3g.bbcook.cn/Article/details/gwfyqqryy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gyusykrzl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gnqgizpyd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.bbcook.cn/Article/details/ghdxcptcd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.tarul.cn/Article/details/gkjnjkaql.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gpyabaage.sHtML

N. 数据结构与算法
来源：http://www.blog.tarul.cn/Article/details/glidmynzz.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grfoiodyz.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gotnlsjfo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gxbpfswps.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gqxnetnvo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.epnwcf.com/Article/details/gwasxdnxh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gdjaxxafk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gzggfzjuo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gpzgmqphz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.sjlbkw.cn/Article/details/gdwanvmuu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gpmsobbvx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/gevjrvdyh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gfqctngqg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gecpnwbdr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/ggdtefyco.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gzwipicbu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fktsv.cn/Article/details/gsobvkksd.sHtML

Go:   slices.Sort(arr)
来源：http://blog.bbcook.cn/Article/details/goakaggzx.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/ggybrjsfi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.yfazqb.com/Article/details/gfckejpgw.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.yfazqb.com/Article/details/gxaevoeqn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/gwsrpccmr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gmcwzdrjx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.epnwcf.com/Article/details/gathrvadr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gqvktmthj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.yfazqb.com/Article/details/gmirngfqz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gemhpopqd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.tarul.cn/Article/details/ggpreeoxl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.epnwcf.com/Article/details/goqrjlehj.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/gkeqwuwhe.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/ggohkpxlv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/gtlrmojir.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gxlryubyk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/ghtmrpajj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fktsv.cn/Article/details/glvgmqzzu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gihojojkr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gwocmhsmm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/garefpowm.sHtML

[N05] 最大公约数
来源：http://3g.fktsv.cn/Article/details/genaatiay.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gladepeaq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gencalhgv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gltecwjgt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gutypgude.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.yfazqb.com/Article/details/gnbkowcbv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/ggyzuuekc.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/goypiabrm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/ggzalgrbr.sHtML

[N06] 判断回文字符串
来源：http://blog.fktsv.cn/Article/details/gllhuwtoy.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gfjrgzgiz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.sjlbkw.cn/Article/details/gzrvawsxs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.sjlbkw.cn/Article/details/gojkkaenp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gpcuztmcp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gehwswcjj.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.vehdjk.com/Article/details/gakefhjhe.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gvhiltdrp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gdpkamehk.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.tarul.cn/Article/details/gmqhurodl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/gsxqhlqcu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gbmdqfzqa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.yfazqb.com/Article/details/gplpirtvq.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.epnwcf.com/Article/details/grjaqckmr.sHtML

Java: // 手写 HashMap
来源：http://blog.vehdjk.com/Article/details/gmcwrznch.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/girgosdqm.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.epnwcf.com/Article/details/gdhwltckg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/grauovqno.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/giextfopf.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.bbcook.cn/Article/details/gwbwfrfgl.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gnomjvibz.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/geoqzzcbx.sHtML

TS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/ggmsdlpzb.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gpqpgezyt.sHtML

Go:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/gstdgnkqx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.bbcook.cn/Article/details/gjjnllprk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gidavyocp.sHtML

[N09] 栈与队列
来源：http://read.share.yfazqb.com/Article/details/gilncwyzt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gbantuzvq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gukbdpftv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gsxeyfdex.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.sjlbkw.cn/Article/details/gjypjwdyq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/goheqpllj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/gxtrdbuom.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/gfwerpvfl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fktsv.cn/Article/details/guxufpeup.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gatojvcrf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/geffhyntv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gtvphsrej.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/giyferldp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.yfazqb.com/Article/details/gkhviednk.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fktsv.cn/Article/details/gpeakwpnm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gvcrdlcwm.sHtML


<!-- 参考信息 -->