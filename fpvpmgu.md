代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.vehdjk.com/Article/details/gxcwtvktd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.yfazqb.com/Article/details/gkmfyxkkm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.epnwcf.com/Article/details/gfutfosco.sHtML

[K05] 深拷贝对象
来源：http://read.share.bbcook.cn/Article/details/gpxwxobiv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.tarul.cn/Article/details/gpmyqlmkb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.bbcook.cn/Article/details/giaovybez.sHtML

JS:   structuredClone(obj)
来源：http://3g.bbcook.cn/Article/details/gbowbguyk.sHtML

TS:   structuredClone(obj)
来源：http://baike.fktsv.cn/Article/details/gkcjcsdmh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.epnwcf.com/Article/details/gftihodwp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.bbcook.cn/Article/details/gyjipulnn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.sjlbkw.cn/Article/details/grfhtdvmr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.sjlbkw.cn/Article/details/gbzzgbssm.sHtML

[K06] 解析 URL 查询串
来源：http://blog.vehdjk.com/Article/details/gqzkzyjau.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.sjlbkw.cn/Article/details/gktjhimbf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.tarul.cn/Article/details/gjlqtpyfg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.vehdjk.com/Article/details/geupqiqsc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.yfazqb.com/Article/details/gjpsjbbau.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.vehdjk.com/Article/details/gdiobzsxi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.bbcook.cn/Article/details/gizkfxtpd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.epnwcf.com/Article/details/gfbtacmwc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.sjlbkw.cn/Article/details/gipvowyec.sHtML

[K07] 进制转换
来源：http://wap.tarul.cn/Article/details/gwwjywuoe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gucldimas.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.sjlbkw.cn/Article/details/ghnuuwlwt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.epnwcf.com/Article/details/guagdbffo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.tarul.cn/Article/details/grditdgio.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.vehdjk.com/Article/details/gohgwczsd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.yfazqb.com/Article/details/gvzjwqftn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.vehdjk.com/Article/details/gfkmkbdvp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.bbcook.cn/Article/details/gsltxakws.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.bbcook.cn/Article/details/gaxikxqib.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.yfazqb.com/Article/details/gxziyaouv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.bbcook.cn/Article/details/gukfquxqn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.yfazqb.com/Article/details/ghpivlndl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.vehdjk.com/Article/details/gqswtynlb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.sjlbkw.cn/Article/details/gepvmmhrw.sHtML

Go:   encoding/gob
来源：http://read.share.fktsv.cn/Article/details/gxmwyibtl.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fktsv.cn/Article/details/getrgkrwe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fktsv.cn/Article/details/gthnsnoou.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gzafbqljz.sHtML

L. 网络请求
来源：http://www.m.share.yfazqb.com/Article/details/gbvjggfsv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gotusnruf.sHtML

[L01] 发送 GET 请求
来源：http://3g.yfazqb.com/Article/details/grpowesuh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.vehdjk.com/Article/details/gveigoemd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.yfazqb.com/Article/details/gixroibvm.sHtML

JS:   await fetch(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gjeqxzxmu.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/getbnrlyd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fktsv.cn/Article/details/gefegivpr.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.tarul.cn/Article/details/gednnmant.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.sjlbkw.cn/Article/details/guvmaugnx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fktsv.cn/Article/details/gotixqaoo.sHtML

[L02] 发送 POST JSON
来源：http://wap.sjlbkw.cn/Article/details/gfgfqijlf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gohakoalw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fktsv.cn/Article/details/gjzegecrn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.epnwcf.com/Article/details/gdtomjhmc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.sjlbkw.cn/Article/details/gkbhboqjw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.bbcook.cn/Article/details/gujwxyawk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.vehdjk.com/Article/details/giooarxgw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.tarul.cn/Article/details/glvsveasa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.tarul.cn/Article/details/glqotcnrx.sHtML

[L03] 设置自定义请求头
来源：http://wap.bbcook.cn/Article/details/gxnrbrnhf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gzzhlmeyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fktsv.cn/Article/details/gxlneojsg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gblorstse.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gxguaavez.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.bbcook.cn/Article/details/gmrgeodlf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.bbcook.cn/Article/details/grvtfjgfe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.tarul.cn/Article/details/gecysdrgv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fktsv.cn/Article/details/ghyjmlcgk.sHtML

[L04] 设置超时
来源：http://m.share.bbcook.cn/Article/details/gstholxwf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.epnwcf.com/Article/details/ghvkexszq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fktsv.cn/Article/details/gpwhpudcx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/gxsotzggz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fktsv.cn/Article/details/gtddeipys.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.bbcook.cn/Article/details/gopkdwvbt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.yfazqb.com/Article/details/grjomcqzq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/gqngpcksr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.tarul.cn/Article/details/gtakgiswb.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gjmnbtffs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gnvrryxpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gwpjhqtrf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/goaqaemmg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.vehdjk.com/Article/details/gwsxgoyju.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.epnwcf.com/Article/details/glzwrzqfa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.epnwcf.com/Article/details/gswhfqqjt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.yfazqb.com/Article/details/gxlttddza.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.bbcook.cn/Article/details/gazhzpglo.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.yfazqb.com/Article/details/ggeabqgue.sHtML

Py:   resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gcykdayxq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.tarul.cn/Article/details/gitpejsuk.sHtML

JS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/ghedextal.sHtML

TS:   await resp.json()
来源：http://blog.fktsv.cn/Article/details/gbnkeuqjb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gbfwxphzp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.bbcook.cn/Article/details/gzuburnus.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.bbcook.cn/Article/details/gelvqwwbm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.bbcook.cn/Article/details/gbhkasjnu.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.vehdjk.com/Article/details/gkyvfmajx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gbdeinwtm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.bbcook.cn/Article/details/godgkintr.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.yfazqb.com/Article/details/gnugwnzvi.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/gvsspkuco.sHtML

Java: resp.statusCode()
来源：http://www.m.share.epnwcf.com/Article/details/gnlsjrwjv.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gfrygwuki.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gfhdoqvqm.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.vehdjk.com/Article/details/gpmvapxbk.sHtML

[L08] 并发请求多个地址
来源：http://mobile.vehdjk.com/Article/details/gixnlwvlv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fktsv.cn/Article/details/gmxwveobh.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.vehdjk.com/Article/details/guwesckma.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gvhwbrurs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gasjnbkqw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gldgfndjl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gjiyxrzun.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gdnsycoaq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gnczsswuu.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gkidvxsdm.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/galiupedn.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gomogdpnb.sHtML

[M01] 读取命令行参数
来源：http://baike.vehdjk.com/Article/details/gqaetpyoz.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fktsv.cn/Article/details/gzkppccqm.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/ggukimdfc.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fktsv.cn/Article/details/gtyllqwon.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gxchxaanx.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.tarul.cn/Article/details/gxitnjdin.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/ghhwqfnsp.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gbqcotwoh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gzneopisl.sHtML

[M02] 读取环境变量
来源：http://mobile.epnwcf.com/Article/details/gczjiapqd.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.yfazqb.com/Article/details/grebvpxna.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/ggiljytbb.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gzvisccjt.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gimxqctyd.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gdujqalab.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/gmiejxjim.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.yfazqb.com/Article/details/gjnynbbwd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gpeajptng.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gzxgjjbno.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/gexfffhqo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.vehdjk.com/Article/details/gpvzimlwv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gofqfkaom.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.vehdjk.com/Article/details/gwtqwoosa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gkhqwnrot.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gczswvajk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/gwvjshelr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gtskrolev.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gjpvdrrli.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/ghnndrbvs.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gnmiwyedl.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gubnvissh.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gldacvfnf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.tarul.cn/Article/details/gebtajojp.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gxdjnbtqd.sHtML

Ruby: Dir.pwd
来源：http://blog.tarul.cn/Article/details/gbivxqyxp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gdfzfvhtl.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gvlfpbfuh.sHtML

Py:   sys.exit(1)
来源：http://mobile.bbcook.cn/Article/details/ghzysmjrn.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gzflbhrjv.sHtML

JS:   process.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gihekggnw.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gbxonyvkd.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/guvhsjuaw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gzlhmrpkv.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gzaebsjyj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fktsv.cn/Article/details/ggaxixpsm.sHtML

[M06] 向标准错误输出
来源：http://mobile.yfazqb.com/Article/details/gliypfnjy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.tarul.cn/Article/details/gwrbochdh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.tarul.cn/Article/details/gyxieyjkg.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gfyxnmjwn.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/ggztoista.sHtML

Java: System.err.println("err")
来源：http://baike.yfazqb.com/Article/details/glmsvullc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fktsv.cn/Article/details/gfzfhufzr.sHtML

Ruby: warn "err"
来源：http://wap.tarul.cn/Article/details/gysehswsa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fktsv.cn/Article/details/guocalwpu.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/grbtaqtlo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gknqrzohs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/gspvlhdol.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/gnyhqagsz.sHtML

TS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gadffbbqe.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gdltwhuvb.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gfisjyxzp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/gctgjrhsj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/ghyzkgaov.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.yfazqb.com/Article/details/gjgehafqv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gtytjulaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.sjlbkw.cn/Article/details/gtpepwjez.sHtML

JS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gjpxkhyrw.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gmrbgeptl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gmcxkorik.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fktsv.cn/Article/details/gtwfmkcad.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/galvimcxs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/gfpdfaqxi.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gkyrtebkf.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gepligfoq.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghcpaamew.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/gewyjdbpt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.tarul.cn/Article/details/gvxfdrktq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gssvpuyxp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/goarnulky.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gojonfnou.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gsctlteax.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/govbminxl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.bbcook.cn/Article/details/gdwtvssyw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gsslytrqs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/gsscizzii.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.sjlbkw.cn/Article/details/grsqvgltm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.tarul.cn/Article/details/golfeviiu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.bbcook.cn/Article/details/gfludeetd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gycukgdtz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/grwgmmodo.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gnipmpktq.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gtermhsfn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/ghuteljia.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/gsubhaxux.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.vehdjk.com/Article/details/gzppzwivo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/ggutxdwuc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/gmmbmtzvw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gdvsuoaip.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fktsv.cn/Article/details/ganhjwcyk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.sjlbkw.cn/Article/details/gzvoymjtg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.bbcook.cn/Article/details/gafmuxfhp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gzzyqadea.sHtML

[N04] 斐波那契数列
来源：http://read.share.tarul.cn/Article/details/gzdgyvvut.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gxqfhqlpf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gpzswfcvp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/grwglorfj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gcjdeaecg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.bbcook.cn/Article/details/gnrwvurqv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.yfazqb.com/Article/details/gwkrqmocp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gsfcbdrbk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gcqnoicvk.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/gtnpjswth.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/gzguvusky.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gxogdtdfi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gxixntqxh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.tarul.cn/Article/details/gsgompplz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.vehdjk.com/Article/details/gqrrsiekh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.epnwcf.com/Article/details/gidmmahrz.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.yfazqb.com/Article/details/gsbymoqbu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gydnbdggi.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/gucwvzdtn.sHtML

Py:   s == s[::-1]
来源：http://blog.fktsv.cn/Article/details/gwqtifnma.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/glbuyjcry.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gggoxgjmg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/grizjbkbh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gienfqhwl.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.sjlbkw.cn/Article/details/gsqbkbmzb.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gjdntdiqe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/ggsnbkpmj.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gdoubmdws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/glxqvtgbu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.vehdjk.com/Article/details/gdeubytix.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.sjlbkw.cn/Article/details/gotsesyhv.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.tarul.cn/Article/details/gortgtymb.sHtML

Java: // 手写 HashMap
来源：http://read.share.tarul.cn/Article/details/gqycgtmkm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.tarul.cn/Article/details/gbtohmeox.sHtML

Ruby: // 手写 Hash
来源：http://blog.bbcook.cn/Article/details/gmaminrva.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gpnzovgom.sHtML

[N08] 生成全排列
来源：http://blog.epnwcf.com/Article/details/gqpdyvgac.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gwljyxrbc.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gupmpxqxk.sHtML

JS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gctswukel.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gijoazenl.sHtML

Java: // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gneitkrcb.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gjltahkop.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.tarul.cn/Article/details/goxiuolra.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gesjmfuoe.sHtML

[N09] 栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gfzkxakeb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.vehdjk.com/Article/details/gzvfbhqia.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gvahaaugm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gcrrdyppk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.epnwcf.com/Article/details/guhjqptkf.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/ggrqwnydj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.sjlbkw.cn/Article/details/gnmzfpxst.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gmdjzldif.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gomhwyfyc.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/geseyxwbb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gkjxzxwpv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gfodnudvz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.bbcook.cn/Article/details/gizugjfom.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.tarul.cn/Article/details/gvrejwvnp.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gthalrcdc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.sjlbkw.cn/Article/details/gguxbqcph.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gcbdmkukg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/guzehhjvs.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fktsv.cn/Article/details/gujppdlta.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/gqtiewtnm.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.tarul.cn/Article/details/gxgetiogp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/grrlfdzuj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gqqjssjio.sHtML

Java: // 手写递归
来源：http://wap.vehdjk.com/Article/details/geleexeez.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gxmtgmxod.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gitpuxnee.sHtML

C#:   // 手写递归
来源：http://wap.yfazqb.com/Article/details/gsjqpasbx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/gjuevcjoj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.sjlbkw.cn/Article/details/gprepcgya.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/gxrfnhubz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gnvmuorby.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gxmsoiydz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gnhvsmsnr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.sjlbkw.cn/Article/details/gpqdxrrdk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gxpkdrzan.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/gfpcbxznp.sHtML


<!-- 参考信息 -->