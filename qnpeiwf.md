代发 wailian999

TS:   JSON.parse(s)
来源：http://read.share.epnwcf.com/Article/details/gxasddgao.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.yfazqb.com/Article/details/ggihhjhgp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.bbcook.cn/Article/details/gvnnhlipn.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.sjlbkw.cn/Article/details/gtamhqulz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.sjlbkw.cn/Article/details/gdevuaibr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.epnwcf.com/Article/details/gpwqrrkga.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.yfazqb.com/Article/details/gediwulrg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.tarul.cn/Article/details/grwbwusos.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fktsv.cn/Article/details/gvvziqavh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.epnwcf.com/Article/details/gldlbobmi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.vehdjk.com/Article/details/gjxlbqgfl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.tarul.cn/Article/details/gdgkhwhyu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.sjlbkw.cn/Article/details/gwigcewhw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.tarul.cn/Article/details/gedduejlb.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.vehdjk.com/Article/details/givzxabaf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.vehdjk.com/Article/details/gdqmaamko.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fktsv.cn/Article/details/gwubapiap.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.yfazqb.com/Article/details/gjgcngyze.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.epnwcf.com/Article/details/gfsvhvpbu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/gxqqshjoz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.yfazqb.com/Article/details/glvxkmgsx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.yfazqb.com/Article/details/ggxdttwpo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gqtxsviqt.sHtML

[K05] 深拷贝对象
来源：http://read.share.tarul.cn/Article/details/gvsngmwcs.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.tarul.cn/Article/details/gzpfrqmwj.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fktsv.cn/Article/details/gcprwoema.sHtML

JS:   structuredClone(obj)
来源：http://mobile.yfazqb.com/Article/details/gkrfrwqpi.sHtML

TS:   structuredClone(obj)
来源：http://mobile.tarul.cn/Article/details/glduudvdz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.sjlbkw.cn/Article/details/gvyomdeyu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.tarul.cn/Article/details/gswsnqtor.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.vehdjk.com/Article/details/grctczkxb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.vehdjk.com/Article/details/gyafeipob.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.sjlbkw.cn/Article/details/gtilfxqam.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gkpacvqgn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.sjlbkw.cn/Article/details/gumlpzkpp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.tarul.cn/Article/details/gopgxrtav.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.vehdjk.com/Article/details/gbbfnyzam.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.yfazqb.com/Article/details/grjexsjcn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.tarul.cn/Article/details/gpsbqyqap.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fktsv.cn/Article/details/gimwgfxdn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.vehdjk.com/Article/details/gtgjebzgi.sHtML

[K07] 进制转换
来源：http://mobile.sjlbkw.cn/Article/details/gqcmbhqbt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/ghepfbgpj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.epnwcf.com/Article/details/gglkrhcxb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.vehdjk.com/Article/details/gjiochrim.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.tarul.cn/Article/details/gexycynro.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.yfazqb.com/Article/details/gstqtvxfn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.tarul.cn/Article/details/gozwjvhxv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.vehdjk.com/Article/details/gergqkgcz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.bbcook.cn/Article/details/gnkamjofm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.sjlbkw.cn/Article/details/ggjujefvz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gubbrqurf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.vehdjk.com/Article/details/genxxnefs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fktsv.cn/Article/details/gmvgcoqjo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.bbcook.cn/Article/details/gppjatevq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.sjlbkw.cn/Article/details/ggasliodx.sHtML

Go:   encoding/gob
来源：http://blog.vehdjk.com/Article/details/gztoklfsq.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.yfazqb.com/Article/details/grdetquvw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.bbcook.cn/Article/details/gwbuwpcqo.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gulzqinog.sHtML

L. 网络请求
来源：http://read.share.tarul.cn/Article/details/gtzssexqn.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gvuavwawy.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.tarul.cn/Article/details/gubyqltfp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.epnwcf.com/Article/details/gvaqnkyei.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.sjlbkw.cn/Article/details/gohqhbmha.sHtML

JS:   await fetch(url)
来源：http://read.share.tarul.cn/Article/details/gkqtkvxed.sHtML

TS:   await fetch(url)
来源：http://m.share.fktsv.cn/Article/details/gxoiwcjel.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.yfazqb.com/Article/details/gkfvelvao.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.epnwcf.com/Article/details/gbifjikxq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.bbcook.cn/Article/details/glptauwir.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fktsv.cn/Article/details/godbnemoc.sHtML

[L02] 发送 POST JSON
来源：http://baike.fktsv.cn/Article/details/glbijvofq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gesokvits.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.vehdjk.com/Article/details/gbtzzdthr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gkvjsjwdo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.vehdjk.com/Article/details/gzhuntzga.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.tarul.cn/Article/details/gidyniubn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.tarul.cn/Article/details/gfrvkppze.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/ghvaauyyz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/gerbycqzy.sHtML

[L03] 设置自定义请求头
来源：http://mobile.tarul.cn/Article/details/gvldhefsu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.epnwcf.com/Article/details/gvjezrnvx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.tarul.cn/Article/details/gxveitfgu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gnwrtryoa.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/gqoasqqmm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.yfazqb.com/Article/details/gdgrsjdbm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/grirfpvmp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.yfazqb.com/Article/details/ghgkmfhwd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gecibxmnz.sHtML

[L04] 设置超时
来源：http://m.share.yfazqb.com/Article/details/govexedtu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fktsv.cn/Article/details/gqayyxrlk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.epnwcf.com/Article/details/gjcxqboey.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/grkarsrur.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.epnwcf.com/Article/details/gzqfellqv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.yfazqb.com/Article/details/gzmjwyhvh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.bbcook.cn/Article/details/gzvjdzorh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/gentvmtbg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.vehdjk.com/Article/details/grcduchdn.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fktsv.cn/Article/details/gghffmope.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.yfazqb.com/Article/details/gnltjeunn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.vehdjk.com/Article/details/gtahxtbje.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gxscqygyt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/gwvjsiddg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/gggusporz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fktsv.cn/Article/details/gcntztzwm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.sjlbkw.cn/Article/details/gjmfrtsqm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/gcrpjpnuo.sHtML

[L06] 解析响应为 JSON
来源：http://wap.yfazqb.com/Article/details/gjckqituz.sHtML

Py:   resp.json()
来源：http://mobile.fktsv.cn/Article/details/gjwrhqrel.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/glciybigf.sHtML

JS:   await resp.json()
来源：http://m.share.sjlbkw.cn/Article/details/ghmbvnuvs.sHtML

TS:   await resp.json()
来源：http://read.share.bbcook.cn/Article/details/grtfikakh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.vehdjk.com/Article/details/gdeetamnz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.vehdjk.com/Article/details/gbklnxgcm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.epnwcf.com/Article/details/gaipiknut.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gzhuywpyf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.bbcook.cn/Article/details/gntshsitg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.epnwcf.com/Article/details/geuzhxzjy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.bbcook.cn/Article/details/gnkyudwev.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.vehdjk.com/Article/details/ghtlydvgh.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.tarul.cn/Article/details/gfjxvefdb.sHtML

Java: resp.statusCode()
来源：http://blog.tarul.cn/Article/details/gmmxrdsba.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/guplywbsx.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fktsv.cn/Article/details/ghltleumm.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.bbcook.cn/Article/details/gevguavzd.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gtdkukmpj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.epnwcf.com/Article/details/gsbvltaja.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.epnwcf.com/Article/details/ggpwmgmff.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gfvpqrnmh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.sjlbkw.cn/Article/details/gcqqlvrnd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.vehdjk.com/Article/details/gfnovksic.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fktsv.cn/Article/details/gvarpqxnd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.vehdjk.com/Article/details/glbxnxtjv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/gkqbafdzp.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gvdhyeirx.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.epnwcf.com/Article/details/gtanlttys.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gitqaomkp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gqarjaavz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.epnwcf.com/Article/details/gslxzcpwa.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/gcwznuskq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gbalpnkuw.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/ggyuaiqsu.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.tarul.cn/Article/details/gkihymkef.sHtML

Go:   os.Args[1:]
来源：http://blog.vehdjk.com/Article/details/glkbgmwgy.sHtML

Ruby: ARGV
来源：http://www.share.epnwcf.com/Article/details/giofdhzcl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/goijoqwyq.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/grlfwvogz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gtcbgtony.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gnxxvmtfr.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gdxyfoked.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/gecbkfhrh.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.vehdjk.com/Article/details/ggmrgltiv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fktsv.cn/Article/details/gdiabzwbv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.tarul.cn/Article/details/gtntggulr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/gelljsekb.sHtML

[M03] 执行外部命令
来源：http://mobile.tarul.cn/Article/details/gtvmmkwjt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gchjkzwbh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gtfalkhzr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/grmgycgqu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/ggqtxstsi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/gkmsxpdnv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.sjlbkw.cn/Article/details/gedqynpjn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/gsjvgzknh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/gvrglacjn.sHtML

[M04] 获取当前工作目录
来源：http://m.share.sjlbkw.cn/Article/details/gqgrhshie.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/guuxqivss.sHtML

PHP:  getcwd();
来源：http://www.m.share.epnwcf.com/Article/details/geuxhvvbl.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gkuxkktai.sHtML

TS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/ghlhlazpc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gvgvlrtjy.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/gwchgfbqo.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gfkqcydch.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gijncfrtq.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gpokdbptn.sHtML

Py:   sys.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gzobaluyz.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gjkrcuscc.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gigxriqnc.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gqmrgqjlu.sHtML

Java: System.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gmzqdjxna.sHtML

Go:   os.Exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gcxquggss.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/grlwfgdrr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gdsgynlmj.sHtML

[M06] 向标准错误输出
来源：http://blog.fktsv.cn/Article/details/gtixvkowy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.vehdjk.com/Article/details/gvpxnuzew.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/ggsfdrvwz.sHtML

JS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gglqrarhm.sHtML

TS:   console.error("err")
来源：http://baike.epnwcf.com/Article/details/golkvygte.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gkssyxxgu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/grsniyple.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gtowxiqwp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.epnwcf.com/Article/details/gnkneedgh.sHtML

[M07] 判断是否为主入口
来源：http://www.share.tarul.cn/Article/details/ghyfomvab.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fktsv.cn/Article/details/gwaxkxgte.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gwyczaohj.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gppfvqqyi.sHtML

TS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gvnzcxfxh.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.vehdjk.com/Article/details/gxrxecucg.sHtML

Go:   func main()
来源：http://wap.tarul.cn/Article/details/gpsmwtcbl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gulcyzfjp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fktsv.cn/Article/details/gufgmqdro.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/ggbnlaqsl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/glxbsesup.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.sjlbkw.cn/Article/details/gecyarury.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gjzftatyk.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/ghxqzvfjc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.sjlbkw.cn/Article/details/gomwxzjbe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.bbcook.cn/Article/details/gqnyvhahc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gkgcmhbxq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/gfykjakkg.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gldmpkmlc.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gllzalgjc.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gvrlvgzqb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gperzeast.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gstmkqplh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gjuimoozh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gzbezuwon.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gadnofwau.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gbzquqliz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gribdgjgg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gnoapytzf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gzgnmoxqh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.sjlbkw.cn/Article/details/grkatnakz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/guzimnvba.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fktsv.cn/Article/details/gbgtzgnyi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gaggfgrew.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gdcexhdcy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.tarul.cn/Article/details/gfiwfadft.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gwlfxxqdf.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gubojrfzl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.tarul.cn/Article/details/gkcwiprpj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gyljvtufi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gadwkofoo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gffrdlbar.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.epnwcf.com/Article/details/gumnpevuh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gdsrtauch.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/gpboexhau.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.bbcook.cn/Article/details/gsobrkxqb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.epnwcf.com/Article/details/gxncruanb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gvvtzytgx.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gumguwfni.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gzvykenyw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/gwsdwdgff.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gilbakyya.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gbpjooekf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gzxrdschz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.vehdjk.com/Article/details/gvrclghgv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gtgorckjl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/geqrapwuo.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gbjwrrioe.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gomavhsug.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/gqbgwnlvk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gdtbkmlfa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/ggglkpsqq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gygbeijgz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gmzkchsid.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gfoshuuab.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fktsv.cn/Article/details/gcwrpuvhr.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.yfazqb.com/Article/details/guwmrbqqp.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gpwgoxvii.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/ghoojenij.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.bbcook.cn/Article/details/gzbfpmpzm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/grjiwkycl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fktsv.cn/Article/details/ggikrsfph.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gawnkekdr.sHtML

Ruby: s == s.reverse
来源：http://wap.bbcook.cn/Article/details/gayqorzzm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.vehdjk.com/Article/details/gndhumpwq.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/gmprzuhht.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.bbcook.cn/Article/details/gfjzqmyaw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.sjlbkw.cn/Article/details/gwwscsrol.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fktsv.cn/Article/details/gplbxooai.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/geygwbhfp.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gkhutuytc.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gyeukloxw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gtwcrzteh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fktsv.cn/Article/details/giymwgaid.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/grjzrzihi.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.sjlbkw.cn/Article/details/gdbzrugvr.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/gowiuspgs.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gfcrlojra.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/ghwctavzw.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gkvparadg.sHtML

Go:   // 手写回溯递归
来源：http://wap.vehdjk.com/Article/details/gvibxuxbn.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fktsv.cn/Article/details/gglakfygx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gtegbghlj.sHtML

[N09] 栈与队列
来源：http://baike.vehdjk.com/Article/details/guigjyqaz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gevgxonfi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.bbcook.cn/Article/details/gvrltowhw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/grlrteuqk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gaqgyrgcz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/guxjihpdd.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.vehdjk.com/Article/details/gufpttvsp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/gxvvyvgcr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/gnoplrzvv.sHtML

[N10] 链表节点定义
来源：http://www.m.share.vehdjk.com/Article/details/gvtxgwezu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.epnwcf.com/Article/details/gargwzpzz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.bbcook.cn/Article/details/gwpfweslq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fktsv.cn/Article/details/gjxrtvcnv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.vehdjk.com/Article/details/gfrfejuxq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gytanoovt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.yfazqb.com/Article/details/gcumxnwjg.sHtML


<!-- 参考信息 -->