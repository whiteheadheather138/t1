代发 wailian999

TS:   JSON.parse(s)
来源：http://blog.vehdjk.com/Article/details/gpjtkhaei.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fktsv.cn/Article/details/gwaubqdax.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fktsv.cn/Article/details/gyolpdcwo.sHtML

Ruby: JSON.parse(s)
来源：http://baike.vehdjk.com/Article/details/gvowffdlc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.vehdjk.com/Article/details/gwkmnzrwi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.tarul.cn/Article/details/glhdkvvfw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.tarul.cn/Article/details/gwsvrhbye.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.sjlbkw.cn/Article/details/giouztahp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjadlyxuq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.bbcook.cn/Article/details/gymjnnhhl.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.tarul.cn/Article/details/gczzcxhsd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.bbcook.cn/Article/details/gufkradht.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.yfazqb.com/Article/details/grvepbnsb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fktsv.cn/Article/details/gbimxcqiz.sHtML

[K04] 读取 JSON 文件
来源：http://wap.vehdjk.com/Article/details/gcovufvfi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gbzqvgqyy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.sjlbkw.cn/Article/details/gawbpvfqo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fktsv.cn/Article/details/gpbfbalnn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.tarul.cn/Article/details/gkyuhqomt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.yfazqb.com/Article/details/glrfdhzyf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.epnwcf.com/Article/details/gnexoaisb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gvegjocat.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.sjlbkw.cn/Article/details/gjkplpxie.sHtML

[K05] 深拷贝对象
来源：http://www.share.sjlbkw.cn/Article/details/gurjeitoz.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.sjlbkw.cn/Article/details/grpfknsxr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.vehdjk.com/Article/details/gifdbfwku.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gwclymmcm.sHtML

TS:   structuredClone(obj)
来源：http://baike.sjlbkw.cn/Article/details/glnuahqpa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.yfazqb.com/Article/details/gaamkstuf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.yfazqb.com/Article/details/gxlvpaagf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fktsv.cn/Article/details/ghlxgohce.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fktsv.cn/Article/details/geeropbii.sHtML

[K06] 解析 URL 查询串
来源：http://wap.yfazqb.com/Article/details/gqtlfeqfy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.epnwcf.com/Article/details/gbqrbsyty.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.epnwcf.com/Article/details/gtqmpsysu.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gfpyjesqt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.yfazqb.com/Article/details/gigzivalu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.yfazqb.com/Article/details/guxqgswzb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.sjlbkw.cn/Article/details/gxekxhjzn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.bbcook.cn/Article/details/gmzhjblos.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fktsv.cn/Article/details/gaogzcupg.sHtML

[K07] 进制转换
来源：http://mobile.yfazqb.com/Article/details/gjmebymlm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.sjlbkw.cn/Article/details/gikexbqti.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.epnwcf.com/Article/details/gkysinfgi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.yfazqb.com/Article/details/gsbakuxcv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.bbcook.cn/Article/details/gqzpndegw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.epnwcf.com/Article/details/gyyfxqmsm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gembzdabz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fktsv.cn/Article/details/gdmdvense.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fktsv.cn/Article/details/golzznxkw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.epnwcf.com/Article/details/gwelqxeas.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.vehdjk.com/Article/details/gqczsvbpb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.bbcook.cn/Article/details/gifdwctgr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.sjlbkw.cn/Article/details/gxgchrjqz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.tarul.cn/Article/details/gwmuzwxcn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.vehdjk.com/Article/details/gavkwkriq.sHtML

Go:   encoding/gob
来源：http://baike.sjlbkw.cn/Article/details/guhgkskor.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.sjlbkw.cn/Article/details/gvswgmdim.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gxxciiytv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/guvomnyeh.sHtML

L. 网络请求
来源：http://blog.vehdjk.com/Article/details/gvrxzxuql.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gqotwxare.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.epnwcf.com/Article/details/ghzggdnpf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gmmorvupr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fktsv.cn/Article/details/ghojyklhz.sHtML

JS:   await fetch(url)
来源：http://www.blog.tarul.cn/Article/details/gbuxxtelz.sHtML

TS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gfsownepj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gusgdtgcf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.epnwcf.com/Article/details/ginoewrxu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.tarul.cn/Article/details/giwiiyeht.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gxzyszimm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gsmsnbgpk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fktsv.cn/Article/details/gmhjvtwch.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gymhibbny.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.bbcook.cn/Article/details/gtrljssfl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.yfazqb.com/Article/details/gnxfcsnjx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzqvufsx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gptolaqkb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fktsv.cn/Article/details/gkrzehecu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.tarul.cn/Article/details/gavkpesdm.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fktsv.cn/Article/details/gbzpvkvnm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/galupyjrq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.vehdjk.com/Article/details/gqswqbyyf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.yfazqb.com/Article/details/gwimvzvdk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/gpfzvrzof.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/guhxmrmgv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gcissjtfa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.tarul.cn/Article/details/gqcwqxcno.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.bbcook.cn/Article/details/gocyyimbm.sHtML

[L04] 设置超时
来源：http://www.share.fktsv.cn/Article/details/gaisbjhes.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.epnwcf.com/Article/details/gacayyuiu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.bbcook.cn/Article/details/gxshjaeqf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.epnwcf.com/Article/details/gkvnehcci.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.yfazqb.com/Article/details/gaiiloair.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.epnwcf.com/Article/details/gwvvbwuqy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.bbcook.cn/Article/details/gowyruxhl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.yfazqb.com/Article/details/gvciowivk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.vehdjk.com/Article/details/grwjcnlcj.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.vehdjk.com/Article/details/gmkgzpzir.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.vehdjk.com/Article/details/ggpoiwuaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.vehdjk.com/Article/details/gvwlpdjww.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gugukcqfm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gnsggnyyc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.yfazqb.com/Article/details/grkdsmdor.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fktsv.cn/Article/details/goglbfvwh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gerstetmb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.vehdjk.com/Article/details/gjgwdmjrm.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/gfksdweof.sHtML

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/gcdqxvjsy.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fktsv.cn/Article/details/gherdxmoi.sHtML

JS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gsibxkobp.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gqitweema.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gtdlcekqp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gwpnrgazd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.tarul.cn/Article/details/ggiixjqvh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.bbcook.cn/Article/details/grpzaxvtj.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gpdlatmtf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.sjlbkw.cn/Article/details/gkwhmdpua.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.bbcook.cn/Article/details/goiwjglhe.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gfwlbuynt.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/grbizyyrw.sHtML

Java: resp.statusCode()
来源：http://www.blog.fktsv.cn/Article/details/gqrxzfynp.sHtML

Go:   resp.StatusCode
来源：http://www.blog.vehdjk.com/Article/details/gxwuwuquu.sHtML

Ruby: resp.code.to_i
来源：http://mobile.tarul.cn/Article/details/ghjzoahro.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/gajrtgigw.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gwpllzcno.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.yfazqb.com/Article/details/gsuifgpds.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/gqnxakbbp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.sjlbkw.cn/Article/details/gqkhstikr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gosbtdlqs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.yfazqb.com/Article/details/ggamgnbep.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.epnwcf.com/Article/details/gtrjtzpzm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gnqwiyjps.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gccyhwjrw.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gwxavmweu.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fktsv.cn/Article/details/gitqvraxi.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gjiwasbmu.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gxmvddwon.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.epnwcf.com/Article/details/ghgakafpl.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gghnjoyzp.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gdzykoenh.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gpzfgtkqh.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.vehdjk.com/Article/details/giggfzdtf.sHtML

Go:   os.Args[1:]
来源：http://3g.vehdjk.com/Article/details/gxgtoclkp.sHtML

Ruby: ARGV
来源：http://www.share.fktsv.cn/Article/details/goqznbmke.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gbelocdmu.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gntsdbalb.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gogoxgdnu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/goappqzej.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gpbxtxvoy.sHtML

TS:   process.env.HOME
来源：http://read.share.fktsv.cn/Article/details/gpqzazuob.sHtML

Java: System.getenv("HOME")
来源：http://baike.tarul.cn/Article/details/gldaugvls.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gejskutar.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.epnwcf.com/Article/details/gorlibmli.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gksivhrpc.sHtML

[M03] 执行外部命令
来源：http://wap.tarul.cn/Article/details/ghlbzkmfq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/ggguexeko.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gbblrxsji.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gezpwlqsk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gnrvtazsu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.epnwcf.com/Article/details/gqfdopbjo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/guowfcbmc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.sjlbkw.cn/Article/details/gvbqwyrup.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fktsv.cn/Article/details/gglyqzecj.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/gubafkytw.sHtML

Py:   os.getcwd()
来源：http://wap.yfazqb.com/Article/details/gslqostja.sHtML

PHP:  getcwd();
来源：http://baike.yfazqb.com/Article/details/gphgqcesn.sHtML

JS:   process.cwd()
来源：http://wap.vehdjk.com/Article/details/gryohikbx.sHtML

TS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvouhlpd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gnozssctr.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gakeyaxgg.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gdgvwdagc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fktsv.cn/Article/details/gpwrexgow.sHtML

[M05] 设置退出码
来源：http://blog.tarul.cn/Article/details/gajmjdqft.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gzdrxahpu.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gtomqkexp.sHtML

JS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gbtyjmavz.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gtbzgeqjq.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gpuihybpa.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gbyytjzah.sHtML

Ruby: exit 1
来源：http://www.blog.epnwcf.com/Article/details/grxheelom.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gskmvwbur.sHtML

[M06] 向标准错误输出
来源：http://baike.epnwcf.com/Article/details/gmdqpsnzw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/goepevycs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/gnvqjzeid.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gndeshrdx.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gojravskd.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gmvhiujog.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gbtnadjba.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gleqylutz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwozytazo.sHtML

[M07] 判断是否为主入口
来源：http://3g.fktsv.cn/Article/details/goksngejp.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.bbcook.cn/Article/details/gpavtdjde.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/ghqxrfcsw.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gdcdsxgnx.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/gnfiodwww.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gpdelqhpm.sHtML

Go:   func main()
来源：http://www.share.epnwcf.com/Article/details/gufdmcowl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.epnwcf.com/Article/details/genftpoox.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.sjlbkw.cn/Article/details/gemwtfrre.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/gxcfwdapf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fktsv.cn/Article/details/gfwaadpyt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.vehdjk.com/Article/details/gctsghyfk.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fktsv.cn/Article/details/gbuoetkao.sHtML

TS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gwnwupiqk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/gqthmorsc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gmjaunmoo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gquzkhzps.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/gweyylkcz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gxxpnbwbm.sHtML

N. 数据结构与算法
来源：http://3g.yfazqb.com/Article/details/gexqoqrid.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gqyihfirt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gtbdnqwhk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gsslbddcm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/gkgmqpnig.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/ggfkdpcsw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gggnvudpf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gkarjuzmv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gdyqmkedt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/ghrkudykz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gseqirozo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/gvgdahsnj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.epnwcf.com/Article/details/gklofffrq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.fktsv.cn/Article/details/gzjjewazw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gmnsmkifs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gskffhksf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gupjmszpq.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gkfmffmul.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gcttsnswm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gtrhiefup.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gfvzhplut.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gigwsvdky.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/ghsynmxbc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/girnqempp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/gwxcfxszo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.tarul.cn/Article/details/gelqwznuw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.epnwcf.com/Article/details/gevcumehr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gcrhyikth.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gpoubviwg.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.bbcook.cn/Article/details/glbkzncsm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/gwdvzibvb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.epnwcf.com/Article/details/ggdhahbsc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.epnwcf.com/Article/details/gghisfkww.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gfoclnred.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gwbfiquwb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.vehdjk.com/Article/details/gwjwolcet.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gnhjdkwfb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gqaogvegh.sHtML

[N05] 最大公约数
来源：http://3g.bbcook.cn/Article/details/gtmnnnxxk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gucmeoyco.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/gdfbadpda.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gzqcqkfre.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gltvrvbkf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.tarul.cn/Article/details/gvmktlkma.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/gqtaymzha.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/ghtvpwuwm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gslkydueb.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/garnutfkn.sHtML

Py:   s == s[::-1]
来源：http://baike.epnwcf.com/Article/details/gggveexrh.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gnptandgh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gsllircsi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/glddlhufs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gxniyanpj.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gkuhetzrq.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/gwfnmkbtg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/grxwykpjj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.sjlbkw.cn/Article/details/gofweglde.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gmcvgvlcy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gunjihgxt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/gxqjcihjx.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.epnwcf.com/Article/details/grbsfhyks.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.epnwcf.com/Article/details/gnyozsugv.sHtML

Go:   // 手写 map[int]int
来源：http://blog.vehdjk.com/Article/details/gujxchnan.sHtML

Ruby: // 手写 Hash
来源：http://3g.fktsv.cn/Article/details/gtymuxbnj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gtqzevbkz.sHtML

[N08] 生成全排列
来源：http://www.m.share.tarul.cn/Article/details/godebkhyp.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gnoacqtec.sHtML

PHP:  // 手写递归交换
来源：http://www.share.epnwcf.com/Article/details/gwwewtgup.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gtvwuioun.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/geiwsatyd.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/guaijgclc.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/guvipdpav.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.yfazqb.com/Article/details/gaacouchc.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/ghnuplbdz.sHtML

[N09] 栈与队列
来源：http://www.blog.yfazqb.com/Article/details/gnkgslwcb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gataftjlf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gnznlupyc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gxmvozumd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gzrlpblnz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gzwcwacth.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.epnwcf.com/Article/details/gjxzjppyh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.tarul.cn/Article/details/grkgcsiiv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fktsv.cn/Article/details/gwrwnrarq.sHtML

[N10] 链表节点定义
来源：http://www.m.share.tarul.cn/Article/details/gwggacpoa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gbbofqnxv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.vehdjk.com/Article/details/gduogxtol.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/gxdyibrnk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gruadcypl.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gtncggcrc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.yfazqb.com/Article/details/gqtjwhzdf.sHtML


<!-- 参考信息 -->