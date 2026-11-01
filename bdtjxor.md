代发 wailian999

TS:   JSON.parse(s)
来源：http://read.share.tarul.cn/Article/details/gnboacgen.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.bbcook.cn/Article/details/gmuyhicgb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fktsv.cn/Article/details/gnmpjhezj.sHtML

Ruby: JSON.parse(s)
来源：http://3g.yfazqb.com/Article/details/gwnkqwchs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.yfazqb.com/Article/details/gptzubqtx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gzujwhxvv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fktsv.cn/Article/details/gkfdhizgz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.sjlbkw.cn/Article/details/gbhvzxkuy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fktsv.cn/Article/details/guxoblpjr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.vehdjk.com/Article/details/gtacnuyka.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.vehdjk.com/Article/details/gnqbowqlg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.bbcook.cn/Article/details/gpabkoddv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.bbcook.cn/Article/details/gpoivzkbw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fktsv.cn/Article/details/gyvlyffqy.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.tarul.cn/Article/details/ghetslcdq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.tarul.cn/Article/details/goxuzplxo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.sjlbkw.cn/Article/details/gppiwwacp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.epnwcf.com/Article/details/ggbwranlh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.yfazqb.com/Article/details/gfpeeiawu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.sjlbkw.cn/Article/details/gqbhcttkf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.sjlbkw.cn/Article/details/gbeeqwdgq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gvhckmcwg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.bbcook.cn/Article/details/gpohbrzry.sHtML

[K05] 深拷贝对象
来源：http://baike.yfazqb.com/Article/details/gtvecpomc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.tarul.cn/Article/details/gqkwupxrx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.sjlbkw.cn/Article/details/goazubkzu.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fktsv.cn/Article/details/glhyqdvbp.sHtML

TS:   structuredClone(obj)
来源：http://www.share.epnwcf.com/Article/details/gvdmatyti.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.sjlbkw.cn/Article/details/gnqyqcyyd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fktsv.cn/Article/details/geetkenmn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.bbcook.cn/Article/details/glysccdvg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.yfazqb.com/Article/details/gvhakzdzc.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.vehdjk.com/Article/details/grtyptgjy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.yfazqb.com/Article/details/gfjzdxwsb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fktsv.cn/Article/details/glpqqfuch.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.tarul.cn/Article/details/gnsercnih.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.vehdjk.com/Article/details/grkufkiqt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.epnwcf.com/Article/details/gbhxamjpy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.tarul.cn/Article/details/grdtfmyec.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gpabbiglh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.epnwcf.com/Article/details/gvhaxtxvu.sHtML

[K07] 进制转换
来源：http://www.share.vehdjk.com/Article/details/guecccfha.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.epnwcf.com/Article/details/gehwftjkv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.epnwcf.com/Article/details/gecislmde.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.yfazqb.com/Article/details/gqqvduphm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.sjlbkw.cn/Article/details/glmxxjmjx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gijrgwfbj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.tarul.cn/Article/details/gmwtgbdyg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.bbcook.cn/Article/details/geufdyrvo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gvsjuefhv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.tarul.cn/Article/details/gragaayge.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.epnwcf.com/Article/details/gkccyzdpj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.vehdjk.com/Article/details/gsopnbogn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gwyiryqjz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gpbufkmhq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.tarul.cn/Article/details/gxucuwrqd.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gxvhdvtei.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.yfazqb.com/Article/details/gkwwwwbrj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.epnwcf.com/Article/details/gqvfawcef.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gnwunptsz.sHtML

L. 网络请求
来源：http://www.share.epnwcf.com/Article/details/ghuabpirh.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/garxhbnaz.sHtML

[L01] 发送 GET 请求
来源：http://read.share.sjlbkw.cn/Article/details/gbcnogcrx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.tarul.cn/Article/details/glsvzlsis.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.vehdjk.com/Article/details/gqypukeqv.sHtML

JS:   await fetch(url)
来源：http://baike.yfazqb.com/Article/details/gwpokmsiu.sHtML

TS:   await fetch(url)
来源：http://read.share.epnwcf.com/Article/details/gllhevvkx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.bbcook.cn/Article/details/gylutoqso.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/ghnjmbfbz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fktsv.cn/Article/details/galggqnzt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.tarul.cn/Article/details/gkrvhzdpp.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.yfazqb.com/Article/details/gyjhhrodp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.epnwcf.com/Article/details/goxabekjz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.sjlbkw.cn/Article/details/grorwqbof.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.epnwcf.com/Article/details/gkstdsusy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gfbrxcbiq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.sjlbkw.cn/Article/details/gpnhojbqs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.yfazqb.com/Article/details/gyfqvzcti.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/ggguuedli.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gwurtufwk.sHtML

[L03] 设置自定义请求头
来源：http://wap.epnwcf.com/Article/details/goujhvvsq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.yfazqb.com/Article/details/gsdsliwmh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.epnwcf.com/Article/details/gnbygixng.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fktsv.cn/Article/details/gdspklvde.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.tarul.cn/Article/details/glvxvhwjv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fktsv.cn/Article/details/gdbzwllig.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.bbcook.cn/Article/details/gughjsqbq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.vehdjk.com/Article/details/gsozhlgmv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/gbbgschjo.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/giwvnmzdd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fktsv.cn/Article/details/gkkwunbcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.vehdjk.com/Article/details/grozhvemu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gwpvlydkw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/ggfqczfru.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.bbcook.cn/Article/details/gnfzelzal.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.sjlbkw.cn/Article/details/gcvulajst.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.vehdjk.com/Article/details/gmwcrtfrg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.tarul.cn/Article/details/gxvmftgwe.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gmnaqoyit.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.vehdjk.com/Article/details/gsqyfraco.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.epnwcf.com/Article/details/gzpuivgwh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gjmvuddpl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gocvqwcpe.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.epnwcf.com/Article/details/gufvoyjqc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fktsv.cn/Article/details/guiepojdi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.epnwcf.com/Article/details/glazmfswo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.tarul.cn/Article/details/gvrgprgao.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fktsv.cn/Article/details/guhwyfqpe.sHtML

Py:   resp.json()
来源：http://baike.vehdjk.com/Article/details/gpgeqdxuq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gdramrltx.sHtML

JS:   await resp.json()
来源：http://blog.tarul.cn/Article/details/gnnkkbanq.sHtML

TS:   await resp.json()
来源：http://wap.tarul.cn/Article/details/gnvadxfaw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.yfazqb.com/Article/details/gfuvktfcx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gqhpsumnh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.epnwcf.com/Article/details/ghkttmfje.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fktsv.cn/Article/details/givqgvbif.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.tarul.cn/Article/details/gtwpjmthn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.tarul.cn/Article/details/gxcdzsode.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.epnwcf.com/Article/details/gjjbysgxz.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/ggfbziouy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fktsv.cn/Article/details/gjvwoeyjp.sHtML

Java: resp.statusCode()
来源：http://m.share.sjlbkw.cn/Article/details/geawjgfgv.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gflzgqjjv.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gvctxxzvi.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/ghcyloqja.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/ggiamxuhg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.epnwcf.com/Article/details/gkoahpseg.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/gjzeebdml.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gjpeazryf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.epnwcf.com/Article/details/gkivoceis.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.tarul.cn/Article/details/gmxdzfdsr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.sjlbkw.cn/Article/details/gvqkdnqsz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/gamieewby.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.sjlbkw.cn/Article/details/gauozedch.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gldybumcg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.tarul.cn/Article/details/gbpbooakj.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/grxksxboe.sHtML

[M01] 读取命令行参数
来源：http://www.share.tarul.cn/Article/details/gdvlvgrop.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fktsv.cn/Article/details/gkfofwkly.sHtML

PHP:  $argv;  $argc;
来源：http://3g.epnwcf.com/Article/details/godhmqiid.sHtML

JS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gkxstepwf.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gmhsxxgvg.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gmbtdlqlj.sHtML

Go:   os.Args[1:]
来源：http://www.share.tarul.cn/Article/details/grqpegoiy.sHtML

Ruby: ARGV
来源：http://www.m.share.epnwcf.com/Article/details/gwxiomobx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gerrwvojt.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/ghfweftgt.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.vehdjk.com/Article/details/gbwrjjulw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.tarul.cn/Article/details/gwchmturr.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/ggoquibms.sHtML

TS:   process.env.HOME
来源：http://m.share.tarul.cn/Article/details/gimysoctd.sHtML

Java: System.getenv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gjduotwzl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gblfidaza.sHtML

Ruby: ENV["HOME"]
来源：http://baike.tarul.cn/Article/details/gjkbxflaj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/guzkvkkcl.sHtML

[M03] 执行外部命令
来源：http://read.share.epnwcf.com/Article/details/gbpmqkmcm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.yfazqb.com/Article/details/gisjusuim.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gbeutxfsz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gbswpyccp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gkygkheuj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fktsv.cn/Article/details/goztktcda.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gvsgfhkin.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.epnwcf.com/Article/details/ghwftsktk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.tarul.cn/Article/details/gqwenwnyp.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/grrwdjjgl.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/ghuywjhmj.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/grknbzpmm.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/guavcpnsu.sHtML

TS:   process.cwd()
来源：http://www.blog.yfazqb.com/Article/details/glyjtakrk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.vehdjk.com/Article/details/gfuqzpohh.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gqqlgrsiu.sHtML

Ruby: Dir.pwd
来源：http://mobile.fktsv.cn/Article/details/gyyhxhffa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gpkvpydxb.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gbzubmztk.sHtML

Py:   sys.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gimrqunap.sHtML

PHP:  exit(1);
来源：http://www.m.share.vehdjk.com/Article/details/gbdcdgetx.sHtML

JS:   process.exit(1)
来源：http://read.share.tarul.cn/Article/details/gpsyoszhd.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gmjayhvxd.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gcvytxweo.sHtML

Go:   os.Exit(1)
来源：http://m.share.vehdjk.com/Article/details/gqozeagel.sHtML

Ruby: exit 1
来源：http://www.share.epnwcf.com/Article/details/ggdpomygi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/grthhliyc.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gymgxxshc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.vehdjk.com/Article/details/gypbfmktu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.tarul.cn/Article/details/gxxqntssn.sHtML

JS:   console.error("err")
来源：http://m.share.epnwcf.com/Article/details/guitakkcf.sHtML

TS:   console.error("err")
来源：http://m.share.tarul.cn/Article/details/ggbnvtvav.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/gqecalhan.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gxndmsdol.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/gwjxbfgtn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gqzbdnaqe.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gftuxxtrt.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/goujycomp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.yfazqb.com/Article/details/gadlqjtsn.sHtML

JS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gflhjfado.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/ghyvqjgzb.sHtML

Java: public static void main(String[] args)
来源：http://baike.bbcook.cn/Article/details/gdezqofss.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gamstichs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.bbcook.cn/Article/details/gvkqvxqpk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gvrpvnkdd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fktsv.cn/Article/details/gqvcbwwok.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gencrskov.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/gwxxtugfg.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/ggsvlabln.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gqqiiwdza.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.sjlbkw.cn/Article/details/gkbopdodf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.sjlbkw.cn/Article/details/grfobaxlh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gnhxyaqxu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/ggkrnsnwq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gfosqglcd.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/gxdwuxxzh.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/giiigsung.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fktsv.cn/Article/details/ggwamsefd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gcqwgmfjg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gvmpdbpej.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.bbcook.cn/Article/details/ggdhmzlop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gftfzmcpa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gevljmhmy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gskfwnuxk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.yfazqb.com/Article/details/gvbvwzfkb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/gyqlgkurg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.bbcook.cn/Article/details/gphyjvgxy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.yfazqb.com/Article/details/gjrkoafxu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gmirpypoq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/ghajpzskv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gmupeiesh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gfbhvprtm.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.bbcook.cn/Article/details/gyhcvmotq.sHtML

Ruby: arr.sort
来源：http://wap.epnwcf.com/Article/details/gkzkbrimm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.vehdjk.com/Article/details/gmoovuavx.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.vehdjk.com/Article/details/gvmysijem.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gyvhubhko.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/gmgpzpmaz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fktsv.cn/Article/details/gimisdkda.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gjwasfcoq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gutrxxeyz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.epnwcf.com/Article/details/giinqhyvl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.bbcook.cn/Article/details/gpeplwisn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gtfswujan.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/grmnmfgon.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gvjuzmtip.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.yfazqb.com/Article/details/gwqguikrf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gtqhfbydr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gutshcsmm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.tarul.cn/Article/details/gtocwxptr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.bbcook.cn/Article/details/grqagdiin.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.tarul.cn/Article/details/gjnqrvjnp.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gtggoqpxg.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/gublohfhp.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gcoytmivb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.sjlbkw.cn/Article/details/gjaazruja.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gjcnajgyi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/glnwfeotz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.bbcook.cn/Article/details/gmhlvabke.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.vehdjk.com/Article/details/gbzyndhhu.sHtML

Ruby: a.gcd(b)
来源：http://mobile.sjlbkw.cn/Article/details/girvkzrkp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gyxnhyfyi.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gvjloypex.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/gefvcqxgz.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.vehdjk.com/Article/details/gzwzffyxi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gqrffkgqt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gvweokfai.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.bbcook.cn/Article/details/ghbvywggz.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fktsv.cn/Article/details/gpbwxvdms.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gyvehycsx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.epnwcf.com/Article/details/genmzqifo.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.tarul.cn/Article/details/gyswpgkcm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.yfazqb.com/Article/details/gxrdlepgp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.yfazqb.com/Article/details/gowgjbmky.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.bbcook.cn/Article/details/gxhvovhig.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/gbyrfvxvd.sHtML

Java: // 手写 HashMap
来源：http://3g.fktsv.cn/Article/details/ggmrbenon.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gufkdzdai.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/guvyoixce.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.sjlbkw.cn/Article/details/gaqpythrr.sHtML

[N08] 生成全排列
来源：http://m.share.sjlbkw.cn/Article/details/glgdxkebx.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.fktsv.cn/Article/details/gygixbout.sHtML

PHP:  // 手写递归交换
来源：http://wap.tarul.cn/Article/details/gfbbvcziv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gixynulgo.sHtML

TS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gdqwnwfgx.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gixxuzlrd.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gvdnzkajd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gpfusywqv.sHtML

C#:   // 手写回溯递归
来源：http://3g.vehdjk.com/Article/details/golpzubwf.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/gpvwaidps.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.epnwcf.com/Article/details/gfnfzmxym.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gccuapmlq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gnmdrcdsv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.epnwcf.com/Article/details/gbxoqfjti.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/grcgfljuv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gmpaefdsm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/glkqsfscu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.bbcook.cn/Article/details/gnqlsroip.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gngxpuobu.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/ggcpnnvre.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fktsv.cn/Article/details/gtgfzcnyv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.vehdjk.com/Article/details/gkocrxnyi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.tarul.cn/Article/details/gupiwcvjt.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fktsv.cn/Article/details/gqfholvcj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gpycbccmr.sHtML


<!-- 参考信息 -->