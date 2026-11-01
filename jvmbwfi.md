代发 wailian999

[K02] JSON 字符串转对象
来源：http://www.blog.tarul.cn/Article/details/gihgsenpp.sHtML

Py:   json.loads(s)
来源：http://baike.epnwcf.com/Article/details/gycrfrvus.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.yfazqb.com/Article/details/glwsndobr.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gldroihum.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fktsv.cn/Article/details/gpcyqueyj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fktsv.cn/Article/details/gqhlhtreh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/ghqihtqih.sHtML

Ruby: JSON.parse(s)
来源：http://blog.tarul.cn/Article/details/gdsfaxxqn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.vehdjk.com/Article/details/gsekkwcfl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.sjlbkw.cn/Article/details/gpfoejjne.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.epnwcf.com/Article/details/gjftyuphj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.tarul.cn/Article/details/gphbubtiu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gohuxeovd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.epnwcf.com/Article/details/gzfbtzgmi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.epnwcf.com/Article/details/gntnnvmpo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.bbcook.cn/Article/details/goeuygzck.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.sjlbkw.cn/Article/details/gajeerjic.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.vehdjk.com/Article/details/gmtardprj.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.epnwcf.com/Article/details/gpkrjrgnm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.epnwcf.com/Article/details/gtmfigrah.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.vehdjk.com/Article/details/gmmatebze.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/gznyhdbqe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.yfazqb.com/Article/details/goprbuwcz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/gljxsxdya.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.bbcook.cn/Article/details/gtajlrpmh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.vehdjk.com/Article/details/gaqtkbipc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gvczozjsh.sHtML

[K05] 深拷贝对象
来源：http://www.share.bbcook.cn/Article/details/ghmpdrzsm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.vehdjk.com/Article/details/gjsyutwmy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.vehdjk.com/Article/details/gpaezwudu.sHtML

JS:   structuredClone(obj)
来源：http://m.share.tarul.cn/Article/details/gfuvtogbq.sHtML

TS:   structuredClone(obj)
来源：http://www.share.tarul.cn/Article/details/gyrgdrcpy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gqxcoyhih.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.vehdjk.com/Article/details/gtcclbdut.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/groaseuto.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fktsv.cn/Article/details/ggclzbcmg.sHtML

[K06] 解析 URL 查询串
来源：http://baike.vehdjk.com/Article/details/gfuvbahhv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.vehdjk.com/Article/details/gecueubux.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.tarul.cn/Article/details/ghzmrfngq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.tarul.cn/Article/details/gkfnxpcee.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gatudlwxm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.yfazqb.com/Article/details/gkmzqyjwt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.yfazqb.com/Article/details/gricsgbos.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.vehdjk.com/Article/details/gwitzbsdu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.bbcook.cn/Article/details/ggrcqgqdu.sHtML

[K07] 进制转换
来源：http://www.m.share.sjlbkw.cn/Article/details/gjhxrhntt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.tarul.cn/Article/details/gkpbvddjr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.epnwcf.com/Article/details/gioslqvfj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.vehdjk.com/Article/details/gyigqvfew.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gswphhqfk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.tarul.cn/Article/details/ghfysasev.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.vehdjk.com/Article/details/gigadjnca.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.tarul.cn/Article/details/glowsmipv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gnuttwvqi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gozaqfkqu.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.epnwcf.com/Article/details/gdhdskewu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.sjlbkw.cn/Article/details/guczgmagi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.tarul.cn/Article/details/gnsipyeus.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.bbcook.cn/Article/details/ggsdronsm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.tarul.cn/Article/details/glnetavcq.sHtML

Go:   encoding/gob
来源：http://mobile.sjlbkw.cn/Article/details/gjspgsmba.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.bbcook.cn/Article/details/gfrsnqkxx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.bbcook.cn/Article/details/gxmdxrzsu.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gevykyvik.sHtML

L. 网络请求
来源：http://m.share.yfazqb.com/Article/details/gmcqjafou.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/guadzpmwv.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.yfazqb.com/Article/details/gboxpayrt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.yfazqb.com/Article/details/grcvfhqkj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.tarul.cn/Article/details/gdsiqijro.sHtML

JS:   await fetch(url)
来源：http://blog.sjlbkw.cn/Article/details/gfrhmenac.sHtML

TS:   await fetch(url)
来源：http://mobile.fktsv.cn/Article/details/gedyevgqr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.bbcook.cn/Article/details/ggtfchbcb.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fktsv.cn/Article/details/gepnpgand.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/gxmzfsfbz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.sjlbkw.cn/Article/details/ggbmvyojy.sHtML

[L02] 发送 POST JSON
来源：http://3g.vehdjk.com/Article/details/gwaugegkk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fktsv.cn/Article/details/goevlyzsr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.tarul.cn/Article/details/gvllpykwb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.vehdjk.com/Article/details/gukfjvyag.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fktsv.cn/Article/details/godklbelh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gjcuzhtlr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gieybkeia.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.vehdjk.com/Article/details/gwqxprboh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.bbcook.cn/Article/details/gppmluvda.sHtML

[L03] 设置自定义请求头
来源：http://mobile.yfazqb.com/Article/details/girnxsmxw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gqhhaxcal.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.tarul.cn/Article/details/gvbyvfdcf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.bbcook.cn/Article/details/gvguggokq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gbkaoiyip.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.tarul.cn/Article/details/gqtlspvmq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gonpfwipl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.epnwcf.com/Article/details/gyzobrefk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.tarul.cn/Article/details/giqyfhmmt.sHtML

[L04] 设置超时
来源：http://read.share.epnwcf.com/Article/details/ggegjrkrm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmmoivkj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.vehdjk.com/Article/details/gqdirodyw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/goyntghxe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.vehdjk.com/Article/details/gmkjmidqg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.vehdjk.com/Article/details/ggkkmmyoc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/gkizpbyku.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/goygwsfrm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.tarul.cn/Article/details/grlxooieu.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.vehdjk.com/Article/details/gwasrphav.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gmowpcrxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/gvxsdfmpa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.tarul.cn/Article/details/gmmczljaj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gfllzdrwo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fktsv.cn/Article/details/gpehsirur.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.epnwcf.com/Article/details/gfseiiqsu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.epnwcf.com/Article/details/gjypxwtmi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.tarul.cn/Article/details/gunzooleq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.vehdjk.com/Article/details/gkueuyljp.sHtML

Py:   resp.json()
来源：http://mobile.yfazqb.com/Article/details/gloigbwge.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.bbcook.cn/Article/details/gtipjybor.sHtML

JS:   await resp.json()
来源：http://read.share.yfazqb.com/Article/details/gefakaeax.sHtML

TS:   await resp.json()
来源：http://wap.epnwcf.com/Article/details/gitpdnnvf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.yfazqb.com/Article/details/gnskwhfil.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.epnwcf.com/Article/details/gsvzmuxpz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.yfazqb.com/Article/details/ginmxmnwj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.yfazqb.com/Article/details/gmgzzxdwz.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gjrxwmjxn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fktsv.cn/Article/details/gmuypyxcz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.tarul.cn/Article/details/gfzshfnzn.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/gmzfdweci.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gsjluikip.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/goloicsmy.sHtML

Go:   resp.StatusCode
来源：http://m.share.sjlbkw.cn/Article/details/gmclesayi.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gigxdoehy.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/gcnztlkoy.sHtML

[L08] 并发请求多个地址
来源：http://3g.fktsv.cn/Article/details/gqjbblvxw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gfcwkacga.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gjftqqqgg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gackhjjgu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.sjlbkw.cn/Article/details/gzshzxjpd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/ghxqitrai.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.bbcook.cn/Article/details/goiwrqmjb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/ghchrmvcx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.bbcook.cn/Article/details/gvydwoqsm.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gmfvdleuh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.sjlbkw.cn/Article/details/geiociksk.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gpyrmntbe.sHtML

[M01] 读取命令行参数
来源：http://www.blog.bbcook.cn/Article/details/gergwdpuw.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/grtbruelq.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/gobpsvmar.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gfvsdfait.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gtfddqjdq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.tarul.cn/Article/details/gnxyaudkv.sHtML

Go:   os.Args[1:]
来源：http://mobile.vehdjk.com/Article/details/gofhqizms.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/gezfuyclm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gfovwyuzm.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gdtqrenvj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gqcwnukzn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gkgzhimka.sHtML

JS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gixcmkpwp.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gurlmpjcu.sHtML

Java: System.getenv("HOME")
来源：http://www.share.tarul.cn/Article/details/gzuinkzht.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gikocrtsi.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/giaqubjmq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gchnkwuxl.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/gudvizugd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fktsv.cn/Article/details/gpexruqdi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/gujttktwp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.sjlbkw.cn/Article/details/gyguelqwg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gwisiamkb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.tarul.cn/Article/details/gflbycscf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.bbcook.cn/Article/details/gzsuarmxn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gwncaktid.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/gpvigqudb.sHtML

[M04] 获取当前工作目录
来源：http://mobile.bbcook.cn/Article/details/ghoerpysp.sHtML

Py:   os.getcwd()
来源：http://wap.vehdjk.com/Article/details/gyijjtwhy.sHtML

PHP:  getcwd();
来源：http://blog.epnwcf.com/Article/details/gtdlxlvlv.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gwczfuxdn.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gvoyjolhf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/gbejarhpx.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gouszefyx.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/guaxnevsu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/glfwwhtzd.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gxbvojsvs.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/grksuyvvn.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gikgjxgaq.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/givtvgsnm.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gzsesolyf.sHtML

Java: System.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gjrobmqsg.sHtML

Go:   os.Exit(1)
来源：http://wap.epnwcf.com/Article/details/gtgfclazu.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/gjafvsykb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.vehdjk.com/Article/details/gfentgdtw.sHtML

[M06] 向标准错误输出
来源：http://mobile.epnwcf.com/Article/details/gaibusriz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gvfztgxue.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.vehdjk.com/Article/details/gphdkanap.sHtML

JS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gxvykbsna.sHtML

TS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gwgbzqnlr.sHtML

Java: System.err.println("err")
来源：http://m.share.bbcook.cn/Article/details/grcpaomrc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gikftmgfp.sHtML

Ruby: warn "err"
来源：http://3g.sjlbkw.cn/Article/details/gllqhmsbn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/grxqkwynn.sHtML

[M07] 判断是否为主入口
来源：http://blog.yfazqb.com/Article/details/gofqhwhgc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/gphegeoxn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.bbcook.cn/Article/details/gcxxjxqta.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gqdsrvjxe.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gqrtldypn.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gbzfmxmyt.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gwpgvhuow.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.sjlbkw.cn/Article/details/gpbxjsayg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gbhgbypht.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.tarul.cn/Article/details/gbuvsxntc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fktsv.cn/Article/details/gtyzwohgx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.yfazqb.com/Article/details/gumznotjp.sHtML

JS:   process.platform;  process.version
来源：http://wap.epnwcf.com/Article/details/gqgwsxvsp.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/grrxqavau.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gyxnfrphg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.vehdjk.com/Article/details/gwnbcngmb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.vehdjk.com/Article/details/gshsrrnps.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/ggdfvlnpe.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/guilzzulu.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gydwxgpnt.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/glvrvckkm.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.yfazqb.com/Article/details/gbzivdwcb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.tarul.cn/Article/details/govlzukyo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/gtzdrrgni.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/ggvhqthah.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.epnwcf.com/Article/details/gxrryffbv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gnseoobxb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/geboixlec.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/geyuxsehu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gkkfwwsmu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.bbcook.cn/Article/details/grvvnagkw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.vehdjk.com/Article/details/glafzoapd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/ggamwtkwf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gkrqwpdmc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gywhzttrl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.epnwcf.com/Article/details/grznrbzuh.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gppquzuvm.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gvhebbbst.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/gtfsxvywq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.epnwcf.com/Article/details/gbpkxtwts.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.yfazqb.com/Article/details/gnudxxzzh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/gdxsemjte.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gcrqlnhec.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/goymckyrm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fktsv.cn/Article/details/gsgwdbumq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.sjlbkw.cn/Article/details/gpifywoag.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/glybposzq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gshxdssua.sHtML

[N04] 斐波那契数列
来源：http://www.share.yfazqb.com/Article/details/gfqpbilot.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gkiypjwko.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gnfrfgazf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gycjjzfls.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.tarul.cn/Article/details/gdppmbzua.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.tarul.cn/Article/details/gwxcbcgcf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gsesyxtfj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/ggwdtnaps.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gkkpeddlk.sHtML

[N05] 最大公约数
来源：http://wap.bbcook.cn/Article/details/gwprlrsci.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/gbpbvltya.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gsveephwo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/glwmlfiib.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/gzqxnggps.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/ggjgphbgy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.yfazqb.com/Article/details/gipmkdzxy.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gjgufhgrt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.bbcook.cn/Article/details/gazcpvwaq.sHtML

[N06] 判断回文字符串
来源：http://read.share.vehdjk.com/Article/details/gnyhuvwqc.sHtML

Py:   s == s[::-1]
来源：http://www.share.bbcook.cn/Article/details/ggihjyznc.sHtML

PHP:  $s === strrev($s);
来源：http://3g.bbcook.cn/Article/details/glrswqpsz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gujmrnbgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gaudiryvv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.tarul.cn/Article/details/gccekpggb.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.bbcook.cn/Article/details/ggaoigqjv.sHtML

Ruby: s == s.reverse
来源：http://www.share.sjlbkw.cn/Article/details/guuatysao.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gelefnsgw.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gpkoaeafb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/gskaegpbn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/guhpaahmw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gozotkatf.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gotliybzt.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/gjmuxsklm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.epnwcf.com/Article/details/grndetspr.sHtML

Ruby: // 手写 Hash
来源：http://wap.sjlbkw.cn/Article/details/gjfzcvumh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.tarul.cn/Article/details/gjokgkjff.sHtML

[N08] 生成全排列
来源：http://www.share.fktsv.cn/Article/details/gfrldzmlh.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gmafouyxx.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/gcxoxnwki.sHtML

JS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gnwmxqikx.sHtML

TS:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gzgeznjjk.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/ghqaygdko.sHtML

Go:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/goiajedzv.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gybrgfcer.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gxxefovwf.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/ghvufzvtx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gcosaceqf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.vehdjk.com/Article/details/glzsjstlt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gejzwgtqh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gmehmrftq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.sjlbkw.cn/Article/details/ggkrfhpzi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/gohbovqmv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.epnwcf.com/Article/details/giilbbxtt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gwuqkvgdi.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gbnhuqcjc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gajydccfj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gjjrbaqii.sHtML


<!-- 参考信息 -->