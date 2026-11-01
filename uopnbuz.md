代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fktsv.cn/Article/details/gslsoinuy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.sjlbkw.cn/Article/details/gnmcajxft.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.vehdjk.com/Article/details/gaqsehaom.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.epnwcf.com/Article/details/ghlpuwaua.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.yfazqb.com/Article/details/gbbgneesf.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.vehdjk.com/Article/details/gdxebmxwx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.tarul.cn/Article/details/gkeztunvp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fktsv.cn/Article/details/ggnpqmfha.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.epnwcf.com/Article/details/genjintbi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fktsv.cn/Article/details/gwpbygzdv.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fktsv.cn/Article/details/gkvdvwmzf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.bbcook.cn/Article/details/ggamvshpe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.bbcook.cn/Article/details/gwtplawhe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.sjlbkw.cn/Article/details/gatntbgnb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.bbcook.cn/Article/details/ghnibbspi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fktsv.cn/Article/details/gzbsqiaum.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fktsv.cn/Article/details/gbqmmfemd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.vehdjk.com/Article/details/ghcyteybm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.sjlbkw.cn/Article/details/gccyckicb.sHtML

[K05] 深拷贝对象
来源：http://m.share.bbcook.cn/Article/details/ggfqsmigf.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.epnwcf.com/Article/details/gtqpebgih.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.epnwcf.com/Article/details/gcomuhrsk.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fktsv.cn/Article/details/gbsahihot.sHtML

TS:   structuredClone(obj)
来源：http://read.share.sjlbkw.cn/Article/details/gygbvlprc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.yfazqb.com/Article/details/gvuydcuaq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.bbcook.cn/Article/details/gqembufbv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.vehdjk.com/Article/details/gmugtefjr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.tarul.cn/Article/details/gzzvyitek.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.yfazqb.com/Article/details/gtcxvybwu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fktsv.cn/Article/details/ghvabvmcb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.epnwcf.com/Article/details/gtzcwzzka.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.vehdjk.com/Article/details/gtqifxenw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.tarul.cn/Article/details/gqoywoxwc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.epnwcf.com/Article/details/gsdfsjbwg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.sjlbkw.cn/Article/details/gzirqopoj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gqmctwivr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gqcibvfls.sHtML

[K07] 进制转换
来源：http://read.share.bbcook.cn/Article/details/gbzwuranp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/gyswjkwql.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.yfazqb.com/Article/details/gcfmwtiva.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/grlxsvqlh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gfrtjdmri.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.tarul.cn/Article/details/gsazpwbpd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.tarul.cn/Article/details/gfgzldyni.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gfskaavtz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.sjlbkw.cn/Article/details/gnwxxzdao.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fktsv.cn/Article/details/gzvqfojzc.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.bbcook.cn/Article/details/gopiwbhiq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gqwxcnrvs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fktsv.cn/Article/details/gmjilcxtp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/gtolhmjhl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.epnwcf.com/Article/details/glbwnqocf.sHtML

Go:   encoding/gob
来源：http://wap.vehdjk.com/Article/details/gqeebdexx.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.sjlbkw.cn/Article/details/gwmpptsgv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fktsv.cn/Article/details/garqikuyy.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gxpbggpjb.sHtML

L. 网络请求
来源：http://mobile.fktsv.cn/Article/details/gzcwbybvz.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gbcjhlxtn.sHtML

[L01] 发送 GET 请求
来源：http://m.share.vehdjk.com/Article/details/gscluqgtg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.bbcook.cn/Article/details/grfatpzdl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.bbcook.cn/Article/details/gdtflutzu.sHtML

JS:   await fetch(url)
来源：http://3g.epnwcf.com/Article/details/gitftllmr.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/ggzfhevac.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.yfazqb.com/Article/details/giedfmswq.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fktsv.cn/Article/details/gseigjonv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/gxxztadqr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gwksrtmjo.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.epnwcf.com/Article/details/gqaxphftu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gjhwactdd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gdilgqwlv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.yfazqb.com/Article/details/gaixerrya.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.tarul.cn/Article/details/ggenytztw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.bbcook.cn/Article/details/gvfyehyvb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fktsv.cn/Article/details/ghhursaya.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.yfazqb.com/Article/details/gvvleyeup.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.vehdjk.com/Article/details/gxtwqdxkx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gstrihash.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.vehdjk.com/Article/details/ghxcwwirp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/gfknrblhz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.sjlbkw.cn/Article/details/gjojkvzfo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.sjlbkw.cn/Article/details/gawgnfbba.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gfnfisksb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.epnwcf.com/Article/details/gptmdjjtw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fktsv.cn/Article/details/gfitrngne.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gxufddmtp.sHtML

[L04] 设置超时
来源：http://baike.bbcook.cn/Article/details/gfjrumzwa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.vehdjk.com/Article/details/ghoxprxff.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.epnwcf.com/Article/details/gluxktquc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.sjlbkw.cn/Article/details/gixnupwix.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gbpxmynjj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.vehdjk.com/Article/details/gweynsrqh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.sjlbkw.cn/Article/details/goktzodtg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fktsv.cn/Article/details/gsjrkuomy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.sjlbkw.cn/Article/details/ghwpbcitr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.sjlbkw.cn/Article/details/grlclmrme.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.yfazqb.com/Article/details/gvnyoqyol.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.bbcook.cn/Article/details/gdlxmkowm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.yfazqb.com/Article/details/gcoaguejj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gquikhwwq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.sjlbkw.cn/Article/details/gvhbwfioj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbocpsji.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/gzwvwppvy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/gatxlzika.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.vehdjk.com/Article/details/ghruifowr.sHtML

Py:   resp.json()
来源：http://read.share.bbcook.cn/Article/details/gbttsqniw.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/grvhzadkq.sHtML

JS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gmxhyohxg.sHtML

TS:   await resp.json()
来源：http://mobile.epnwcf.com/Article/details/gqawurlro.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.sjlbkw.cn/Article/details/gptyrxrvv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.epnwcf.com/Article/details/gwlddsnnb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.epnwcf.com/Article/details/gurcacbxj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gvhjdrzcg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/gepsqzfzy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.tarul.cn/Article/details/gpjkqhiug.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.yfazqb.com/Article/details/glfxadjhj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fktsv.cn/Article/details/ggqwfayiy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fktsv.cn/Article/details/gvrloeqpu.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/gkyzwmriz.sHtML

Go:   resp.StatusCode
来源：http://m.share.yfazqb.com/Article/details/gxxptmsuj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gygwsaeuw.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.epnwcf.com/Article/details/gggfisexk.sHtML

[L08] 并发请求多个地址
来源：http://www.share.yfazqb.com/Article/details/gyzneydbq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.tarul.cn/Article/details/gjweinqxe.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.vehdjk.com/Article/details/gdncsymqt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gxejmowak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gngssxjzg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.vehdjk.com/Article/details/gojfqlzsq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.sjlbkw.cn/Article/details/grltfgpvp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/geayugkas.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/grdgiojyz.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/guxqhqjua.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gpwjgdoor.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gaxhongsb.sHtML

[M01] 读取命令行参数
来源：http://blog.yfazqb.com/Article/details/gssesrhib.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fktsv.cn/Article/details/gynijjsny.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/gtmghafap.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/gbczmwxsj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gxftizjup.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/gdvkiqnaz.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gxavusapp.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/ggdqtyyja.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.tarul.cn/Article/details/gcypkgzgz.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/gvakybqdf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/giyrqlkik.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gnzyxflzp.sHtML

JS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/gwmcqvkdv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gccrdatlh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gfunkgupj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.tarul.cn/Article/details/gcrknqqgt.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fktsv.cn/Article/details/gcadedxxv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.vehdjk.com/Article/details/grdepwtnr.sHtML

[M03] 执行外部命令
来源：http://read.share.sjlbkw.cn/Article/details/gubxcwnis.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.epnwcf.com/Article/details/gomttthre.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.epnwcf.com/Article/details/gghbnarqu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gfnfsqhpt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gnkanwuyz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/geaqqqaff.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/glnkoiagx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/galzznhsb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/gmnacyecr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fktsv.cn/Article/details/gmxdnrasq.sHtML

Py:   os.getcwd()
来源：http://read.share.epnwcf.com/Article/details/gjkgugakv.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gfjmifrkx.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gemmhaptg.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gqtvomefh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.yfazqb.com/Article/details/gtrkpsaos.sHtML

Go:   os.Getwd()
来源：http://www.share.fktsv.cn/Article/details/gighzuwil.sHtML

Ruby: Dir.pwd
来源：http://m.share.bbcook.cn/Article/details/gvmruuqsz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fktsv.cn/Article/details/gdwtgxsyk.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gcqjvgmyf.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gbjkndbkz.sHtML

PHP:  exit(1);
来源：http://blog.vehdjk.com/Article/details/gczcrvgcx.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gqnjtubut.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/ggvdnxvkr.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gxemmuega.sHtML

Go:   os.Exit(1)
来源：http://read.share.fktsv.cn/Article/details/geljoxikm.sHtML

Ruby: exit 1
来源：http://www.share.sjlbkw.cn/Article/details/gaawncjmj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/giqmvmndx.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gjptpepvu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.bbcook.cn/Article/details/gcotjxhoh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.vehdjk.com/Article/details/gyagxdrzm.sHtML

JS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/gcilpvvad.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gikegalax.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gpiklhmqq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/ggpeehpth.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/ggnonjtck.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gtpirnurj.sHtML

[M07] 判断是否为主入口
来源：http://baike.tarul.cn/Article/details/gefhdepqg.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gjyvbjywh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.sjlbkw.cn/Article/details/gpvrelmfr.sHtML

JS:   require.main === module
来源：http://m.share.bbcook.cn/Article/details/gwalnmbdr.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gtvkllozo.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/glepxxang.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/gyqxnyiiz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gfbbawcgy.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.epnwcf.com/Article/details/gkzaybpbc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/ghpweqoaf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gkqavzadq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.yfazqb.com/Article/details/gnkfwbavb.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.sjlbkw.cn/Article/details/gafycjfvr.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/goayfnrci.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gnxlpnqml.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.epnwcf.com/Article/details/gyvrmmxeh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.yfazqb.com/Article/details/gzpiaoopr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/gbsdpmjdu.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/glmbfqzzh.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/gsnawwfyp.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gtlhpedfe.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gjyyhjsli.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gknvcqzco.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gnvpudekc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/grzjhpbta.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gbevdlzgt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gldnlzkhg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gadxkmepr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/gmalowvrt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fktsv.cn/Article/details/grtjjeedw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.yfazqb.com/Article/details/ggzoazxiy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.tarul.cn/Article/details/gxtvuekip.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gkgrtjkkk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gbwiqhxyt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gmlggeimd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/gmjxwibya.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.yfazqb.com/Article/details/gcqujnlmk.sHtML

Ruby: arr.sort
来源：http://m.share.fktsv.cn/Article/details/geijnabvi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/gmwkgyodw.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/grmgfczvj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxypapij.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gmqduiaiw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/glmftzpcm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gxmtvhisn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.bbcook.cn/Article/details/gckomfszo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.bbcook.cn/Article/details/gpxpdqglj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/gtkswusbb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.sjlbkw.cn/Article/details/ggrwpswmd.sHtML

[N04] 斐波那契数列
来源：http://baike.vehdjk.com/Article/details/gsbfctkzg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gtkdenger.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gumsjebag.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gnliavbvh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/ggqrnnqsy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gtxsnjmzv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/gdosqntpx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gbrxkzuco.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/grepltrmk.sHtML

[N05] 最大公约数
来源：http://3g.epnwcf.com/Article/details/goocrtcyh.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.epnwcf.com/Article/details/gvugynfkt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gqetjrurl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gbodwhcaf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.vehdjk.com/Article/details/ghwinnmlh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fktsv.cn/Article/details/gvrdlatie.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.bbcook.cn/Article/details/glxqsxvjw.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/gjsjaqihu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/goxxhomzh.sHtML

[N06] 判断回文字符串
来源：http://m.share.tarul.cn/Article/details/grsferxfe.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gberczgsf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gekphbbzh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/grhsrvnjh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gxdpyapzq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fktsv.cn/Article/details/gfyqrhwgl.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/glokwqnlf.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/gagtjtprb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.epnwcf.com/Article/details/gawakqtgc.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gqrxvgeaa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gjqarztlv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.bbcook.cn/Article/details/ghunxxmsu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.bbcook.cn/Article/details/ghkgbqrca.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.sjlbkw.cn/Article/details/gnjgcbcnq.sHtML

Java: // 手写 HashMap
来源：http://m.share.sjlbkw.cn/Article/details/gvmtuizli.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.tarul.cn/Article/details/gmxtsnfls.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/gwzttpulg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gjtvzgzyf.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/ghdtruhot.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/gejgyfiqk.sHtML

PHP:  // 手写递归交换
来源：http://read.share.tarul.cn/Article/details/gmgsprncx.sHtML

JS:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gbqeddvzq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/giiaojzkd.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gngjkqild.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gkgqkebuw.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/golhamqnu.sHtML

C#:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gcaoxcvvz.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/gueodiefl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gmtakxvgw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.fktsv.cn/Article/details/gguijahdf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gskguvcug.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/ghedogdia.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.epnwcf.com/Article/details/gdmublaci.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.vehdjk.com/Article/details/gghifrgvp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/glpmhabln.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gdcyrhoix.sHtML

[N10] 链表节点定义
来源：http://blog.epnwcf.com/Article/details/gezhrlrot.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/gfinzvmxe.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gwnjvzdym.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.bbcook.cn/Article/details/gnorknfmz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/geeiqxdib.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/gutjzzfup.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.bbcook.cn/Article/details/gwdhgywqy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.bbcook.cn/Article/details/gztedwzxj.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.tarul.cn/Article/details/gwodcismy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gqnyadhhq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/gauzysvko.sHtML


<!-- 参考信息 -->