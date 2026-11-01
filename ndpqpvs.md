代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.bbcook.cn/Article/details/gsvmynmav.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.yfazqb.com/Article/details/gfnztmxfw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.vehdjk.com/Article/details/gjnptgpzs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.tarul.cn/Article/details/gvgxaeqbc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.sjlbkw.cn/Article/details/gjjsljerj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.yfazqb.com/Article/details/godiesrpd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.yfazqb.com/Article/details/gdpgepjvt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.sjlbkw.cn/Article/details/gpxcqclar.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.sjlbkw.cn/Article/details/gvysssqrt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.bbcook.cn/Article/details/grtcowmvx.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.sjlbkw.cn/Article/details/ggusyivoi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.bbcook.cn/Article/details/geocqyfnt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.vehdjk.com/Article/details/gvvwhyzun.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.bbcook.cn/Article/details/goodvawrm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.vehdjk.com/Article/details/gfujnbtug.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.vehdjk.com/Article/details/gmndpokoa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.yfazqb.com/Article/details/gbzvjkwok.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fktsv.cn/Article/details/gybsjwkmy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.yfazqb.com/Article/details/gfjtuqbbe.sHtML

[K05] 深拷贝对象
来源：http://mobile.yfazqb.com/Article/details/gxwnoclcf.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.epnwcf.com/Article/details/gmufmhklc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.yfazqb.com/Article/details/gdzjprrbs.sHtML

JS:   structuredClone(obj)
来源：http://wap.epnwcf.com/Article/details/glgqppmnx.sHtML

TS:   structuredClone(obj)
来源：http://www.share.yfazqb.com/Article/details/gwfhdhhju.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fktsv.cn/Article/details/gytwtqeie.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.epnwcf.com/Article/details/gsduimayg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.tarul.cn/Article/details/gwixvuzga.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.vehdjk.com/Article/details/gbpaxgyni.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.vehdjk.com/Article/details/guxhglcwu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.epnwcf.com/Article/details/gscsgjpnl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.yfazqb.com/Article/details/gfliadtpo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.bbcook.cn/Article/details/gpgstqbxv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.sjlbkw.cn/Article/details/glqdtsojn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.epnwcf.com/Article/details/gtktvydgm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.yfazqb.com/Article/details/geubunegf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.bbcook.cn/Article/details/gwicotiwb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fktsv.cn/Article/details/gigwyvylg.sHtML

[K07] 进制转换
来源：http://blog.fktsv.cn/Article/details/glqmepeam.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.tarul.cn/Article/details/gnpiwgvgd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.sjlbkw.cn/Article/details/glbpuplfa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gfkbicsxc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gwvlgbicw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.tarul.cn/Article/details/gdfxafsjg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.sjlbkw.cn/Article/details/gzunezzyz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.vehdjk.com/Article/details/gjtcwibre.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.bbcook.cn/Article/details/gykiyprhl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.bbcook.cn/Article/details/ghaksepve.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.yfazqb.com/Article/details/gxxwiadhc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fktsv.cn/Article/details/gyarludcc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.bbcook.cn/Article/details/gtgmumizo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gobjlvoha.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.epnwcf.com/Article/details/gojgyadiy.sHtML

Go:   encoding/gob
来源：http://www.share.yfazqb.com/Article/details/gyzzlkxaf.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fktsv.cn/Article/details/gleycxsqp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.tarul.cn/Article/details/goiwbxchz.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gershxftg.sHtML

L. 网络请求
来源：http://blog.tarul.cn/Article/details/gnjdwazof.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gdobggwun.sHtML

[L01] 发送 GET 请求
来源：http://baike.yfazqb.com/Article/details/grqofkccy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.bbcook.cn/Article/details/gqvtilpxc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.tarul.cn/Article/details/glhymxjqm.sHtML

JS:   await fetch(url)
来源：http://blog.tarul.cn/Article/details/gejptrvyy.sHtML

TS:   await fetch(url)
来源：http://www.share.epnwcf.com/Article/details/gfxpbmrin.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gzkquifgs.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.vehdjk.com/Article/details/gjuqnhuja.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.yfazqb.com/Article/details/gujgfzqjq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.epnwcf.com/Article/details/ghqgykasc.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/grdkeqkdg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gackvdatj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.tarul.cn/Article/details/gitnobiom.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.yfazqb.com/Article/details/guprddwof.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.bbcook.cn/Article/details/gahdrjwcz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.tarul.cn/Article/details/gszkojaqb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fktsv.cn/Article/details/gxgmvnado.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.sjlbkw.cn/Article/details/ghqgqedit.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.vehdjk.com/Article/details/gqulzqzsy.sHtML

[L03] 设置自定义请求头
来源：http://read.share.vehdjk.com/Article/details/gawrofsyq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.yfazqb.com/Article/details/gxuqhrouk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.yfazqb.com/Article/details/gdawadbdi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.sjlbkw.cn/Article/details/gqygiwcmx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.epnwcf.com/Article/details/gpuzofppe.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.yfazqb.com/Article/details/glqypmzjo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.bbcook.cn/Article/details/gmghklwed.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.vehdjk.com/Article/details/gztmcurat.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.tarul.cn/Article/details/gftrzzlnf.sHtML

[L04] 设置超时
来源：http://m.share.epnwcf.com/Article/details/gxjbwsxwd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.tarul.cn/Article/details/gtaqjcowc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.yfazqb.com/Article/details/gubcbvvsu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/glfhpbrfy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gcxggvecp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.bbcook.cn/Article/details/gqxcyccbn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.bbcook.cn/Article/details/gearqbvru.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/gwfqekwid.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.vehdjk.com/Article/details/gtehwraws.sHtML

[L05] 上传文件（multipart）
来源：http://blog.epnwcf.com/Article/details/gcmqmkjpx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.epnwcf.com/Article/details/goiyfjxys.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.epnwcf.com/Article/details/gernmlgql.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/gyjbbcjme.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gigyflwux.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fktsv.cn/Article/details/gcjjkrhxj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.bbcook.cn/Article/details/ggerkcaju.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.yfazqb.com/Article/details/gjclimttc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.sjlbkw.cn/Article/details/gckzxmssz.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.bbcook.cn/Article/details/gijesfiyn.sHtML

Py:   resp.json()
来源：http://3g.yfazqb.com/Article/details/gbgqgquqx.sHtML

PHP:  json_decode($body, true);
来源：http://baike.sjlbkw.cn/Article/details/guucjddeh.sHtML

JS:   await resp.json()
来源：http://www.m.share.bbcook.cn/Article/details/gnfdhpotc.sHtML

TS:   await resp.json()
来源：http://www.blog.sjlbkw.cn/Article/details/gipoqhylf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.bbcook.cn/Article/details/ghvttqpgt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/giwrdfrht.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.tarul.cn/Article/details/gvqppnhha.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gbgvrphwg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.sjlbkw.cn/Article/details/gszgeuriv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/gudruikpj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.vehdjk.com/Article/details/gnkpatqoy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.epnwcf.com/Article/details/gtchulvjn.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gbiurtehz.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/ghiixwurq.sHtML

Go:   resp.StatusCode
来源：http://m.share.bbcook.cn/Article/details/gaelardhc.sHtML

Ruby: resp.code.to_i
来源：http://mobile.sjlbkw.cn/Article/details/gqkvjmmbu.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gdxogatmu.sHtML

[L08] 并发请求多个地址
来源：http://read.share.sjlbkw.cn/Article/details/grddwrghc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/gsznhurxo.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fktsv.cn/Article/details/gblnkdgoh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.yfazqb.com/Article/details/gbxbjlkbn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/ggmbasfzg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/gfrfvdfsx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.bbcook.cn/Article/details/gvjfhyblr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fktsv.cn/Article/details/grkxbdinp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.vehdjk.com/Article/details/gzynrdkpj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/ghuhlpbkc.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gyvwjtafc.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gobvffqxb.sHtML

[M01] 读取命令行参数
来源：http://wap.bbcook.cn/Article/details/gqmyshxln.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/gtfipsdnb.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/geyacqldj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gjghafjav.sHtML

TS:   process.argv.slice(2)
来源：http://wap.yfazqb.com/Article/details/gdnkkagsa.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.tarul.cn/Article/details/glnihnqcm.sHtML

Go:   os.Args[1:]
来源：http://m.share.bbcook.cn/Article/details/golozjmyu.sHtML

Ruby: ARGV
来源：http://www.share.bbcook.cn/Article/details/gtfwbvxcs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/ghjgnsigs.sHtML

[M02] 读取环境变量
来源：http://3g.epnwcf.com/Article/details/gqomjfxma.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.vehdjk.com/Article/details/gozhqjfrz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gjwodicba.sHtML

JS:   process.env.HOME
来源：http://m.share.bbcook.cn/Article/details/ggkbsxkyv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gexyetrop.sHtML

Java: System.getenv("HOME")
来源：http://blog.yfazqb.com/Article/details/gwxeyucdr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gcabzdozx.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.tarul.cn/Article/details/gkymmnaxk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.vehdjk.com/Article/details/giuubuecm.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gbvyssges.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.sjlbkw.cn/Article/details/gablnprtw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.vehdjk.com/Article/details/grxrmxqid.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gmzborctp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.yfazqb.com/Article/details/gigaqmlqi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gttjljlly.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gnmqmnxcv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/ggdqraluk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.epnwcf.com/Article/details/gzbocrdyv.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gyhspozyy.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/grzyqhwmg.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/ghisugsjv.sHtML

JS:   process.cwd()
来源：http://m.share.sjlbkw.cn/Article/details/gpuonkbqo.sHtML

TS:   process.cwd()
来源：http://mobile.epnwcf.com/Article/details/gqlemfrzt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/gbnhdtovu.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gzbznjafd.sHtML

Ruby: Dir.pwd
来源：http://read.share.sjlbkw.cn/Article/details/gfybseeok.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.yfazqb.com/Article/details/gnrzsyles.sHtML

[M05] 设置退出码
来源：http://www.m.share.fktsv.cn/Article/details/gusjwezrz.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gdnvzfocq.sHtML

PHP:  exit(1);
来源：http://www.blog.tarul.cn/Article/details/gajbupdei.sHtML

JS:   process.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/garyadkwz.sHtML

TS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/glycwwpmk.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gmjcfecoj.sHtML

Go:   os.Exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gitdomgdy.sHtML

Ruby: exit 1
来源：http://m.share.tarul.cn/Article/details/gugcncyem.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gijmsmozt.sHtML

[M06] 向标准错误输出
来源：http://baike.sjlbkw.cn/Article/details/gtavxbjud.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gmhnlblwa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/gkngarmaf.sHtML

JS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gcskpwcea.sHtML

TS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gewcbkkik.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gbpfytsrw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.sjlbkw.cn/Article/details/gbnpsuvso.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gcxzlnkwk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gwgextkvj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gflgtmgfz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/gpqohhjpv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gtjkwdpnq.sHtML

JS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gqltztzbg.sHtML

TS:   require.main === module
来源：http://3g.yfazqb.com/Article/details/gbuyapysp.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/gjwlxhweb.sHtML

Go:   func main()
来源：http://blog.yfazqb.com/Article/details/gaujbhnqc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.bbcook.cn/Article/details/givnurzpu.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fktsv.cn/Article/details/gysbbbfag.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.vehdjk.com/Article/details/gopzcuykj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gmzficcku.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gxixqjbmm.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gsethvpuc.sHtML

TS:   process.platform;  process.version
来源：http://www.share.yfazqb.com/Article/details/geoiuivzt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gabhtnbjg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.sjlbkw.cn/Article/details/gkjeuqojs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.vehdjk.com/Article/details/gmtfudhnl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gizepwfeh.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/givifrmrd.sHtML

N. 数据结构与算法
来源：http://read.share.epnwcf.com/Article/details/ganqphbzi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtsiajuhc.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/giwpzlwik.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.vehdjk.com/Article/details/gkicaddty.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.bbcook.cn/Article/details/gifbmmwhp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gblwsamto.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.bbcook.cn/Article/details/gkcmhgwwe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/ggvjvswcz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gbarodctu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/ggnndexrr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gxkashcgr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.sjlbkw.cn/Article/details/gkwwtqqzw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fktsv.cn/Article/details/gedccrapm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.bbcook.cn/Article/details/gtwhpzrxy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gvzzgynqm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.tarul.cn/Article/details/grejvcemi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.sjlbkw.cn/Article/details/gnycdhzem.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gfejecjyh.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/grcenbrhp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.sjlbkw.cn/Article/details/gudfmxivc.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/gaduwjynt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.epnwcf.com/Article/details/gfvzwfwre.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.epnwcf.com/Article/details/ghyuxelxv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.sjlbkw.cn/Article/details/gbhqeszqy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gninggfht.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.yfazqb.com/Article/details/gbowahcke.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/gabhgzmqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fktsv.cn/Article/details/gvqaesovq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.epnwcf.com/Article/details/gefhrwthx.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gpvnglgul.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gtspjkqnh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/gwzbpvulc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gehjodgxh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gakcebred.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gimwxumms.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/gjgidjaei.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.bbcook.cn/Article/details/gaxkqoara.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gaigentck.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/gxmhdhvyn.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/ggbfwqpxk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gqdfgmycp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gbujxroow.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gabqsemij.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.yfazqb.com/Article/details/gyotltajn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/gpxbozbck.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/gfiqjxmmy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/grlbchfzj.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gnjtabrxw.sHtML

Py:   s == s[::-1]
来源：http://mobile.yfazqb.com/Article/details/gdzewbubn.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gtstwmdfr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gebkqymkz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gamhuylan.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/ghpwfzezm.sHtML

Go:   // 双指针从两端比较
来源：http://blog.tarul.cn/Article/details/ggdbrctiw.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gqrqppmis.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fktsv.cn/Article/details/gcjdzxuos.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.yfazqb.com/Article/details/ghpkcesyz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.sjlbkw.cn/Article/details/gfcvrcgbi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.yfazqb.com/Article/details/gqmeeblin.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.yfazqb.com/Article/details/gnpunvosw.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/geclhegkt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gsqfujnaq.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.vehdjk.com/Article/details/gcmhxhkdh.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/grhcnqboj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gyvdkitdf.sHtML

[N08] 生成全排列
来源：http://www.share.vehdjk.com/Article/details/gpvjifmmt.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gfputxifq.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gsqtxtzdr.sHtML

JS:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/glrwkyexy.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gojookmjs.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gcfawhbvj.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gwxthkpqm.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.yfazqb.com/Article/details/guyqtcudy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/grxjxwwgd.sHtML

[N09] 栈与队列
来源：http://mobile.fktsv.cn/Article/details/gprzcntpl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.tarul.cn/Article/details/gqiloksnc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gwrrzstln.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fktsv.cn/Article/details/guhrtnxnz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.epnwcf.com/Article/details/gzfffmqds.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.bbcook.cn/Article/details/gofvcvzzg.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.epnwcf.com/Article/details/ggsgxcdaw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gtbqbwczi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gtgnkipfq.sHtML

[N10] 链表节点定义
来源：http://baike.yfazqb.com/Article/details/gtltrlkfn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.tarul.cn/Article/details/gkcoyhnpl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gjnhertvo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.sjlbkw.cn/Article/details/gcodzaeiw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.sjlbkw.cn/Article/details/guuieyiwb.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gijogdimo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.vehdjk.com/Article/details/gjvkzmnuw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/gkxlpdwtm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/gadnhmuir.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/glyfrfbcl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.yfazqb.com/Article/details/ggbawwtwe.sHtML


<!-- 参考信息 -->