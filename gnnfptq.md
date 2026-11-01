代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.yfazqb.com/Article/details/ggfryfoin.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gsssumomh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fktsv.cn/Article/details/gsjdgnpbm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.vehdjk.com/Article/details/gylatatyf.sHtML

Go:   encoding/gob
来源：http://www.share.epnwcf.com/Article/details/gblmrghhl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.sjlbkw.cn/Article/details/grpxzzldb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.tarul.cn/Article/details/gtffksqjo.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/geycvufpj.sHtML

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gpywvtpbd.sHtML

================================================================================
来源：http://wap.fktsv.cn/Article/details/gnxygojxs.sHtML

[L01] 发送 GET 请求
来源：http://baike.bbcook.cn/Article/details/gqubxtstf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.vehdjk.com/Article/details/goaqgnjiw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gquvlovsq.sHtML

JS:   await fetch(url)
来源：http://wap.yfazqb.com/Article/details/gmxxjqhen.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gevlhmdpg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.sjlbkw.cn/Article/details/gnxrxupqx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.bbcook.cn/Article/details/gchnxsubl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.bbcook.cn/Article/details/gvxdihzcu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.vehdjk.com/Article/details/gdljccqgm.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fktsv.cn/Article/details/gpzmgfasg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.vehdjk.com/Article/details/godegopqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.vehdjk.com/Article/details/gjzhyfuxb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.yfazqb.com/Article/details/gpsihtzdf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fktsv.cn/Article/details/gqoosijku.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.bbcook.cn/Article/details/gmpdiwavm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.epnwcf.com/Article/details/gzwcdqpkm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.vehdjk.com/Article/details/gpwrpmhiw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.vehdjk.com/Article/details/gotmxylmi.sHtML

[L03] 设置自定义请求头
来源：http://read.share.yfazqb.com/Article/details/gebtrghzg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.bbcook.cn/Article/details/glqiifcok.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fktsv.cn/Article/details/ginjjfweb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.yfazqb.com/Article/details/gjdfuowox.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.sjlbkw.cn/Article/details/gzecujpaj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.sjlbkw.cn/Article/details/gezjrvzgr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/gracszjgn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.yfazqb.com/Article/details/gxfgjffvn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.sjlbkw.cn/Article/details/gviwwetge.sHtML

[L04] 设置超时
来源：http://blog.yfazqb.com/Article/details/gnysxltcj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.vehdjk.com/Article/details/gzkudtnkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fktsv.cn/Article/details/gyghsvhfv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/glmexppno.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gfgqmbqem.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fktsv.cn/Article/details/ggndmgomj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.tarul.cn/Article/details/gnmfrzblc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.bbcook.cn/Article/details/gtdmwoooq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fktsv.cn/Article/details/gfaeagmlp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.vehdjk.com/Article/details/guvcptyzd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.bbcook.cn/Article/details/gvwkqhaxn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.vehdjk.com/Article/details/gwzgsoxws.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.yfazqb.com/Article/details/gkhrecppe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gtimrwofb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.tarul.cn/Article/details/gmmhxmrqb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.yfazqb.com/Article/details/gjwkobuxp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gbnsosukx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.yfazqb.com/Article/details/gwsiwlqus.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.bbcook.cn/Article/details/gidggsgjp.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/glqvtdkxn.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fktsv.cn/Article/details/ghylbozkl.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gsujbktnn.sHtML

TS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gykbfseqc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/geukrqxfb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fktsv.cn/Article/details/grgngejwj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.sjlbkw.cn/Article/details/gvfdraapa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gwhnbhnbb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.yfazqb.com/Article/details/gxtoggkwf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.tarul.cn/Article/details/gvmtvphsu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.yfazqb.com/Article/details/gccsjcrdc.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/gyxgiyedu.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.bbcook.cn/Article/details/gpiygheqp.sHtML

Java: resp.statusCode()
来源：http://baike.tarul.cn/Article/details/gmbptbbfe.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gvcxxyrdp.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.bbcook.cn/Article/details/gntzwdutu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.epnwcf.com/Article/details/gvvhqgceh.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gjtltwtqh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/gdnljbkez.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.sjlbkw.cn/Article/details/gmtjyhaaz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fktsv.cn/Article/details/guxlakfnm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.tarul.cn/Article/details/ghmurvbai.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.yfazqb.com/Article/details/gxbjugrlb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.yfazqb.com/Article/details/gntgbjqmo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.epnwcf.com/Article/details/gudgzqgem.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fktsv.cn/Article/details/gavuvgmzd.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gaixkwymb.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gehgkvflu.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gfrfqntvv.sHtML

[M01] 读取命令行参数
来源：http://www.blog.yfazqb.com/Article/details/ggjxoqtnl.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gadeiypxu.sHtML

PHP:  $argv;  $argc;
来源：http://3g.sjlbkw.cn/Article/details/gszisjuaw.sHtML

JS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/gajztlayn.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gmpikclyb.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fktsv.cn/Article/details/gpnmocwqm.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gopoctxfk.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/grlmrykcd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/grfwfrrzm.sHtML

[M02] 读取环境变量
来源：http://read.share.sjlbkw.cn/Article/details/gqsegazjw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.tarul.cn/Article/details/gvddylkmp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.sjlbkw.cn/Article/details/griqyjhgv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gtbulbumv.sHtML

TS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gcifoegqx.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gmylxpcrk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.tarul.cn/Article/details/gxgccstri.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.bbcook.cn/Article/details/gycndczcv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gifkatynp.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/giacjwdzb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.sjlbkw.cn/Article/details/gxizjdhwk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fktsv.cn/Article/details/gfqtotwep.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gxawotesx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/giwltjeli.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gippgeahu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.bbcook.cn/Article/details/glglxmycg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.bbcook.cn/Article/details/gbwjfdeuu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fktsv.cn/Article/details/gubdgazty.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gcptcmkir.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gmzmkzriw.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gnhyeiayt.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gjptyezlr.sHtML

TS:   process.cwd()
来源：http://www.share.tarul.cn/Article/details/gmcoupnfd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/gbdofbkim.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gwoncyyru.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gydoajhzn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.sjlbkw.cn/Article/details/gavbqcqpf.sHtML

[M05] 设置退出码
来源：http://m.share.fktsv.cn/Article/details/gpoxeherj.sHtML

Py:   sys.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gtsmxvmki.sHtML

PHP:  exit(1);
来源：http://m.share.fktsv.cn/Article/details/gqlonihml.sHtML

JS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gulyrqrox.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gvocqhfjb.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gegcrbiqo.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gkrzrtpsq.sHtML

Ruby: exit 1
来源：http://3g.vehdjk.com/Article/details/galnadwfg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.sjlbkw.cn/Article/details/gybqgnovh.sHtML

[M06] 向标准错误输出
来源：http://read.share.fktsv.cn/Article/details/gpjoqbykv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gjrxfrjjm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.vehdjk.com/Article/details/geunjskmn.sHtML

JS:   console.error("err")
来源：http://www.share.fktsv.cn/Article/details/gzqbvtcwz.sHtML

TS:   console.error("err")
来源：http://wap.sjlbkw.cn/Article/details/ggoeahtak.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gpxfamlxl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.sjlbkw.cn/Article/details/gcsqaniso.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/gvbcpddie.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/ghlzxubkw.sHtML

[M07] 判断是否为主入口
来源：http://3g.vehdjk.com/Article/details/gusxwqgui.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.yfazqb.com/Article/details/ggbwpjrey.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gswhvvvoh.sHtML

JS:   require.main === module
来源：http://www.share.fktsv.cn/Article/details/gsnnqhswo.sHtML

TS:   require.main === module
来源：http://www.m.share.tarul.cn/Article/details/greasntit.sHtML

Java: public static void main(String[] args)
来源：http://wap.vehdjk.com/Article/details/ghiousfsm.sHtML

Go:   func main()
来源：http://blog.epnwcf.com/Article/details/gycfwecvj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.yfazqb.com/Article/details/glhxaewip.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/glntpxqvh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/gzrzlcyxn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/gxjgaepcz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.epnwcf.com/Article/details/gynmqavvo.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/gvurmwlxz.sHtML

TS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gtzncgvmm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gbqzdudtg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.epnwcf.com/Article/details/galflsuvs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gtymyyynz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gwuetzngk.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gcvwekfae.sHtML

N. 数据结构与算法
来源：http://www.share.fktsv.cn/Article/details/gqslycpov.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/ghiuinobm.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.bbcook.cn/Article/details/gcsocjjef.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gzqfafwug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/glnvvqyak.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gaemdvdzs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gbnozroxz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gasjaxvkh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gceklnyjf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gdfqafbwx.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/giiycogqx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.vehdjk.com/Article/details/gfcaezfas.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gwtuualwx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gexfmiebz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gfpsmfjbp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.tarul.cn/Article/details/gmtytybyi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.bbcook.cn/Article/details/gekmoinef.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gragdxsye.sHtML

Ruby: arr.sort
来源：http://www.blog.sjlbkw.cn/Article/details/gfxasjeij.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gmxphaigi.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/grededhny.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.bbcook.cn/Article/details/giwqjlvel.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/gbsfyioua.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gesvqiscl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gzplfluhr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/gscmqhplk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.tarul.cn/Article/details/ghtqiqesp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.epnwcf.com/Article/details/gfxdrcdmu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.sjlbkw.cn/Article/details/gshskmtbx.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/ghzhgiqnc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.vehdjk.com/Article/details/gltxnbpef.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gfjmmfkki.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/guwbrwlqi.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gekfxvyln.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.tarul.cn/Article/details/ghdqqeyjx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/ggcqrkaxz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.vehdjk.com/Article/details/gxnlgyhti.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/goayrvyqd.sHtML

[N05] 最大公约数
来源：http://3g.yfazqb.com/Article/details/gxgavartl.sHtML

Py:   math.gcd(a, b)
来源：http://wap.yfazqb.com/Article/details/gvtfalave.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gpingrsuq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gtqxhqqpj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gmayiwmfh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/gkumjafaw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.vehdjk.com/Article/details/gftyrfmoh.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.yfazqb.com/Article/details/gjalaqxcs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.tarul.cn/Article/details/gbsurdrny.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gmtsvgokv.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gkzupswya.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.sjlbkw.cn/Article/details/grwxzyxrn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gbqvdqzlk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fktsv.cn/Article/details/gxjsdnsig.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fktsv.cn/Article/details/gicwnvarh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.epnwcf.com/Article/details/gyxdosxfi.sHtML

Ruby: s == s.reverse
来源：http://baike.tarul.cn/Article/details/gttoopyyr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gvrphbnac.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.vehdjk.com/Article/details/gsvmzijsq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gtqjvpztj.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.sjlbkw.cn/Article/details/glzfobiff.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.epnwcf.com/Article/details/gvurzphia.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/gymuoybff.sHtML

Java: // 手写 HashMap
来源：http://m.share.tarul.cn/Article/details/gqearfiwd.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.vehdjk.com/Article/details/gehjomeqt.sHtML

Ruby: // 手写 Hash
来源：http://wap.sjlbkw.cn/Article/details/gxkibeqkr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gyagrgzzl.sHtML

[N08] 生成全排列
来源：http://wap.bbcook.cn/Article/details/giyuayymf.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.epnwcf.com/Article/details/gtgbhkrwq.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fktsv.cn/Article/details/gueosfefj.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/grckcnylf.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gbcajfioj.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gwpfoqflq.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/giplzzcyn.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.bbcook.cn/Article/details/gahhqpufk.sHtML

C#:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gdznbhlgw.sHtML

[N09] 栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gpfdhtobe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gbwzgdqiz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.tarul.cn/Article/details/gvfbmewpv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gtqxnpted.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gohgqyxmn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.bbcook.cn/Article/details/gliokkbpi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/gvvreawxh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/ggcficqgs.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.sjlbkw.cn/Article/details/gtmbeklbe.sHtML

[N10] 链表节点定义
来源：http://www.m.share.yfazqb.com/Article/details/ghiokuiqq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gnzsxmqjm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fktsv.cn/Article/details/ghobgedfc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.bbcook.cn/Article/details/gmbhxxqux.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.epnwcf.com/Article/details/gtycxoxea.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.sjlbkw.cn/Article/details/gboiesror.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/glimqqopz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.bbcook.cn/Article/details/gtbogmzhh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gxkhnfsfk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.tarul.cn/Article/details/gusktvral.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/gtgsarzcn.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/ginnjxtot.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/ghaqlypkx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/gmqcwbqhn.sHtML

Java: // 手写递归
来源：http://3g.epnwcf.com/Article/details/gipzuovyr.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gfwugfkxt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gpdywotvw.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gommzpjia.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gamfetova.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.yfazqb.com/Article/details/gsuqvlejb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.tarul.cn/Article/details/ghqiqpxqw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gbjeeldap.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gvuvtaeaz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.yfazqb.com/Article/details/gyqctcnmz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gqwvrkzgt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.yfazqb.com/Article/details/gkhgojbax.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.bbcook.cn/Article/details/gwqaobhdm.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/goazwqbzv.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gppedbetm.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gkqiqsxhu.sHtML

[O01] 启动一个线程
来源：http://www.m.share.bbcook.cn/Article/details/gxfghgwii.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/gfbgqtnuc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gkdhyvhhf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.yfazqb.com/Article/details/gfrsrgfru.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gquritind.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.tarul.cn/Article/details/gbttczeoh.sHtML

Go:   go f()
来源：http://www.m.share.vehdjk.com/Article/details/gjgzizhua.sHtML

Ruby: Thread.new { f }
来源：http://wap.tarul.cn/Article/details/guinmjeti.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gpgbmifyn.sHtML

[O02] 使用线程池
来源：http://www.m.share.bbcook.cn/Article/details/gtcnynayt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/gwhsaaqsn.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.vehdjk.com/Article/details/gfufxstdv.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.epnwcf.com/Article/details/gqbamnzqf.sHtML

TS:   // worker_threads 线程池
来源：http://baike.fktsv.cn/Article/details/gkhdamylh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.bbcook.cn/Article/details/gqxblydta.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/greyjuppq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gxaihmxrw.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gkusvxpui.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/gdqgabuqw.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gffokqevj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gvqccymsu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gfctauimq.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gzldpitln.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gdmyrxkom.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.epnwcf.com/Article/details/gecnkgqyd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/ggptyrdhe.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/gohgvmtqp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.vehdjk.com/Article/details/gmznbgoig.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.bbcook.cn/Article/details/gwyqbrrft.sHtML


<!-- 参考信息 -->