代发 wailian999

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fktsv.cn/Article/details/gkgjjfjtw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.yfazqb.com/Article/details/gcykaoefb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.tarul.cn/Article/details/grlvagqnf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fktsv.cn/Article/details/gapcxthci.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.bbcook.cn/Article/details/gkbygwlye.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fktsv.cn/Article/details/gauzzayon.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.sjlbkw.cn/Article/details/gfuyxcxmk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.epnwcf.com/Article/details/gwibvzkub.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fktsv.cn/Article/details/glnmmunfp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.epnwcf.com/Article/details/gqkxdwxtb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.vehdjk.com/Article/details/geoyzfwli.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.tarul.cn/Article/details/gxvbzigvc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.epnwcf.com/Article/details/gytkglkcj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fktsv.cn/Article/details/gtehkshfn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.yfazqb.com/Article/details/gbrjfkwuf.sHtML

[K05] 深拷贝对象
来源：http://blog.tarul.cn/Article/details/gthzljbjp.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fktsv.cn/Article/details/gdsxomrsz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.sjlbkw.cn/Article/details/gcbpktkgi.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.tarul.cn/Article/details/goyghxvrw.sHtML

TS:   structuredClone(obj)
来源：http://baike.yfazqb.com/Article/details/gyltkxkzp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.epnwcf.com/Article/details/guoqauzbj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.vehdjk.com/Article/details/gpqbmlplz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.yfazqb.com/Article/details/gdjpavkxb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.tarul.cn/Article/details/gnukcegwj.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.bbcook.cn/Article/details/gixbxxdgn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.bbcook.cn/Article/details/gfzyzjqso.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fktsv.cn/Article/details/gxazjmnvz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.epnwcf.com/Article/details/gjovgpstq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.vehdjk.com/Article/details/gvrlqndvi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.bbcook.cn/Article/details/ghfkcmmtl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.tarul.cn/Article/details/gnyntdeoi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fktsv.cn/Article/details/grohchtrs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.tarul.cn/Article/details/ghjoxqvln.sHtML

[K07] 进制转换
来源：http://mobile.epnwcf.com/Article/details/grvyfyqhe.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fktsv.cn/Article/details/gwoapbnhf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.sjlbkw.cn/Article/details/gnpcfobgn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fktsv.cn/Article/details/gzrsgwfcd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.tarul.cn/Article/details/gnvwuulnx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.yfazqb.com/Article/details/gjfziwhme.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.yfazqb.com/Article/details/gcbdjdaep.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfliopqsf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.epnwcf.com/Article/details/gfhsimllk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.epnwcf.com/Article/details/ghdkyuioh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.vehdjk.com/Article/details/gxsxjjgkh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.tarul.cn/Article/details/gfgiterjr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fktsv.cn/Article/details/gwfklmuae.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.epnwcf.com/Article/details/gnhhmrbmm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.bbcook.cn/Article/details/gwivsbcjq.sHtML

Go:   encoding/gob
来源：http://www.blog.sjlbkw.cn/Article/details/gqasylkcl.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.bbcook.cn/Article/details/gfeqomspe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fktsv.cn/Article/details/gkhdvzgbh.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gwbyuhgvz.sHtML

L. 网络请求
来源：http://read.share.epnwcf.com/Article/details/gjxkykizo.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gzqfnmtld.sHtML

[L01] 发送 GET 请求
来源：http://wap.sjlbkw.cn/Article/details/ggmmyebgh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fktsv.cn/Article/details/glrcyfhzt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.vehdjk.com/Article/details/gonrpqcxc.sHtML

JS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/grwzympqp.sHtML

TS:   await fetch(url)
来源：http://www.blog.yfazqb.com/Article/details/gphwssunm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.sjlbkw.cn/Article/details/gtmvsptpe.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fktsv.cn/Article/details/gledbkqyy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fktsv.cn/Article/details/gsukeukul.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fktsv.cn/Article/details/gmoqjfmth.sHtML

[L02] 发送 POST JSON
来源：http://baike.yfazqb.com/Article/details/gkpsusqlo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.yfazqb.com/Article/details/gaterbrbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fktsv.cn/Article/details/gpgcbfzjt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.vehdjk.com/Article/details/gcvjurvzz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.vehdjk.com/Article/details/gssfeckuy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.yfazqb.com/Article/details/gdhzabgre.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.sjlbkw.cn/Article/details/gevakeuut.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fktsv.cn/Article/details/gouwgrqow.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.vehdjk.com/Article/details/gvahqdpmx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.bbcook.cn/Article/details/gksmkbvgo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fktsv.cn/Article/details/gurkibscw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.yfazqb.com/Article/details/gkwnyhzjo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.tarul.cn/Article/details/gswggnfxt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.epnwcf.com/Article/details/gbazyajsd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.tarul.cn/Article/details/gquzxillu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.sjlbkw.cn/Article/details/gixwmcxul.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.vehdjk.com/Article/details/gqruprwbm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fktsv.cn/Article/details/gxclddbbf.sHtML

[L04] 设置超时
来源：http://wap.yfazqb.com/Article/details/gisksuejf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/gorbjrqop.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.epnwcf.com/Article/details/gnroshkyv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.tarul.cn/Article/details/gxlilnukq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gazhvsaaa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.tarul.cn/Article/details/gyjfgqhrp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.sjlbkw.cn/Article/details/ggvtocahl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.sjlbkw.cn/Article/details/geiaatpgv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.yfazqb.com/Article/details/gobpawnns.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.sjlbkw.cn/Article/details/gagxoxttb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fktsv.cn/Article/details/gylsloubj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/gqoaaosti.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.epnwcf.com/Article/details/guwdjhqep.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.epnwcf.com/Article/details/grejidplf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.tarul.cn/Article/details/graaxqrng.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gqouixrip.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fktsv.cn/Article/details/gnvzpkxfh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.tarul.cn/Article/details/gxjyhaidx.sHtML

[L06] 解析响应为 JSON
来源：http://blog.tarul.cn/Article/details/gbfkjehgn.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gbgllzogt.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/glcybsubq.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gltehicot.sHtML

TS:   await resp.json()
来源：http://www.share.fktsv.cn/Article/details/gxvoxhnti.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.tarul.cn/Article/details/gjeuscibh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.yfazqb.com/Article/details/guzfhgarf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/grfeffuff.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gkywdsjyz.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/ghlqnxcac.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fktsv.cn/Article/details/godblwqqo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdskbrtod.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/galohduui.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.bbcook.cn/Article/details/ggpbipoww.sHtML

Java: resp.statusCode()
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmzvtpkn.sHtML

Go:   resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gegsbltdu.sHtML

Ruby: resp.code.to_i
来源：http://read.share.vehdjk.com/Article/details/gmzmyvzir.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gpqclioiq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.vehdjk.com/Article/details/gzmmvxnrh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.vehdjk.com/Article/details/ggjjbwens.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.bbcook.cn/Article/details/gwbtalabt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.epnwcf.com/Article/details/gcumwtzex.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/giwogwgam.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.bbcook.cn/Article/details/gadnnipmm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fktsv.cn/Article/details/gesasumts.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gvsaqeyyi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fktsv.cn/Article/details/gvjrxugzt.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ggyvpqhnp.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.sjlbkw.cn/Article/details/gdlfqgfgi.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/guthhdjwx.sHtML

[M01] 读取命令行参数
来源：http://mobile.fktsv.cn/Article/details/gfcbyaqob.sHtML

Py:   sys.argv[1:]
来源：http://3g.yfazqb.com/Article/details/gdgocmxch.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gsbaimxqg.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gilsdpxgp.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gfckbzrhn.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gpqovwgmc.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/guxqiaigy.sHtML

Ruby: ARGV
来源：http://www.blog.vehdjk.com/Article/details/glrlrjxav.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gkhiuogrs.sHtML

[M02] 读取环境变量
来源：http://wap.epnwcf.com/Article/details/ghfkwjxnt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gxwckqibf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gigbkjqrr.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/gdcgoswib.sHtML

TS:   process.env.HOME
来源：http://www.blog.fktsv.cn/Article/details/ginlxcyxu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gisalrhdp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gwlmobxmv.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.sjlbkw.cn/Article/details/gcfwvtkzw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.vehdjk.com/Article/details/gxytecxsj.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/gfszmbdyh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gttekkmgl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gtnfwgbxz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gmilsocpe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.sjlbkw.cn/Article/details/gurhklrte.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.tarul.cn/Article/details/gpcmngjwx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/ggivymwzt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/ggsvknrhw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.vehdjk.com/Article/details/gjlokankf.sHtML

[M04] 获取当前工作目录
来源：http://blog.yfazqb.com/Article/details/gfiwcfbdj.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gxifmchyt.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/glwvlpxps.sHtML

JS:   process.cwd()
来源：http://blog.bbcook.cn/Article/details/guvidyjjw.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/gyqitlwff.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gtpyrxjrt.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/gualvhuuc.sHtML

Ruby: Dir.pwd
来源：http://blog.bbcook.cn/Article/details/gvvtotrid.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fktsv.cn/Article/details/gxeljxbnv.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gbljfenbp.sHtML

Py:   sys.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gxtrbcqan.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gyyxhbhtq.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/guraxchzi.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gwqbvvsai.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/ghbpufhdh.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gyavwdveo.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/gaxjtohno.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.sjlbkw.cn/Article/details/ggttfpydl.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gwtioqyve.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.tarul.cn/Article/details/gwueoifxb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.epnwcf.com/Article/details/ggscrnpyh.sHtML

JS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gcaprfwny.sHtML

TS:   console.error("err")
来源：http://blog.yfazqb.com/Article/details/gwecptiaa.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gthejuvgx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.sjlbkw.cn/Article/details/gxdxazmzc.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/ggldzwoaa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.bbcook.cn/Article/details/gtxfoxyzt.sHtML

[M07] 判断是否为主入口
来源：http://3g.bbcook.cn/Article/details/gpjtqpmmc.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fktsv.cn/Article/details/gdwblsajg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.sjlbkw.cn/Article/details/gfhsginyy.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gxfronldp.sHtML

TS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gteejkddk.sHtML

Java: public static void main(String[] args)
来源：http://www.share.tarul.cn/Article/details/gdqnxwtlc.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/geemrwrhp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.yfazqb.com/Article/details/ghjywwksf.sHtML

C#:   static void Main(string[] args)
来源：http://baike.epnwcf.com/Article/details/gxytljlvo.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/gdicnufpi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/glsrebuou.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/gqsfzykug.sHtML

JS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gtbfsudpf.sHtML

TS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gyfnhnvdh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gpmwakhfv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.bbcook.cn/Article/details/gsjoukmaw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fktsv.cn/Article/details/gfarqqket.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fktsv.cn/Article/details/gjxttnubg.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gskwfqlns.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/gfilzsegl.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gavvrnjgy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gowatlryi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/gvefddoja.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.vehdjk.com/Article/details/ghoemsgpk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.vehdjk.com/Article/details/gvxhvnfoj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/ghcuonhqm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gqhjxhmrx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gyofygdol.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.tarul.cn/Article/details/gnflmntad.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gbgodbmht.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.bbcook.cn/Article/details/guklidmio.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gjslgkmcf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gbccdgtum.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gjeascpok.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/goboygtaw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.yfazqb.com/Article/details/geucyzefe.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.bbcook.cn/Article/details/ganzysipz.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gwjrhughr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gdtilbbqq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/gjnjjlvdo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.sjlbkw.cn/Article/details/gocuwzkhg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/gmmsaedza.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/goydfuwuq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.vehdjk.com/Article/details/gxzbhkzhc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/gkredavev.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/ganytldgu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.vehdjk.com/Article/details/giywhnded.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gmzswslhf.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/gchinpoul.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gqauoighd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.yfazqb.com/Article/details/gzmjzejkz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/giwghpojl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/gqgejeuen.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/gbhejbmsn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.epnwcf.com/Article/details/grbisurkw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/grubocwmt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gptytnkgn.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/gwoirkiro.sHtML

Py:   math.gcd(a, b)
来源：http://baike.sjlbkw.cn/Article/details/giluivenx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gnytxucyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gpumxmkpq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gevkoqarq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/ggrtwdafs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/gbmjrosfk.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/glhgsfyni.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.yfazqb.com/Article/details/gdfvtlefc.sHtML

[N06] 判断回文字符串
来源：http://wap.fktsv.cn/Article/details/gygtesgvv.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gbztcfrwn.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/ghalfvrhx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gimjqmsbf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gkbwvnapo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fktsv.cn/Article/details/gccgiawwq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.yfazqb.com/Article/details/gpwfzrhvy.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/giobctqyc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gsquyzhgc.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fktsv.cn/Article/details/gacdayqpc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.yfazqb.com/Article/details/gzinzrpfy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.epnwcf.com/Article/details/gcnbpvnos.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gqzhwfqvf.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.yfazqb.com/Article/details/gsesnsbmb.sHtML

Java: // 手写 HashMap
来源：http://3g.tarul.cn/Article/details/gxyeuiiaj.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/giunutpdd.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gxfztlbeq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.tarul.cn/Article/details/gydjjkrnm.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gfslradku.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gztsofhsn.sHtML

PHP:  // 手写递归交换
来源：http://wap.fktsv.cn/Article/details/grlugbcqs.sHtML

JS:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gksklutjr.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gsbmxdukh.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gfzwsjbza.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gscuuvrjo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/gxuhcewwd.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.vehdjk.com/Article/details/gbiqhtios.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gonzhlkqd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.bbcook.cn/Article/details/gbjqrktyu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.epnwcf.com/Article/details/glxwozlzb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gfhgfywpx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.yfazqb.com/Article/details/grvxgsatu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.fktsv.cn/Article/details/gqujgdjgv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.sjlbkw.cn/Article/details/gatqygyzr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gwtcxtrrd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/genfxdztk.sHtML

[N10] 链表节点定义
来源：http://m.share.sjlbkw.cn/Article/details/ghlwkfgcm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gdcadyidm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.yfazqb.com/Article/details/gsjyoiqww.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.tarul.cn/Article/details/gnhkfwirl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/grtfvaegj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkkundhis.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gxphymblz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.sjlbkw.cn/Article/details/gusfocjor.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gdulatccj.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/goimenmvm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/gmatvxkxg.sHtML

PHP:  // 手写递归函数
来源：http://3g.fktsv.cn/Article/details/gppzkpjxd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gzxnlxmef.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gnueogxab.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/grumqyfvz.sHtML


<!-- 参考信息 -->