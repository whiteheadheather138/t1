代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.tarul.cn/Article/details/groetynrf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.yfazqb.com/Article/details/gbaszulsw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.bbcook.cn/Article/details/gmcksbqyo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fktsv.cn/Article/details/gyssjpfnt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.vehdjk.com/Article/details/gloseggmw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.yfazqb.com/Article/details/gjpjojmuh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fktsv.cn/Article/details/gtxadohez.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.epnwcf.com/Article/details/gxdsggwni.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fktsv.cn/Article/details/gclzzhrif.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.tarul.cn/Article/details/gzxqelydr.sHtML

[K04] 读取 JSON 文件
来源：http://baike.yfazqb.com/Article/details/gkamejwbw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fktsv.cn/Article/details/gpipbgvkw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.yfazqb.com/Article/details/grodyvnub.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gxisaqmqc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.bbcook.cn/Article/details/geudxnaik.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gxxwrehyy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.epnwcf.com/Article/details/guzgvvrnf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.epnwcf.com/Article/details/grtaqrgpd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/geejugzoi.sHtML

[K05] 深拷贝对象
来源：http://wap.epnwcf.com/Article/details/grglxnbwe.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.epnwcf.com/Article/details/gdwhbrzhq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.yfazqb.com/Article/details/gyfgzebkr.sHtML

JS:   structuredClone(obj)
来源：http://wap.yfazqb.com/Article/details/gwcrofnhz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.vehdjk.com/Article/details/gxdpiljzi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.yfazqb.com/Article/details/glozgdwnd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.sjlbkw.cn/Article/details/gmbiscldp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.sjlbkw.cn/Article/details/gabfvfyrd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/gfxmeievj.sHtML

[K06] 解析 URL 查询串
来源：http://wap.sjlbkw.cn/Article/details/gcjueotfc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fktsv.cn/Article/details/gfzwkxiuj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.epnwcf.com/Article/details/gyfoxbjne.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gukdyubpi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gzbpbrynh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.bbcook.cn/Article/details/gqqmybbdz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvcugzoyc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/ggqmvuivy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gwfrevvgm.sHtML

[K07] 进制转换
来源：http://3g.fktsv.cn/Article/details/gyhipqrja.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gxyxkocad.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/gnnooxbdg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gosvgdbou.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.vehdjk.com/Article/details/gbeupvopd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gmcdjsnwx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.sjlbkw.cn/Article/details/glblhfiil.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/goclarvrb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.epnwcf.com/Article/details/geyjrfumj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.yfazqb.com/Article/details/gxhbniynx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fktsv.cn/Article/details/gwvxicwsh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.yfazqb.com/Article/details/gkvmwllpw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gjlesvexg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/gbvsvdncm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.yfazqb.com/Article/details/gvijhqnbr.sHtML

Go:   encoding/gob
来源：http://m.share.epnwcf.com/Article/details/gvyazbdfe.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.tarul.cn/Article/details/gulbuqkvu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.sjlbkw.cn/Article/details/guewmpnfq.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gozypduzg.sHtML

L. 网络请求
来源：http://www.blog.sjlbkw.cn/Article/details/grjrnnswf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gmrceifsl.sHtML

[L01] 发送 GET 请求
来源：http://baike.fktsv.cn/Article/details/gdcaxthjg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.sjlbkw.cn/Article/details/geuuvtskw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.yfazqb.com/Article/details/gbmiquyck.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/goygakaot.sHtML

TS:   await fetch(url)
来源：http://read.share.yfazqb.com/Article/details/gscixwufb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/giekqhdqo.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.tarul.cn/Article/details/gsoeinjjy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.sjlbkw.cn/Article/details/gqayyfnpe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.yfazqb.com/Article/details/ggczjszbg.sHtML

[L02] 发送 POST JSON
来源：http://3g.tarul.cn/Article/details/glnmfkipq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/gmpjehaol.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.epnwcf.com/Article/details/gzdxnyswy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/ggfvxdysm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.yfazqb.com/Article/details/gqqqzwpsn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.sjlbkw.cn/Article/details/gumxgtxgd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fktsv.cn/Article/details/gckrztypc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/giudfmicu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.sjlbkw.cn/Article/details/giqauutnj.sHtML

[L03] 设置自定义请求头
来源：http://baike.tarul.cn/Article/details/ggmxgwqyz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.tarul.cn/Article/details/gkgchpnlf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.epnwcf.com/Article/details/guzaloejw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gdwkznolx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/gwbvifzxp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.tarul.cn/Article/details/gloosegnv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gpqsedgiy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.sjlbkw.cn/Article/details/gfhyrcsjr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.bbcook.cn/Article/details/ghhutnedl.sHtML

[L04] 设置超时
来源：http://3g.epnwcf.com/Article/details/gcgquwjpy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.bbcook.cn/Article/details/grlthdhmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.vehdjk.com/Article/details/gmgndkzhe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/gyzjtaoym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/ghbrxzglq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.yfazqb.com/Article/details/goyjvpzwh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.epnwcf.com/Article/details/grjhbzuwy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.epnwcf.com/Article/details/gzhufhtco.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fktsv.cn/Article/details/gsgmpnbuv.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fktsv.cn/Article/details/glrtfhfph.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/gqoewgmab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gggoippyo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gdccswsbr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gsdqhiiiy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fktsv.cn/Article/details/gxfjjmznv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.tarul.cn/Article/details/gxrxuypjt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.vehdjk.com/Article/details/ggjpnqctr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gtzvgqgyk.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/gmcqezlqm.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/gmwzgdrda.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gcwigayzf.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gvnzgyqft.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gcbqlpjkx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.sjlbkw.cn/Article/details/gbzyexjqn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/gelggyvro.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.yfazqb.com/Article/details/gusbpxfsj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gofkoriep.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.bbcook.cn/Article/details/ggkottrqp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.vehdjk.com/Article/details/gmkcbsfgk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gteahpxxt.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.bbcook.cn/Article/details/gbtmuimyx.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gzirsntfg.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gpbuornju.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/goqodmmao.sHtML

Ruby: resp.code.to_i
来源：http://wap.yfazqb.com/Article/details/gsxxwyrfq.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gptobiqov.sHtML

[L08] 并发请求多个地址
来源：http://mobile.yfazqb.com/Article/details/gnmqlrusc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gkaqjyruw.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fktsv.cn/Article/details/gijveubea.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.tarul.cn/Article/details/gaedcfzet.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gapwkkhxy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/gjyzuaoce.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.bbcook.cn/Article/details/gadoeohct.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.yfazqb.com/Article/details/gsjpwvuqr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/ggzqrgtfn.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gnefrvznt.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.epnwcf.com/Article/details/guamcvgdk.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gihmvesep.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gtnxlyeks.sHtML

Py:   sys.argv[1:]
来源：http://m.share.bbcook.cn/Article/details/gzqvltlzn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fktsv.cn/Article/details/gyjhkumht.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/glzwejcla.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/grubgkmny.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gxaxunwxj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.sjlbkw.cn/Article/details/gaadgvqne.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhyddmck.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gaakrtzcx.sHtML

[M02] 读取环境变量
来源：http://m.share.sjlbkw.cn/Article/details/gomluhwaj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gdtnzczsb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.epnwcf.com/Article/details/gdljildli.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gxrowaqtz.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gkilmtczb.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/gzwphffst.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gxdksmvtn.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.bbcook.cn/Article/details/gwgyeifxt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/gdklfjdyr.sHtML

[M03] 执行外部命令
来源：http://www.m.share.yfazqb.com/Article/details/gdiecithy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/gkzojcpro.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gsarzxfnm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/giqfjpuou.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gkpstjrox.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fktsv.cn/Article/details/grdwdfogy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gnexxjdqb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/ghgehoxfi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gelglmxiq.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/gcjfocvax.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/gragglxjl.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/gticijadu.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gqnjywgkr.sHtML

TS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/grjhfjxgo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gzkomyhbq.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/guhwozswv.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/ghxywrald.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gfjnqsmlq.sHtML

[M05] 设置退出码
来源：http://m.share.bbcook.cn/Article/details/gwlhazsgk.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/guuraeyhs.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gcfwtqqvs.sHtML

JS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gofavxziy.sHtML

TS:   process.exit(1)
来源：http://blog.bbcook.cn/Article/details/gigmjdili.sHtML

Java: System.exit(1)
来源：http://www.share.tarul.cn/Article/details/gvsyesrbn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gbustthco.sHtML

Ruby: exit 1
来源：http://mobile.fktsv.cn/Article/details/gwoyqkuyz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gdujimaxh.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gyzzvriap.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gmcngfwth.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.epnwcf.com/Article/details/givuiyiwl.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gygcjhocs.sHtML

TS:   console.error("err")
来源：http://mobile.yfazqb.com/Article/details/gziostieo.sHtML

Java: System.err.println("err")
来源：http://m.share.fktsv.cn/Article/details/gvxlihfgt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gtguhxsrz.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/gwspyypem.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.tarul.cn/Article/details/gnkdulkep.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/gqninpuze.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/glrfndaow.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/gnmwidzpi.sHtML

JS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gpjhnaxdz.sHtML

TS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/ggvhulyhd.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gkhpdaiyw.sHtML

Go:   func main()
来源：http://m.share.sjlbkw.cn/Article/details/gqqbbnpfn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.vehdjk.com/Article/details/ggvqfzggv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gihbzsdua.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gxamnvhmz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.yfazqb.com/Article/details/glfhypyfz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.yfazqb.com/Article/details/gddxqkeaf.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gaxezpyxd.sHtML

TS:   process.platform;  process.version
来源：http://baike.fktsv.cn/Article/details/gruswvmgd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.vehdjk.com/Article/details/gefgszvpf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/glbvkilzz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.epnwcf.com/Article/details/gfvkathuk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.bbcook.cn/Article/details/gafjaauwg.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gnjsunvnz.sHtML

N. 数据结构与算法
来源：http://www.m.share.vehdjk.com/Article/details/gffdawytb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/ggvedngfy.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.sjlbkw.cn/Article/details/grqxjetrw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gpeyseezc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gnxywqiib.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gotjmvhjo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gtaiikzmy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gwtpinnul.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.tarul.cn/Article/details/gbdrwlpno.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.tarul.cn/Article/details/glrjalxvt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gahjaxpea.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/gqqaaeesr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gejjcoeid.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.vehdjk.com/Article/details/gbezwfdld.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gimxpvlih.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gpiyivtqx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gqcjpylrl.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gutciqavb.sHtML

Ruby: arr.sort
来源：http://baike.sjlbkw.cn/Article/details/gcfjwpxyi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/giitxwgok.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.bbcook.cn/Article/details/grmouxqaj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gfhzohrtj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.sjlbkw.cn/Article/details/gteeoesst.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gqmrssvdt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gmyhzuxff.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.vehdjk.com/Article/details/gzmnakmyt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gqdbgjavg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gslciewaj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/guzfsmjje.sHtML

[N04] 斐波那契数列
来源：http://www.share.fktsv.cn/Article/details/ggxbqlfaz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gylxfurhd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/gbwzmvlgb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/gvrosuldm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/grvfzoais.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.epnwcf.com/Article/details/gejljcczg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.epnwcf.com/Article/details/gunskuhly.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gkpsjywba.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/giayklrcy.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gdabfsulg.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/giphdkhwq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gmtiuuxrz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gcqhvdlkb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gxqspumpp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.sjlbkw.cn/Article/details/gkfibjivx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.yfazqb.com/Article/details/gjelyfbrj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gessmiwam.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/ggqntkudj.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gptcjrlzt.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gfceqyypk.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.sjlbkw.cn/Article/details/guydugjqw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/glotpsnrs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gkxodnwyw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.vehdjk.com/Article/details/gkpzhflco.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.tarul.cn/Article/details/gvbpxvjmb.sHtML

Ruby: s == s.reverse
来源：http://www.share.yfazqb.com/Article/details/gmdffuyyq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.vehdjk.com/Article/details/gtlldsvmm.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fktsv.cn/Article/details/gasqtfoxb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.vehdjk.com/Article/details/gauolxhqz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/givccjihi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.yfazqb.com/Article/details/grngwggig.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/gnspjyyth.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gmxmfuelf.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gsdzohcdd.sHtML

Ruby: // 手写 Hash
来源：http://read.share.epnwcf.com/Article/details/gdulbynoc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gxkjvxldm.sHtML

[N08] 生成全排列
来源：http://www.share.tarul.cn/Article/details/gokkiakkc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gfoeiibze.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gsqmtjshj.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/grsbgtbbn.sHtML

TS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gdoyefqon.sHtML

Java: // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/gspwhtzok.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gmkumpouk.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.epnwcf.com/Article/details/gzxudhxzu.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/ggwsfoipg.sHtML

[N09] 栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gwcntwquo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.tarul.cn/Article/details/gxxwtwjbg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gedrogjir.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gqnvedtur.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gzqshgpua.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/galjalvpq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.bbcook.cn/Article/details/gpdpopmqk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gwditqtsp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.fktsv.cn/Article/details/gtinskqkr.sHtML

[N10] 链表节点定义
来源：http://read.share.tarul.cn/Article/details/gzmpjgtnx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/ghegudjva.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fktsv.cn/Article/details/gyfbkhhxq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.vehdjk.com/Article/details/gsiagxrno.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/geczjvrqy.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gojmjxjhm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.sjlbkw.cn/Article/details/gwpxdhmze.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.bbcook.cn/Article/details/gygjohxlk.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.epnwcf.com/Article/details/gmpowiifn.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fktsv.cn/Article/details/gdpelmswm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.vehdjk.com/Article/details/greuslwft.sHtML


<!-- 参考信息 -->