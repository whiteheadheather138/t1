代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.bbcook.cn/Article/details/grulutrxx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.sjlbkw.cn/Article/details/gwxycmihy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.tarul.cn/Article/details/guwakhygs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.vehdjk.com/Article/details/gdbfixwiu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.epnwcf.com/Article/details/gldoxknrk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fktsv.cn/Article/details/gmfbihjtg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.vehdjk.com/Article/details/gsiixiaup.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fktsv.cn/Article/details/gguxftshk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gzbprlgvq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/ggdutzuuy.sHtML

[K04] 读取 JSON 文件
来源：http://3g.tarul.cn/Article/details/gfgeibqsz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fktsv.cn/Article/details/gytlxmxca.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.yfazqb.com/Article/details/gmdyhqmki.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.epnwcf.com/Article/details/gnmvgghtk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.epnwcf.com/Article/details/gwmccijdr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.epnwcf.com/Article/details/gfpnaukxr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/glibhzhnr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.vehdjk.com/Article/details/gwgfqvkpo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gfahnvqqq.sHtML

[K05] 深拷贝对象
来源：http://m.share.epnwcf.com/Article/details/gocdsdpdk.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.yfazqb.com/Article/details/gfphsmtqb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.tarul.cn/Article/details/gxqzkjkyu.sHtML

JS:   structuredClone(obj)
来源：http://baike.bbcook.cn/Article/details/gacrvxaww.sHtML

TS:   structuredClone(obj)
来源：http://baike.tarul.cn/Article/details/ghzssixkh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.epnwcf.com/Article/details/gqbjpbroy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.bbcook.cn/Article/details/gaaeaobkc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fktsv.cn/Article/details/gradobqlg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fktsv.cn/Article/details/gciajcovs.sHtML

[K06] 解析 URL 查询串
来源：http://wap.vehdjk.com/Article/details/gqspaqjhz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.vehdjk.com/Article/details/gcprknoil.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.bbcook.cn/Article/details/ghwlfjbru.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gkjdxxcwb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.sjlbkw.cn/Article/details/gpkttahkd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.bbcook.cn/Article/details/gfogrlkfn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.yfazqb.com/Article/details/ggmqaxsyc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.tarul.cn/Article/details/ghsdjpzcl.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gmufwvpom.sHtML

[K07] 进制转换
来源：http://m.share.epnwcf.com/Article/details/grbnwwepn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gzfctljqh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.tarul.cn/Article/details/gwdsnfoxh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fktsv.cn/Article/details/guowqmnoy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gwivrkban.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.sjlbkw.cn/Article/details/gaqhjubhy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.bbcook.cn/Article/details/grjynwhjr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fktsv.cn/Article/details/gcjindsjy.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.tarul.cn/Article/details/gvmvcpnag.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.vehdjk.com/Article/details/gibwsruit.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fktsv.cn/Article/details/ghnywipuj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.tarul.cn/Article/details/gxjsszqfh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/geoykevvo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.bbcook.cn/Article/details/gxeotfkgr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.tarul.cn/Article/details/gbiygzkst.sHtML

Go:   encoding/gob
来源：http://read.share.tarul.cn/Article/details/gpfoxybrh.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.vehdjk.com/Article/details/gwbaeajsw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.sjlbkw.cn/Article/details/gztdbwrvl.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gbkwjmzmz.sHtML

L. 网络请求
来源：http://m.share.sjlbkw.cn/Article/details/gpfzohgok.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gudncmhec.sHtML

[L01] 发送 GET 请求
来源：http://m.share.sjlbkw.cn/Article/details/gzkcsskui.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.sjlbkw.cn/Article/details/gmdejhxdc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gfsynialj.sHtML

JS:   await fetch(url)
来源：http://blog.yfazqb.com/Article/details/gzwrjzhvz.sHtML

TS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gjhedrwym.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.yfazqb.com/Article/details/gtwbrphsd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.bbcook.cn/Article/details/gyrrcdryc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.yfazqb.com/Article/details/gbwzxtmtm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.vehdjk.com/Article/details/gjfaspqxj.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gkdvbxisg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.tarul.cn/Article/details/gjxichafj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.epnwcf.com/Article/details/gzradvmum.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gfxukhtwd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.bbcook.cn/Article/details/grbwgfhte.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.tarul.cn/Article/details/gkxzdjaha.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.yfazqb.com/Article/details/gmhnmjvoi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gejkkhenu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.epnwcf.com/Article/details/gexqjcwbp.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.vehdjk.com/Article/details/gxjxxcdnl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.bbcook.cn/Article/details/gkdkuqxvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.yfazqb.com/Article/details/gqzckfjqq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.sjlbkw.cn/Article/details/grxoxsrvn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.epnwcf.com/Article/details/ggsrkcrxr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.sjlbkw.cn/Article/details/gcxdovprt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.tarul.cn/Article/details/gglpocgog.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gwpqnncrc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.yfazqb.com/Article/details/gfufcmetb.sHtML

[L04] 设置超时
来源：http://wap.epnwcf.com/Article/details/gsrfbyoat.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fktsv.cn/Article/details/gkebcmygw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.sjlbkw.cn/Article/details/gkfoxjdil.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/glpmgwaep.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.tarul.cn/Article/details/glfybubho.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.yfazqb.com/Article/details/geuctrpkg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gfgynszjd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gpiyshlfk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/grnllpyfs.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gmxnhnuhk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.yfazqb.com/Article/details/gpzfjgitg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.epnwcf.com/Article/details/grrkuqtwn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.vehdjk.com/Article/details/gryqwdzwl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/gvblciizy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.tarul.cn/Article/details/gpxmzmwfq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/ggvwguqbw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.yfazqb.com/Article/details/gdqhfaptc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.tarul.cn/Article/details/gvvrwkeby.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fktsv.cn/Article/details/gzxaaxcdc.sHtML

Py:   resp.json()
来源：http://mobile.tarul.cn/Article/details/guxngswkx.sHtML

PHP:  json_decode($body, true);
来源：http://baike.epnwcf.com/Article/details/ggaybgjrg.sHtML

JS:   await resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gyazmynxl.sHtML

TS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/gvipqjvtv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gpppolsyx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gzvecqcvh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fktsv.cn/Article/details/gopqhkzkb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.yfazqb.com/Article/details/glcuuwoxu.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.vehdjk.com/Article/details/gepuvkzrs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fktsv.cn/Article/details/gdyxokggc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.epnwcf.com/Article/details/gjzsrprrm.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/geahoflsa.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/gnnbcidfq.sHtML

Java: resp.statusCode()
来源：http://www.m.share.sjlbkw.cn/Article/details/girrwffvg.sHtML

Go:   resp.StatusCode
来源：http://m.share.fktsv.cn/Article/details/gkrkbcbvk.sHtML

Ruby: resp.code.to_i
来源：http://wap.vehdjk.com/Article/details/gdwgskqii.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/grubwjvmm.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/gzrecjudt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fktsv.cn/Article/details/gouqeyuln.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.yfazqb.com/Article/details/gdbvmrcbu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gdsdaxpmo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gzjeesevf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.epnwcf.com/Article/details/ghtetxxuv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.vehdjk.com/Article/details/gicuupmfv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gqpbixzpa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.epnwcf.com/Article/details/gkahpnbyq.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/ghqnvwsfp.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.sjlbkw.cn/Article/details/gcozuhlxf.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/grgqudpbl.sHtML

[M01] 读取命令行参数
来源：http://mobile.tarul.cn/Article/details/gbnvuydha.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gqbqiabhk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gvctvoval.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/goqdtmdpy.sHtML

TS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gvapgdmez.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/ggqxhduwk.sHtML

Go:   os.Args[1:]
来源：http://read.share.bbcook.cn/Article/details/gzoxreqcs.sHtML

Ruby: ARGV
来源：http://mobile.yfazqb.com/Article/details/gdfujjvew.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gcuarfrio.sHtML

[M02] 读取环境变量
来源：http://baike.epnwcf.com/Article/details/gbdrgbogq.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gacveflge.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gevdvppwo.sHtML

JS:   process.env.HOME
来源：http://baike.epnwcf.com/Article/details/gjbepbwkj.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gymdpmkvs.sHtML

Java: System.getenv("HOME")
来源：http://baike.epnwcf.com/Article/details/gzyoqgbaj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gljahlvaf.sHtML

Ruby: ENV["HOME"]
来源：http://blog.epnwcf.com/Article/details/gslruvnph.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gsmnysqap.sHtML

[M03] 执行外部命令
来源：http://blog.sjlbkw.cn/Article/details/gjznanqhz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.tarul.cn/Article/details/gwspjmbgj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/guwggdvrh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gmogvfnls.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gtomfczfv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gsoyfmoes.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gvkoavsmh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gnxziqzde.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.vehdjk.com/Article/details/gaidwvmjj.sHtML

[M04] 获取当前工作目录
来源：http://baike.fktsv.cn/Article/details/gfdcxrrix.sHtML

Py:   os.getcwd()
来源：http://www.blog.fktsv.cn/Article/details/gcsrdushk.sHtML

PHP:  getcwd();
来源：http://read.share.yfazqb.com/Article/details/gjjcconwc.sHtML

JS:   process.cwd()
来源：http://3g.yfazqb.com/Article/details/gokfzpurl.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/grhkdnrys.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fktsv.cn/Article/details/gasikrbdu.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gtafytmrd.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/getjldkix.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gdyeqpxxn.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/ghbaweity.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gcglxvits.sHtML

PHP:  exit(1);
来源：http://3g.bbcook.cn/Article/details/gyfxyzbqp.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gkovdxnzr.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gcpttrdkr.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gbscuvtic.sHtML

Go:   os.Exit(1)
来源：http://wap.tarul.cn/Article/details/gqtqdmtlu.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gadipehlg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fktsv.cn/Article/details/gsrntwglu.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gvhcddmdr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.bbcook.cn/Article/details/ggqvucznq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.tarul.cn/Article/details/gklfryscc.sHtML

JS:   console.error("err")
来源：http://www.blog.vehdjk.com/Article/details/gbgqoalpy.sHtML

TS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gyddojsmp.sHtML

Java: System.err.println("err")
来源：http://m.share.yfazqb.com/Article/details/gwayihnrs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.yfazqb.com/Article/details/giyglsdnt.sHtML

Ruby: warn "err"
来源：http://www.blog.sjlbkw.cn/Article/details/grwrqjtgc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.vehdjk.com/Article/details/gwcgnmotf.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/gcqjjvnbu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.vehdjk.com/Article/details/gvngjbwrc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gxvavzezm.sHtML

JS:   require.main === module
来源：http://mobile.yfazqb.com/Article/details/glivovknn.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gtkfjppkm.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gwekwjndu.sHtML

Go:   func main()
来源：http://wap.fktsv.cn/Article/details/gakssrnaj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.epnwcf.com/Article/details/gdkrvorpl.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/gjnavqysq.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/gtfgqzfda.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gyjnovety.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/ggbywwthk.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gyuidgqzg.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/gklpaktvo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gxifgspzr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.vehdjk.com/Article/details/gfwtoulfq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.bbcook.cn/Article/details/gakjxvlha.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.yfazqb.com/Article/details/gcpipkwlx.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gepibhpzd.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gsnsfrovt.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/grnolsjov.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gxwndgvte.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gqzqjhtkn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/geffzxwcl.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gbznmuale.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gfaaktajo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/ghtrhmvtc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fktsv.cn/Article/details/gzftkygkd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gllvsmcat.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gxmmxlqic.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.bbcook.cn/Article/details/gbybfdslz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.tarul.cn/Article/details/giwzteebi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.epnwcf.com/Article/details/gfoktataq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gqcsfkidn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gzanubvgn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.epnwcf.com/Article/details/gniycrfcw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fktsv.cn/Article/details/gtzxdanrx.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gxkcvtdlj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.sjlbkw.cn/Article/details/gejprucci.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.sjlbkw.cn/Article/details/gylaamfyb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.bbcook.cn/Article/details/gkpwzzhnl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/glbtyrrml.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fktsv.cn/Article/details/gglkukzpg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gczdpacwd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gnzszwder.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.yfazqb.com/Article/details/ggutxkysl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.tarul.cn/Article/details/gpnrmedyo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/ggnrfnoay.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/gnftgulil.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/gcqvimiwc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/gxwmtinca.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gklqtydpx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gydobmjyd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gasvhgpms.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/gfrhiczda.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fktsv.cn/Article/details/ggsbbsdns.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gwuzdknrn.sHtML

[N05] 最大公约数
来源：http://www.m.share.tarul.cn/Article/details/gkyxxgmma.sHtML

Py:   math.gcd(a, b)
来源：http://3g.epnwcf.com/Article/details/ggdgofixo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fktsv.cn/Article/details/guniapmsu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gyxvgoajp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gykckhkin.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/gvvxfkujb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gogtzfjdc.sHtML

Ruby: a.gcd(b)
来源：http://3g.fktsv.cn/Article/details/gvmeftgzi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/gtwubdwxx.sHtML

[N06] 判断回文字符串
来源：http://wap.yfazqb.com/Article/details/gizfcfgpf.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gngvzqffj.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.epnwcf.com/Article/details/gobtbgxrh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gsizavfpi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/ghbzafysl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/gdubzxjrr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fktsv.cn/Article/details/govxcaual.sHtML

Ruby: s == s.reverse
来源：http://www.blog.vehdjk.com/Article/details/gcyzacxjo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fktsv.cn/Article/details/gqlfqzxos.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gecnvordm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/goirmzaes.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.vehdjk.com/Article/details/gyuwtmaky.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.yfazqb.com/Article/details/gfoopitpj.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.yfazqb.com/Article/details/gshrtkers.sHtML

Java: // 手写 HashMap
来源：http://3g.epnwcf.com/Article/details/gtcbzbrqw.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.bbcook.cn/Article/details/grsitytgk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gqrfnpbco.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gbqcqptkc.sHtML

[N08] 生成全排列
来源：http://blog.sjlbkw.cn/Article/details/gprdhyhuo.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.tarul.cn/Article/details/gllyvnmjq.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/gxdrabmob.sHtML

JS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gjhdeyyxm.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gqrspppsc.sHtML

Java: // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gpwfemwfy.sHtML

Go:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/ggywvvstu.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.vehdjk.com/Article/details/gjgcvsenp.sHtML

C#:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gnhntsqsn.sHtML

[N09] 栈与队列
来源：http://3g.fktsv.cn/Article/details/gdqjfwkdh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.sjlbkw.cn/Article/details/gdxxjhwhz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gmocxgwhm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gmltlvpsm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.epnwcf.com/Article/details/ggfgbkkzw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gfkiixiug.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/gyhooxmyd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/gmdradnhx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.vehdjk.com/Article/details/gpslykrlw.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/gwryarrms.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/glfipdshp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.epnwcf.com/Article/details/gdsajotct.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gzpmrcefd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.bbcook.cn/Article/details/geocpjwrs.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.bbcook.cn/Article/details/gamgwvkot.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.epnwcf.com/Article/details/ggabhehgj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.bbcook.cn/Article/details/ggtrofqxu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.epnwcf.com/Article/details/gtvuywndp.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.tarul.cn/Article/details/gqkwqmetg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.yfazqb.com/Article/details/ggdpiekku.sHtML


<!-- 参考信息 -->