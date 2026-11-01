代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.yfazqb.com/Article/details/gkhdyccxb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.bbcook.cn/Article/details/grbtjnuph.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.tarul.cn/Article/details/gsjilsdin.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.bbcook.cn/Article/details/ggybgwjuu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.sjlbkw.cn/Article/details/gwvrjvtjy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.epnwcf.com/Article/details/gmxnbslok.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gamuyaswh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.vehdjk.com/Article/details/ggzzsjjbv.sHtML

Go:   encoding/gob
来源：http://www.m.share.vehdjk.com/Article/details/gklsygapj.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.epnwcf.com/Article/details/gktutnval.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.sjlbkw.cn/Article/details/gmnbfewbu.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbzqumzda.sHtML

L. 网络请求
来源：http://wap.yfazqb.com/Article/details/gnvqcgvii.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gbilwlptq.sHtML

[L01] 发送 GET 请求
来源：http://blog.sjlbkw.cn/Article/details/ggkagjylu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fktsv.cn/Article/details/gtylizliq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.vehdjk.com/Article/details/gwhxlkocc.sHtML

JS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gsrxwebjc.sHtML

TS:   await fetch(url)
来源：http://www.blog.epnwcf.com/Article/details/gotamrdse.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.epnwcf.com/Article/details/gbgqexxii.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.sjlbkw.cn/Article/details/geaszirtw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.tarul.cn/Article/details/gurszfiss.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.epnwcf.com/Article/details/gdqdlaaxk.sHtML

[L02] 发送 POST JSON
来源：http://mobile.yfazqb.com/Article/details/gijmztlua.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.vehdjk.com/Article/details/gigzvtmmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.tarul.cn/Article/details/gibnkidmt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.yfazqb.com/Article/details/grriymofq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.vehdjk.com/Article/details/gwequkgxc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.tarul.cn/Article/details/gnwzmwasb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.vehdjk.com/Article/details/gswbubvvw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.bbcook.cn/Article/details/gpptyubno.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.epnwcf.com/Article/details/gyprbopbc.sHtML

[L03] 设置自定义请求头
来源：http://wap.epnwcf.com/Article/details/gryvmsdut.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fktsv.cn/Article/details/gcsdotcma.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.epnwcf.com/Article/details/ghnrhqcxd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.tarul.cn/Article/details/gydeqfszu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gispzyfob.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.yfazqb.com/Article/details/gfjvknbro.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/ghircovwr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.tarul.cn/Article/details/gselrswuc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.yfazqb.com/Article/details/ghdfebldo.sHtML

[L04] 设置超时
来源：http://wap.yfazqb.com/Article/details/gdaqawhea.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.yfazqb.com/Article/details/gswltrjcg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fktsv.cn/Article/details/ghxrslfye.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.sjlbkw.cn/Article/details/geuddbjsj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.bbcook.cn/Article/details/gxecmcbrl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.tarul.cn/Article/details/gurpleerp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.yfazqb.com/Article/details/gulgcbxvx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fktsv.cn/Article/details/ggtwltqbo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.vehdjk.com/Article/details/gcuamwkoi.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.tarul.cn/Article/details/gisrrecss.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.bbcook.cn/Article/details/gftenkids.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.sjlbkw.cn/Article/details/gjbnplttm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.yfazqb.com/Article/details/gkrhgpqnp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gyjrkhcco.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.tarul.cn/Article/details/gthrsiktj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.vehdjk.com/Article/details/gikelscww.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.sjlbkw.cn/Article/details/gzyhmhpqv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/grudygpsd.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.bbcook.cn/Article/details/goucgfdbb.sHtML

Py:   resp.json()
来源：http://read.share.vehdjk.com/Article/details/gxuocuyra.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.tarul.cn/Article/details/gdwjxxnwk.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/gohzldkat.sHtML

TS:   await resp.json()
来源：http://www.m.share.vehdjk.com/Article/details/gimsnhyoq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.tarul.cn/Article/details/gvhsucskf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fktsv.cn/Article/details/glekwzpej.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.bbcook.cn/Article/details/gzwektrkv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.sjlbkw.cn/Article/details/gvlksvlhz.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.yfazqb.com/Article/details/gawkoukyw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/groaiaeha.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/gckaiiwpd.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.yfazqb.com/Article/details/gjzkgnpwp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.sjlbkw.cn/Article/details/gswthplfb.sHtML

Java: resp.statusCode()
来源：http://wap.bbcook.cn/Article/details/gunyqzrmg.sHtML

Go:   resp.StatusCode
来源：http://read.share.vehdjk.com/Article/details/gypriplio.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gojkendto.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gecistkbd.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gkzhfkled.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gwnmnbhhz.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.yfazqb.com/Article/details/gvwneazvm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.vehdjk.com/Article/details/glrulwklf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.tarul.cn/Article/details/gkcfqmbfi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fktsv.cn/Article/details/ghbptuloq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/geqylqpem.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gqksdnybz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.yfazqb.com/Article/details/gnpcirdab.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gozkfqfdk.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/giursvcva.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gqcwztnfw.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.vehdjk.com/Article/details/gxzasvflw.sHtML

Py:   sys.argv[1:]
来源：http://wap.bbcook.cn/Article/details/gzpuufqav.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.epnwcf.com/Article/details/gxuhmkjvw.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gbiprzkak.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gnbpynodb.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gnzvzgxsz.sHtML

Go:   os.Args[1:]
来源：http://mobile.bbcook.cn/Article/details/gwkqanval.sHtML

Ruby: ARGV
来源：http://baike.fktsv.cn/Article/details/gmkrusjoq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gyausvgru.sHtML

[M02] 读取环境变量
来源：http://m.share.yfazqb.com/Article/details/gupugjgpo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/glnygpbfy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.yfazqb.com/Article/details/gnhdterwg.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gbrptjlzp.sHtML

TS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/ggcndcwwb.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gicgblrmp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.tarul.cn/Article/details/gcympmebh.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gybidxzgz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gssagelpn.sHtML

[M03] 执行外部命令
来源：http://baike.vehdjk.com/Article/details/gblslzsze.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gddkokevx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.yfazqb.com/Article/details/gmubgayxq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.yfazqb.com/Article/details/gaeswzuaj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/glkszchgp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.bbcook.cn/Article/details/gwjpdcjzt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gwjyeedty.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.tarul.cn/Article/details/gygloltsb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.epnwcf.com/Article/details/grzyzxgxq.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gdouyisnb.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gertdvvea.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gshgzstpf.sHtML

JS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gdacooioq.sHtML

TS:   process.cwd()
来源：http://www.m.share.yfazqb.com/Article/details/gakdgjxfv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gvfrwkfpx.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gjovlptiz.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/gtlmuqrow.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.yfazqb.com/Article/details/glmcpmkux.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gqkpfknnx.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gcrwjwyvq.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/goxegwutp.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/ggmqmviag.sHtML

TS:   process.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gekzkmgit.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/guadtbhoq.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/gppyuqamk.sHtML

Ruby: exit 1
来源：http://3g.yfazqb.com/Article/details/gtxtnnjgo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.epnwcf.com/Article/details/gaznuvhrw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/guxthupbl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gbfyssqze.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gkisflwrv.sHtML

JS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gwenmxhix.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gsokjmcra.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/gjsguvlxi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gwurxawjk.sHtML

Ruby: warn "err"
来源：http://m.share.epnwcf.com/Article/details/gihtwyerq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fktsv.cn/Article/details/gxalfsjbl.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.bbcook.cn/Article/details/gpkzsxmvb.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fktsv.cn/Article/details/gfimwrmod.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.sjlbkw.cn/Article/details/gbtzquyse.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gxwafppsb.sHtML

TS:   require.main === module
来源：http://blog.vehdjk.com/Article/details/gcsyitdzx.sHtML

Java: public static void main(String[] args)
来源：http://m.share.vehdjk.com/Article/details/gumceusrs.sHtML

Go:   func main()
来源：http://mobile.tarul.cn/Article/details/gkyuliaro.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/gaizwocne.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gscbpsedp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.yfazqb.com/Article/details/goxaxxyzo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/ginaamahi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gkcxrhtoe.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fktsv.cn/Article/details/gctnoncnf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gpociiasv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.epnwcf.com/Article/details/gxwynwhrc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.vehdjk.com/Article/details/gcbbyebbu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fktsv.cn/Article/details/gwsnajudb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/gpboumlcl.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gfdblyyvu.sHtML

N. 数据结构与算法
来源：http://www.share.sjlbkw.cn/Article/details/geaosqnxj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gkfbbnkni.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gijkigamn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gingwmrej.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gnlxkojhj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gmprekszw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gaujhwkdx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gfvppabky.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/ghxgjmqqf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gpztamwyv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.tarul.cn/Article/details/gyjkfkkwd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/gasuyefra.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/gwpzzynrr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/ghgvvaqck.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gdmimvzlk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gnuysvggf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fktsv.cn/Article/details/gejwgvvvz.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gjrhtgslo.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/gdhxiqliw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.vehdjk.com/Article/details/glcfyvbzk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.vehdjk.com/Article/details/gmrbfrtqy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gyijagfwk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.yfazqb.com/Article/details/gtyrqflci.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.bbcook.cn/Article/details/gdxubskof.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gkelzecnt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.epnwcf.com/Article/details/gjqgtusdx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.yfazqb.com/Article/details/geeaqjwje.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.tarul.cn/Article/details/gaenbswkl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gyqzvpvdw.sHtML

[N04] 斐波那契数列
来源：http://3g.fktsv.cn/Article/details/gbzxhhpwf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.bbcook.cn/Article/details/gfdxtdcgr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gmxbadpnv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gzockhnif.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gpysftxzy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.sjlbkw.cn/Article/details/gtqawfbyf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gisabhpoj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.sjlbkw.cn/Article/details/gtdopjblz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/glajchvjq.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/gbgpnlijc.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/goaxsndgn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/gvdcccqot.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gwzwosvmb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gnbhdrhmh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.epnwcf.com/Article/details/gbuqfgftl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.sjlbkw.cn/Article/details/gzzvqshqd.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/gaknnnzos.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.bbcook.cn/Article/details/gwfrwopuu.sHtML

[N06] 判断回文字符串
来源：http://baike.vehdjk.com/Article/details/ggqmdiuee.sHtML

Py:   s == s[::-1]
来源：http://m.share.tarul.cn/Article/details/gllvhtvdu.sHtML

PHP:  $s === strrev($s);
来源：http://wap.bbcook.cn/Article/details/glmdflufv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fktsv.cn/Article/details/gxjlooyyb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.epnwcf.com/Article/details/gxlxpppvk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.vehdjk.com/Article/details/gtkrbxobq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.sjlbkw.cn/Article/details/gdrpzqmpi.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gxbpnmfwi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fktsv.cn/Article/details/gjrrvcjgd.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gdvouioia.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/glxhneypa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/grnvjufin.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.tarul.cn/Article/details/gchraurao.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fktsv.cn/Article/details/gftcoxlaj.sHtML

Java: // 手写 HashMap
来源：http://read.share.bbcook.cn/Article/details/gwgltrdiw.sHtML

Go:   // 手写 map[int]int
来源：http://wap.vehdjk.com/Article/details/gvczowqgn.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.yfazqb.com/Article/details/gdeudhkdt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.tarul.cn/Article/details/gwcwdedsd.sHtML

[N08] 生成全排列
来源：http://blog.bbcook.cn/Article/details/gmsjefyvf.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/grjpoacgm.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/guanvqokg.sHtML

JS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gslxtzmns.sHtML

TS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gqcmmzwpx.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/gdawvfgow.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/glphoilbc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gsomzdiir.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gdstbtrrv.sHtML

[N09] 栈与队列
来源：http://wap.sjlbkw.cn/Article/details/gnoyvnikr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.vehdjk.com/Article/details/goitaactz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gbqiisurh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.epnwcf.com/Article/details/ghqricwir.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fktsv.cn/Article/details/gvpfnyylh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gzntipqum.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.fktsv.cn/Article/details/guiewqxwe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gtahsqdys.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.vehdjk.com/Article/details/gdzwtgwks.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gqwyjuyne.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.epnwcf.com/Article/details/gxzyopqxn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.yfazqb.com/Article/details/gqcgphsbf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.tarul.cn/Article/details/gdfrdpkjx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.vehdjk.com/Article/details/gdacvfmve.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/gwdfbelza.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.yfazqb.com/Article/details/gtcmbqlpw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gddqnqyql.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/ggxzbwmut.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.fktsv.cn/Article/details/gtjtwmtqk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.vehdjk.com/Article/details/gkasbsoct.sHtML

PHP:  // 手写递归函数
来源：http://wap.fktsv.cn/Article/details/grlsudizo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fktsv.cn/Article/details/ganbziuld.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gtaykpoct.sHtML

Java: // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gpppqvimm.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gypvgnltu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gyuylfyoj.sHtML

C#:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gcpqlfins.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.epnwcf.com/Article/details/gogeqdkgk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gislmarhl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.bbcook.cn/Article/details/gtswrepdo.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gaxdlikig.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gvhsckngk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gprqbivny.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.vehdjk.com/Article/details/gkronrisr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.sjlbkw.cn/Article/details/gimwdzxiq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fktsv.cn/Article/details/glwjvmlaz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gepoberpm.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/guogvmuvp.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gvhelujki.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/gljfldcul.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/grensgvtc.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.yfazqb.com/Article/details/gehltmafa.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/gukvwdcca.sHtML

TS:   // 同 JS
来源：http://www.blog.tarul.cn/Article/details/gujnywmot.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.yfazqb.com/Article/details/giazcwyjw.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gndfetyad.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fktsv.cn/Article/details/gcsygnvkx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gwfsudyiv.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/guvujvtbc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gzxsqpntg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.vehdjk.com/Article/details/gibxiukmv.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.tarul.cn/Article/details/gtywvyyhj.sHtML

TS:   // worker_threads 线程池
来源：http://blog.epnwcf.com/Article/details/gscefeizp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.tarul.cn/Article/details/gmybcyvnk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/guozctmwe.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fktsv.cn/Article/details/giiyopshz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.epnwcf.com/Article/details/gmrjltghq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.epnwcf.com/Article/details/gfahliyaa.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/gmjpedtsc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.yfazqb.com/Article/details/gfwbrsceq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gvipxuyhj.sHtML

TS:   // 同 JS
来源：http://3g.sjlbkw.cn/Article/details/gsrjujwka.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fktsv.cn/Article/details/gflyllpjp.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.sjlbkw.cn/Article/details/gvnybgync.sHtML


<!-- 参考信息 -->