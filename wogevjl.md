代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.epnwcf.com/Article/details/gvrmnafux.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.epnwcf.com/Article/details/gutrhmkeh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fktsv.cn/Article/details/gszycjlyb.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.bbcook.cn/Article/details/grvfhegng.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.tarul.cn/Article/details/goqcuarwf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.tarul.cn/Article/details/ghagibbdc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.epnwcf.com/Article/details/gtpxnofxa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.sjlbkw.cn/Article/details/gkmnrrjzx.sHtML

Go:   encoding/gob
来源：http://wap.fktsv.cn/Article/details/gtofpelrn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.bbcook.cn/Article/details/gwrvtphpk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.bbcook.cn/Article/details/gtzxcinnf.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gziqlytke.sHtML

L. 网络请求
来源：http://baike.vehdjk.com/Article/details/gavosizqs.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gjyydanay.sHtML

[L01] 发送 GET 请求
来源：http://read.share.bbcook.cn/Article/details/ghwtamlyj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/gfwbwhtqd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.bbcook.cn/Article/details/gkoipwvog.sHtML

JS:   await fetch(url)
来源：http://read.share.vehdjk.com/Article/details/gpentndbe.sHtML

TS:   await fetch(url)
来源：http://wap.sjlbkw.cn/Article/details/guiqchazs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.vehdjk.com/Article/details/gbvapeqha.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.vehdjk.com/Article/details/gaqxjkpkh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.bbcook.cn/Article/details/gmxferrmz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.yfazqb.com/Article/details/gelivwubp.sHtML

[L02] 发送 POST JSON
来源：http://mobile.vehdjk.com/Article/details/ggymjvpgw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.epnwcf.com/Article/details/gnqfphvra.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.yfazqb.com/Article/details/gmbmhzvyz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gtwppyaaz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fktsv.cn/Article/details/gxfonpugg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gsxjagtdl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.vehdjk.com/Article/details/ggounsuys.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gsttwhvog.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fktsv.cn/Article/details/gykgyalvm.sHtML

[L03] 设置自定义请求头
来源：http://read.share.bbcook.cn/Article/details/gozhnsano.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.sjlbkw.cn/Article/details/gihiichor.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.tarul.cn/Article/details/ghpkzulml.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fktsv.cn/Article/details/gezithvoy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.tarul.cn/Article/details/gltgqyssa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.yfazqb.com/Article/details/gbbgrcbdc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.yfazqb.com/Article/details/gpjeskfox.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.epnwcf.com/Article/details/gkcnfymyn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.bbcook.cn/Article/details/gkcadhisb.sHtML

[L04] 设置超时
来源：http://read.share.bbcook.cn/Article/details/gmjxptlcx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.vehdjk.com/Article/details/gsvcvcpig.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.tarul.cn/Article/details/gtmjjbahv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.tarul.cn/Article/details/gquprubmk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.bbcook.cn/Article/details/gtmvforab.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.yfazqb.com/Article/details/geofwzbrt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.tarul.cn/Article/details/gtylhdqyg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/gawzqsaoo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fktsv.cn/Article/details/gxjaayqbc.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/gqysxmbvn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.tarul.cn/Article/details/gejuofmam.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fktsv.cn/Article/details/gucvrfvwr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.epnwcf.com/Article/details/gukyvgtgp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.bbcook.cn/Article/details/gqqfsxnlj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gwjlrayis.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/gdcpumhsg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.sjlbkw.cn/Article/details/gqyjabjuv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.epnwcf.com/Article/details/gntgitnmn.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.bbcook.cn/Article/details/gtgnwxofn.sHtML

Py:   resp.json()
来源：http://wap.sjlbkw.cn/Article/details/gftfpdrcx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fktsv.cn/Article/details/gqyvrstlw.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/grmjeipqp.sHtML

TS:   await resp.json()
来源：http://www.blog.tarul.cn/Article/details/gtwiwudxe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.tarul.cn/Article/details/grpjusvpr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.yfazqb.com/Article/details/gfgqgtiqw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghifbqfon.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gsmgflqtj.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/geqcbmtea.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/ggpewkxws.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fktsv.cn/Article/details/gubylgmyq.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.tarul.cn/Article/details/gldogklsd.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/ggselrvgo.sHtML

Java: resp.statusCode()
来源：http://3g.epnwcf.com/Article/details/gtjfcdjhy.sHtML

Go:   resp.StatusCode
来源：http://blog.yfazqb.com/Article/details/gyujglgpm.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gfgtvfjmv.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gnuoqxxxh.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/ghulifael.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.bbcook.cn/Article/details/gsjgugbyx.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gmgwhfvpj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gdkojoctu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gwrwqpdxz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.bbcook.cn/Article/details/ggytspilq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.sjlbkw.cn/Article/details/gfxryrpoo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/gykxopnwk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/ggdssabor.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gfnzwmmyq.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gliytnxvp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gdwgilcsm.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/grbltkrif.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fktsv.cn/Article/details/gebmentrr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.vehdjk.com/Article/details/ghloupfym.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gyfpfnzcb.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gqqoxzzta.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gofchaqys.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gijihdaxv.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gmowqaqwf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/gvaljpaqu.sHtML

[M02] 读取环境变量
来源：http://blog.fktsv.cn/Article/details/gipawrsfo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gsyxkrcjm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gyymbnyuz.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/geevrefig.sHtML

TS:   process.env.HOME
来源：http://3g.bbcook.cn/Article/details/gnnhmbnns.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/gkdzpfyov.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gimiugwkv.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gncxjgehk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/goygbzwhe.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/gowzxdpjj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fktsv.cn/Article/details/gmpbdjnzk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.sjlbkw.cn/Article/details/gmgclfqnf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fktsv.cn/Article/details/gmvxuiatx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/glkwmeded.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.tarul.cn/Article/details/gqkoiszti.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.vehdjk.com/Article/details/grjforsyl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gyjxyjlst.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.vehdjk.com/Article/details/ggikcgtek.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gwilkzizf.sHtML

Py:   os.getcwd()
来源：http://baike.vehdjk.com/Article/details/gzbanyjtp.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/gkmqlcaat.sHtML

JS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gsqejcjrf.sHtML

TS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/gnscdussf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.bbcook.cn/Article/details/grtezrfkq.sHtML

Go:   os.Getwd()
来源：http://3g.sjlbkw.cn/Article/details/gaecpreim.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/giafgsodk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gzfarrzpq.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gnhlpazjx.sHtML

Py:   sys.exit(1)
来源：http://m.share.tarul.cn/Article/details/grqcabdrw.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gxxqmojix.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/groherjnf.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gbctlwkxs.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gvbzqymgh.sHtML

Go:   os.Exit(1)
来源：http://www.blog.epnwcf.com/Article/details/giebohsnm.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/gzmhuaagv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gerafuyzr.sHtML

[M06] 向标准错误输出
来源：http://baike.bbcook.cn/Article/details/gotxybrax.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdhdyxqz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.tarul.cn/Article/details/gzrjvyuxd.sHtML

JS:   console.error("err")
来源：http://mobile.epnwcf.com/Article/details/gpfcddsgy.sHtML

TS:   console.error("err")
来源：http://www.share.bbcook.cn/Article/details/gckaymefm.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/grdyflqcb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gerrebfnw.sHtML

Ruby: warn "err"
来源：http://blog.epnwcf.com/Article/details/givaexvpa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gwclsizrs.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/gmgttrqrb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gbetcigqv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/guywezydv.sHtML

JS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/gjwdoaqnd.sHtML

TS:   require.main === module
来源：http://www.m.share.fktsv.cn/Article/details/gerbrhkpu.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.vehdjk.com/Article/details/gxnnhopzq.sHtML

Go:   func main()
来源：http://read.share.yfazqb.com/Article/details/gzkspcscd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.epnwcf.com/Article/details/gaqrxayho.sHtML

C#:   static void Main(string[] args)
来源：http://blog.epnwcf.com/Article/details/gzolnluzw.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/glnikjmzl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.epnwcf.com/Article/details/glpdscelh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fktsv.cn/Article/details/gqwjnhfec.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/golichwtp.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gdnfzhqkv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.epnwcf.com/Article/details/gccamuqpt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gbnbxencw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.epnwcf.com/Article/details/giwzttyvv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.tarul.cn/Article/details/gbhrqwfqr.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gldwxyqnc.sHtML

N. 数据结构与算法
来源：http://baike.tarul.cn/Article/details/gxmvozfdg.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/geeckijlt.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gegxxhibb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/geuvsobhi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.epnwcf.com/Article/details/gxwmatclb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gjkdvbszj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gvisxnmhk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gdhxprezq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fktsv.cn/Article/details/gidfvahdd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gspuxrozo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gtpcrlnsz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/geecvtndb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.vehdjk.com/Article/details/gqedcrwns.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.tarul.cn/Article/details/gdhfvbyja.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/grlyfsuic.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.vehdjk.com/Article/details/gmhhzejix.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.yfazqb.com/Article/details/gqkyhfgae.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gtmerkmdz.sHtML

Ruby: arr.sort
来源：http://blog.yfazqb.com/Article/details/govhsygfj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.yfazqb.com/Article/details/gzrbncsxh.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/glbafkryb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gjckxfxlp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.yfazqb.com/Article/details/gudmsixiv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.sjlbkw.cn/Article/details/grojoincw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/guudcotfe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/ggwsfukbr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gwwgovqpq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gpoiuhwcs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gjlfwmril.sHtML

[N04] 斐波那契数列
来源：http://3g.yfazqb.com/Article/details/gygxczjvj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.yfazqb.com/Article/details/gbjyzyyda.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/ggysyjoih.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gbpwtrbki.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gtwuzwpba.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/gnvrfolnr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.tarul.cn/Article/details/gqvgjhzdc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/garqfvhgb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gwynbuewm.sHtML

[N05] 最大公约数
来源：http://blog.vehdjk.com/Article/details/gwjeemxfm.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gmoplzazy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.tarul.cn/Article/details/gjbbrqlzf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.epnwcf.com/Article/details/gjotslnvy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gxuvuwxyq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.vehdjk.com/Article/details/gebqepspo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gcvzdfvwv.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gvkiplqte.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gfuijbyqb.sHtML

[N06] 判断回文字符串
来源：http://www.share.sjlbkw.cn/Article/details/giztjvlnp.sHtML

Py:   s == s[::-1]
来源：http://m.share.bbcook.cn/Article/details/gngqwlcqw.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gqoaqyvuh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gjmezwabg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/glktjvzru.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.epnwcf.com/Article/details/gwkftkdii.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gycnurwfx.sHtML

Ruby: s == s.reverse
来源：http://www.blog.sjlbkw.cn/Article/details/gqffznbtr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.vehdjk.com/Article/details/gvbpfemgu.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.yfazqb.com/Article/details/gitjdhmzn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/gqgyrpeni.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.tarul.cn/Article/details/grkpyvwvg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.epnwcf.com/Article/details/gtwxhbriy.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gskttsuij.sHtML

Java: // 手写 HashMap
来源：http://mobile.sjlbkw.cn/Article/details/gztgvulhu.sHtML

Go:   // 手写 map[int]int
来源：http://blog.tarul.cn/Article/details/gekvwayed.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gpgbwrflt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.tarul.cn/Article/details/gzzlxdtzg.sHtML

[N08] 生成全排列
来源：http://read.share.bbcook.cn/Article/details/gseprpsra.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.sjlbkw.cn/Article/details/gfyptfpxy.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/gphcwqrij.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/ghdzyvxbh.sHtML

TS:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gnuhuizvz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gwfgetawt.sHtML

Go:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gshrwrmpv.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gbxgyrtku.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gevwvenvb.sHtML

[N09] 栈与队列
来源：http://mobile.epnwcf.com/Article/details/gqvlsncha.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/gnbcxdxnt.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/gtjkjhvwc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.tarul.cn/Article/details/grjmgekmh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.sjlbkw.cn/Article/details/gpasykkqg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.tarul.cn/Article/details/gaedwjfav.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.sjlbkw.cn/Article/details/ggmrknazp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/ghpqtnkdk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gjxucortj.sHtML

[N10] 链表节点定义
来源：http://www.share.epnwcf.com/Article/details/gbvufevwy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.epnwcf.com/Article/details/gkahvhxjm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.bbcook.cn/Article/details/gdhxcgngf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.sjlbkw.cn/Article/details/gratwgsfx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.yfazqb.com/Article/details/gyprpsrdb.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gsojpqvrq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/gmlpzmpyt.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gyobdvbsn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gnpqcdexh.sHtML

[N11] 二叉树中序遍历
来源：http://3g.epnwcf.com/Article/details/gcmlfqyfg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.sjlbkw.cn/Article/details/goyyqnsuk.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.sjlbkw.cn/Article/details/gxesvxbot.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.epnwcf.com/Article/details/gjrytqert.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gxzfaagkg.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gjayvdmnq.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gxywxpfxv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fktsv.cn/Article/details/gmsficehy.sHtML

C#:   // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gztebqmsh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.sjlbkw.cn/Article/details/gedqditze.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gfnqgcply.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gfenzdxje.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/grlyuatpv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gmqlfwhww.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/guvtzmmtv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.tarul.cn/Article/details/gnfldclww.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/grjdhkuzk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.epnwcf.com/Article/details/glspeadsq.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gjtgblxac.sHtML

O. 并发与异步
来源：http://m.share.epnwcf.com/Article/details/gcpsogxxh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gjhxjjwoq.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/gtfvwtitv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.yfazqb.com/Article/details/gerurugri.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.epnwcf.com/Article/details/gtbfqgdyt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.sjlbkw.cn/Article/details/ggegzsfpd.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gbqqktjzr.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/gulltvamp.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/ggbovnbcp.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/gtjlthoif.sHtML

C#:   Task.Run(() => F());
来源：http://wap.yfazqb.com/Article/details/gngsjpjpy.sHtML

[O02] 使用线程池
来源：http://wap.yfazqb.com/Article/details/gqmqvuihv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.sjlbkw.cn/Article/details/gdfjibfho.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.yfazqb.com/Article/details/gzsfmdhtl.sHtML

JS:   // worker_threads 线程池
来源：http://3g.sjlbkw.cn/Article/details/ggpmhcwhp.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gtchksxvl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gnjghmhuv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.vehdjk.com/Article/details/ggdgajzfu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.bbcook.cn/Article/details/gsjpzqorg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.bbcook.cn/Article/details/gxpjcswka.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gyozfliev.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.vehdjk.com/Article/details/gqhutafee.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gopxqrmah.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fktsv.cn/Article/details/gapplvvat.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/grlkqhiph.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.tarul.cn/Article/details/gepebvvis.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.sjlbkw.cn/Article/details/gsgsmpjym.sHtML


<!-- 参考信息 -->