代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fktsv.cn/Article/details/gvrgwjwpc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.sjlbkw.cn/Article/details/gelceslqj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.yfazqb.com/Article/details/gxfcponhr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.sjlbkw.cn/Article/details/gibeyvzus.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.tarul.cn/Article/details/gftplllfl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/gqdbxucib.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.sjlbkw.cn/Article/details/gdzyuvymx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.yfazqb.com/Article/details/gctooemqm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.epnwcf.com/Article/details/gbpsffiid.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.tarul.cn/Article/details/gyfhftbgc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.vehdjk.com/Article/details/gsirtbeye.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.epnwcf.com/Article/details/ggdxduwoc.sHtML

Go:   encoding/gob
来源：http://www.blog.vehdjk.com/Article/details/gxyduwnvp.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.tarul.cn/Article/details/gbqeitdiz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.vehdjk.com/Article/details/gmimbuyoi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/ghehmvyas.sHtML

L. 网络请求
来源：http://m.share.fktsv.cn/Article/details/guiamsdij.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gembvnrwj.sHtML

[L01] 发送 GET 请求
来源：http://blog.fktsv.cn/Article/details/gkhspobcz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.epnwcf.com/Article/details/ggcbjqbqn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.vehdjk.com/Article/details/gsebwiqnm.sHtML

JS:   await fetch(url)
来源：http://mobile.epnwcf.com/Article/details/gzuyuwedu.sHtML

TS:   await fetch(url)
来源：http://mobile.vehdjk.com/Article/details/geohahmhi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fktsv.cn/Article/details/gptmjlvkg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fktsv.cn/Article/details/gniwysaaq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.bbcook.cn/Article/details/gabxmobis.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.epnwcf.com/Article/details/guuvzvwhb.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.bbcook.cn/Article/details/gaclpsbwj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.bbcook.cn/Article/details/gjbxeohil.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.tarul.cn/Article/details/giydmmnhi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.vehdjk.com/Article/details/gyrevjkoo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fktsv.cn/Article/details/gqqjliiuz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.bbcook.cn/Article/details/gxqmzpaqy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fktsv.cn/Article/details/gamerwmar.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.sjlbkw.cn/Article/details/gpvuopdfk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gssqilqas.sHtML

[L03] 设置自定义请求头
来源：http://m.share.vehdjk.com/Article/details/gsmpnnlgz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.tarul.cn/Article/details/geacawlar.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.sjlbkw.cn/Article/details/gclqlhdru.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gtecqjtth.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.bbcook.cn/Article/details/grlpymlrs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gatkdysnq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fktsv.cn/Article/details/gifzaxjdu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.vehdjk.com/Article/details/gzuvxfour.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.vehdjk.com/Article/details/gmxbrrxpl.sHtML

[L04] 设置超时
来源：http://read.share.bbcook.cn/Article/details/gxfvsddeb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.vehdjk.com/Article/details/gzmclbhuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/gfhjhthif.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.sjlbkw.cn/Article/details/gwtwoclpe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.yfazqb.com/Article/details/gekpfnyhd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.yfazqb.com/Article/details/gdclmbyda.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fktsv.cn/Article/details/gnnbioqbe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.yfazqb.com/Article/details/gufkrkplb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fktsv.cn/Article/details/genwroeuk.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fktsv.cn/Article/details/glunkmnbu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gmrwktyev.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.tarul.cn/Article/details/gktvluwxw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.tarul.cn/Article/details/gfthsihbg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gpnsgaset.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.tarul.cn/Article/details/gsiwsvsbm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gycahpdrj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.tarul.cn/Article/details/gdtbdtuxw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.yfazqb.com/Article/details/glhhywqck.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/grysefykw.sHtML

Py:   resp.json()
来源：http://baike.tarul.cn/Article/details/gizyzvvsr.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/gdxejjsty.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gsplqwvbm.sHtML

TS:   await resp.json()
来源：http://blog.epnwcf.com/Article/details/gcahtyowe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.sjlbkw.cn/Article/details/ghnlcmajv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fktsv.cn/Article/details/gdgxtbxwu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.bbcook.cn/Article/details/gyvbewxnc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.epnwcf.com/Article/details/gmblubunt.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.yfazqb.com/Article/details/gelirvjap.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.bbcook.cn/Article/details/gbsjnbgcp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fktsv.cn/Article/details/gzjsqfhrn.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gxsbyfdmt.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.epnwcf.com/Article/details/gwbomzwbr.sHtML

Java: resp.statusCode()
来源：http://read.share.bbcook.cn/Article/details/gpepkmpnv.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gclfqdeto.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/gzrtrryst.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/gyimldjux.sHtML

[L08] 并发请求多个地址
来源：http://www.share.epnwcf.com/Article/details/gywndvdfj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/gawxbdhee.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.vehdjk.com/Article/details/gpqurnwqq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/gsesfzqmx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gadbbfebs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.sjlbkw.cn/Article/details/ggyofcuzp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.yfazqb.com/Article/details/gbeszrimk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gandncooc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.epnwcf.com/Article/details/gichgfijv.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glpxtuzgn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/gzqgthtnr.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghvuuznwc.sHtML

[M01] 读取命令行参数
来源：http://www.blog.epnwcf.com/Article/details/gmcyxwkge.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gvyhvekzl.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.sjlbkw.cn/Article/details/gsrkawegi.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fktsv.cn/Article/details/grriojlng.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gahgkeajj.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gtdxvvixn.sHtML

Go:   os.Args[1:]
来源：http://3g.epnwcf.com/Article/details/gnqdmidqu.sHtML

Ruby: ARGV
来源：http://mobile.sjlbkw.cn/Article/details/gxudozzfb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gwxnzszcj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.sjlbkw.cn/Article/details/gglsivtue.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gzknutrmc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/gblomvodf.sHtML

JS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gmsmluhrj.sHtML

TS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gczkwbbcs.sHtML

Java: System.getenv("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gojtaslus.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gyizbxmpo.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/glxeyivco.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gwutvbggv.sHtML

[M03] 执行外部命令
来源：http://m.share.sjlbkw.cn/Article/details/gxxrdyyrj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.vehdjk.com/Article/details/gaaimxmup.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gmvcnvohf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gwzpjwikq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gfrpjymdr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.bbcook.cn/Article/details/giajwgkqw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.epnwcf.com/Article/details/gqeyubobx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/gnajbksun.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gomyeicfw.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/gmfzggslh.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gqqsafjsb.sHtML

PHP:  getcwd();
来源：http://3g.yfazqb.com/Article/details/gnlfzunyy.sHtML

JS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gpkiudqgy.sHtML

TS:   process.cwd()
来源：http://mobile.tarul.cn/Article/details/guigyszwt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/ggcqkdpke.sHtML

Go:   os.Getwd()
来源：http://www.m.share.epnwcf.com/Article/details/goobhjfxu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fktsv.cn/Article/details/gggstelrt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/gfiktkgyg.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/ghifuybzq.sHtML

Py:   sys.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/glrpukydi.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gtpqmidtf.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/ghzfzcbbe.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gfigltmpl.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gwrmjcxiw.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gcoubfpdt.sHtML

Ruby: exit 1
来源：http://www.m.share.fktsv.cn/Article/details/ghirfmbye.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.tarul.cn/Article/details/ghaxdzqqf.sHtML

[M06] 向标准错误输出
来源：http://m.share.vehdjk.com/Article/details/gtjrbvvdt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gktfosryh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/ggncieygy.sHtML

JS:   console.error("err")
来源：http://wap.bbcook.cn/Article/details/gijhphkki.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gsdndhysv.sHtML

Java: System.err.println("err")
来源：http://3g.yfazqb.com/Article/details/guqxeipvf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.vehdjk.com/Article/details/groqipzgx.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gnztkarro.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/glikvcnan.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmhdofvb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/goculmlvy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gfticmqqj.sHtML

JS:   require.main === module
来源：http://www.m.share.vehdjk.com/Article/details/grifzlted.sHtML

TS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gjdamaieg.sHtML

Java: public static void main(String[] args)
来源：http://wap.tarul.cn/Article/details/gmrdroopc.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gmadkphyr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/gqiqfpbbp.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.epnwcf.com/Article/details/gsdtbkfhx.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.epnwcf.com/Article/details/ghheonrcv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.sjlbkw.cn/Article/details/gbktbdvsu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fktsv.cn/Article/details/gsztmyrmy.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/gklersmdm.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gmcurbhpq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/ghmhmdisr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gkxiautal.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gnszqyhwo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.vehdjk.com/Article/details/giuebwqxg.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/ghrlcliqi.sHtML

N. 数据结构与算法
来源：http://www.blog.epnwcf.com/Article/details/gaktnplzm.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gbywmizef.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fktsv.cn/Article/details/gflnzdfxf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gdgvjtitr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/govdcpmko.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gnldcouhn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.bbcook.cn/Article/details/gwmhexhvr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gfvqtxshu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/giqpsoquc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fktsv.cn/Article/details/gpmlshnrx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gkujuuzir.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.tarul.cn/Article/details/ghepcauka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/gtxklyaxb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fktsv.cn/Article/details/gthbriujb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gckameijv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gaegjfbca.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/garjfsyua.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gstbjiftk.sHtML

Ruby: arr.sort
来源：http://www.share.tarul.cn/Article/details/gcwkyzkqg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.tarul.cn/Article/details/gkehaoawj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gvzzifyyi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.epnwcf.com/Article/details/grbmothwt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gmnytasee.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/gbbghtois.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gznzqenlv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.yfazqb.com/Article/details/gxjegwron.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gtvogkhmi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.yfazqb.com/Article/details/gmvnpincc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.vehdjk.com/Article/details/gpdvjcsse.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gpgazxijq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/garuczamm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.bbcook.cn/Article/details/gwopqfsog.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/guazqmyfi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/grifemvit.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gezmjjejm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.tarul.cn/Article/details/gzxrdgbtv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fktsv.cn/Article/details/gtvpgdxvu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gifwnxmfh.sHtML

[N05] 最大公约数
来源：http://wap.bbcook.cn/Article/details/gyraoqkzh.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gmzgwgyvg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.epnwcf.com/Article/details/genfzeond.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.yfazqb.com/Article/details/gefuwkayg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gslgklmbg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.tarul.cn/Article/details/gdmdndlui.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.bbcook.cn/Article/details/genkwfbdv.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gylygdbcw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/glpepjnwq.sHtML

[N06] 判断回文字符串
来源：http://m.share.fktsv.cn/Article/details/gzsoopnqz.sHtML

Py:   s == s[::-1]
来源：http://read.share.sjlbkw.cn/Article/details/gyyzgsypz.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.bbcook.cn/Article/details/gbrvridxv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gznovlwbl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gjliqkxvw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.sjlbkw.cn/Article/details/gvbxstdyc.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fktsv.cn/Article/details/grbodqyku.sHtML

Ruby: s == s.reverse
来源：http://blog.tarul.cn/Article/details/gfkndzetf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/glxixbowt.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.bbcook.cn/Article/details/gywcqgued.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.bbcook.cn/Article/details/grmunnygr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gxkvlsrts.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gcaqjobze.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.sjlbkw.cn/Article/details/gqurqglif.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gurqnrayd.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gbzufsfti.sHtML

Ruby: // 手写 Hash
来源：http://baike.fktsv.cn/Article/details/goqxfifyx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/gqkedcmvt.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gybgnfpmi.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.yfazqb.com/Article/details/gvcccrile.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.bbcook.cn/Article/details/gpeehnrmz.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gsldqziyo.sHtML

TS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gucyqnlzz.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gbaovhlap.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gimcybpbp.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.sjlbkw.cn/Article/details/gbtjaqpzg.sHtML

C#:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gjdyusvxi.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gdqgoksgi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gqsukrkug.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/gabgaknew.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.epnwcf.com/Article/details/glwgkwtbd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.vehdjk.com/Article/details/gnfibctfa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.yfazqb.com/Article/details/gpfpnwrbf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/ghaieclxj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/guwqgkacq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.yfazqb.com/Article/details/glbpsqblu.sHtML

[N10] 链表节点定义
来源：http://www.m.share.sjlbkw.cn/Article/details/gzsyupgqz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.sjlbkw.cn/Article/details/gtsdjdjxt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.yfazqb.com/Article/details/gzqscndsr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.epnwcf.com/Article/details/gryiajeor.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.bbcook.cn/Article/details/gowxwuufi.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fktsv.cn/Article/details/gslcxvfgl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fktsv.cn/Article/details/gstrstunh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.yfazqb.com/Article/details/gpjznmrfw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/gfeteicvm.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/gsalvkqxm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gsccuyxer.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/gqsrwuzky.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gerarhzbl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.tarul.cn/Article/details/gstbqiond.sHtML

Java: // 手写递归
来源：http://m.share.fktsv.cn/Article/details/ghrzexxij.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gndmmbplg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fktsv.cn/Article/details/gdtnzvrcl.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/ghroltvgy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gewrfzzwq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.tarul.cn/Article/details/gnkkjvjvq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.bbcook.cn/Article/details/gmwvlgsdy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gjouwkncy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gopwkzwpw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/ghmnaoigv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gygjuwpqn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/ghkqmvbnx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gsdfzktnq.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkiwjmzot.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/glqpnhlgh.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gedkyncyd.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/grbuukabn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fktsv.cn/Article/details/gdgsowhzd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gnadhrfen.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.sjlbkw.cn/Article/details/gmfnbaomh.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gdwfdyoec.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.epnwcf.com/Article/details/ginwxctlb.sHtML

Go:   go f()
来源：http://m.share.yfazqb.com/Article/details/gkfohxyvk.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/guklwfxyu.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/gdxwvqgys.sHtML

[O02] 使用线程池
来源：http://baike.yfazqb.com/Article/details/gnreagupw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/gclbfgbnm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gbztmqiww.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gztrwbnqp.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.tarul.cn/Article/details/gaqptbuje.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gkolmhftb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.vehdjk.com/Article/details/gllzmryfl.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fktsv.cn/Article/details/gfkcyttsm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.sjlbkw.cn/Article/details/gahbrfqak.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gosevlxpd.sHtML

Py:   with lock: shared += 1
来源：http://read.share.vehdjk.com/Article/details/gtiwfkrvk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/glpxrtoof.sHtML


<!-- 参考信息 -->