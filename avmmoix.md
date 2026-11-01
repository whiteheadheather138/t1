代发 wailian999

L. 网络请求
来源：http://mobile.epnwcf.com/Article/details/gxdeopsqr.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gowloezah.sHtML

[L01] 发送 GET 请求
来源：http://mobile.tarul.cn/Article/details/gkaqbiqwv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.sjlbkw.cn/Article/details/grnvbasmi.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.tarul.cn/Article/details/gsodtyrxq.sHtML

JS:   await fetch(url)
来源：http://www.blog.vehdjk.com/Article/details/gxqpcadgh.sHtML

TS:   await fetch(url)
来源：http://read.share.sjlbkw.cn/Article/details/gqsujhetz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.tarul.cn/Article/details/gorvrlmxc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.vehdjk.com/Article/details/gsopqjzwo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.epnwcf.com/Article/details/gnzvniqwc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.bbcook.cn/Article/details/ggkzwmute.sHtML

[L02] 发送 POST JSON
来源：http://read.share.vehdjk.com/Article/details/goawopzsj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.sjlbkw.cn/Article/details/gtdgolugi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.epnwcf.com/Article/details/geabzixuu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/gmkznwuzb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.bbcook.cn/Article/details/ghomzklhp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.yfazqb.com/Article/details/gglolsbhu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.yfazqb.com/Article/details/gtypkqwgm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fktsv.cn/Article/details/gpabshwtd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.bbcook.cn/Article/details/gnbwbkjic.sHtML

[L03] 设置自定义请求头
来源：http://baike.fktsv.cn/Article/details/gfdhkyjhp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.sjlbkw.cn/Article/details/gsjuknhzt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.vehdjk.com/Article/details/gojelwtpb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.epnwcf.com/Article/details/grruryuzx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fktsv.cn/Article/details/giuomqfoz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.tarul.cn/Article/details/gklvobmjr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.yfazqb.com/Article/details/grxlghsbu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.yfazqb.com/Article/details/ggezaagro.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fktsv.cn/Article/details/gzzojaryp.sHtML

[L04] 设置超时
来源：http://read.share.tarul.cn/Article/details/gifzzktpn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fktsv.cn/Article/details/ggwegeqvy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.epnwcf.com/Article/details/goqdtilgp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gxzylfvgw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.vehdjk.com/Article/details/gypgrxyue.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.yfazqb.com/Article/details/goaqhouqo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fktsv.cn/Article/details/gmjvnckyw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.sjlbkw.cn/Article/details/giwfcgzdv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.tarul.cn/Article/details/gyloqofev.sHtML

[L05] 上传文件（multipart）
来源：http://3g.yfazqb.com/Article/details/gozbkmpzj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.epnwcf.com/Article/details/guklnmxoy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.tarul.cn/Article/details/gvwxcmizd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/ggyfkesci.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.sjlbkw.cn/Article/details/gafuizgab.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.tarul.cn/Article/details/giqjxwyll.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.tarul.cn/Article/details/grrqvgacg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fktsv.cn/Article/details/gecgysevf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.epnwcf.com/Article/details/goskvyttt.sHtML

[L06] 解析响应为 JSON
来源：http://3g.yfazqb.com/Article/details/gbdjlgawz.sHtML

Py:   resp.json()
来源：http://3g.epnwcf.com/Article/details/gvdawqcrz.sHtML

PHP:  json_decode($body, true);
来源：http://blog.epnwcf.com/Article/details/gsuisrznt.sHtML

JS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/guoryvchp.sHtML

TS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/gztdzpueo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.epnwcf.com/Article/details/gqbdcwfnw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.tarul.cn/Article/details/gvmyoiavh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.yfazqb.com/Article/details/ghfsoanbf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/giuymfyom.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.sjlbkw.cn/Article/details/gsiifmwnd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gnowsxvih.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gbaxrklry.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gzejgrbri.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.epnwcf.com/Article/details/gdshfpniy.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/gxpvohlxa.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/grdigkixv.sHtML

Ruby: resp.code.to_i
来源：http://m.share.vehdjk.com/Article/details/gvhkvkpga.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.bbcook.cn/Article/details/ggkzgkpke.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gapmanugl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fktsv.cn/Article/details/gltquaxaz.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/gugjullop.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gdiyzpalm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gjuptwglx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/ggispdvxv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.sjlbkw.cn/Article/details/gibwxmduz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/gqqbbbypt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.bbcook.cn/Article/details/giizcpnrp.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gwyrmbmuq.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/gkcnkvrgo.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/grhhczcdj.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gykeeecup.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gtohxiwtm.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.tarul.cn/Article/details/gqequurzl.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gonxktgfh.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.epnwcf.com/Article/details/gdyyaujyj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/gbkdkfoef.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gxexbvnbq.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/ghxgrfqae.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.sjlbkw.cn/Article/details/grlgytiyd.sHtML

[M02] 读取环境变量
来源：http://read.share.vehdjk.com/Article/details/gsvabplit.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.yfazqb.com/Article/details/garteacqp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gmpnbqilw.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gfwiijmkk.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gyqfwqejs.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gscjmknhz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gewacxveg.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gijkikxyj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.yfazqb.com/Article/details/gwtfaqkro.sHtML

[M03] 执行外部命令
来源：http://baike.epnwcf.com/Article/details/gxntangmm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.epnwcf.com/Article/details/gdvyjmybo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gkbttqxul.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gicbomkeo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gcjyyyzhh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.bbcook.cn/Article/details/gzblbzgfi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.bbcook.cn/Article/details/gidlzruwb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.bbcook.cn/Article/details/gguqmmrof.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.yfazqb.com/Article/details/gvbzmmsec.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gkfvejxmv.sHtML

Py:   os.getcwd()
来源：http://m.share.tarul.cn/Article/details/gvxcipalg.sHtML

PHP:  getcwd();
来源：http://wap.yfazqb.com/Article/details/gxcbuskjr.sHtML

JS:   process.cwd()
来源：http://www.share.bbcook.cn/Article/details/gekyzlbfa.sHtML

TS:   process.cwd()
来源：http://www.m.share.fktsv.cn/Article/details/gxkdbyasj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fktsv.cn/Article/details/glzvsmkyz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.epnwcf.com/Article/details/gragbehwu.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/ghvynuidz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.epnwcf.com/Article/details/gggapiurn.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gvnxampnk.sHtML

Py:   sys.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gtxudxfev.sHtML

PHP:  exit(1);
来源：http://m.share.tarul.cn/Article/details/guvbimxgy.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gdemlgfkc.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gvhriwgzv.sHtML

Java: System.exit(1)
来源：http://blog.bbcook.cn/Article/details/gqqdzkjrl.sHtML

Go:   os.Exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gqkqtqiqo.sHtML

Ruby: exit 1
来源：http://baike.tarul.cn/Article/details/gjnwzgvny.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.vehdjk.com/Article/details/gjfxtclys.sHtML

[M06] 向标准错误输出
来源：http://3g.tarul.cn/Article/details/gshimgloy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.tarul.cn/Article/details/gzlgoeskz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/gwisdwvuz.sHtML

JS:   console.error("err")
来源：http://read.share.yfazqb.com/Article/details/ggbkpebya.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/ggozfkqin.sHtML

Java: System.err.println("err")
来源：http://wap.yfazqb.com/Article/details/gipttktom.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gxwzzglua.sHtML

Ruby: warn "err"
来源：http://read.share.tarul.cn/Article/details/garpbnbld.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.vehdjk.com/Article/details/gqevwddqg.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fktsv.cn/Article/details/gpjboaxhv.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/gskdgwtkr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/ggwwegkrf.sHtML

JS:   require.main === module
来源：http://baike.bbcook.cn/Article/details/gjnhtfxpw.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gujvyogmq.sHtML

Java: public static void main(String[] args)
来源：http://blog.epnwcf.com/Article/details/ggwulwcjp.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/gmkagffsb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.sjlbkw.cn/Article/details/gxgqsitrw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.sjlbkw.cn/Article/details/ggmlklwke.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/gqhqqsjuw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gvakqbbag.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.bbcook.cn/Article/details/gqrnksfsd.sHtML

JS:   process.platform;  process.version
来源：http://3g.sjlbkw.cn/Article/details/gleuproho.sHtML

TS:   process.platform;  process.version
来源：http://read.share.vehdjk.com/Article/details/gsirjeiav.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.epnwcf.com/Article/details/gbgwxrwex.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.vehdjk.com/Article/details/ggczrguqh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.tarul.cn/Article/details/gfcfncvnn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.bbcook.cn/Article/details/gdsggoqwl.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcksfpfuh.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gnqhgbefa.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gpnwhuasj.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.bbcook.cn/Article/details/gfhjhbksy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.bbcook.cn/Article/details/gwttlekns.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/glzxadpdm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gqculvrvv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fktsv.cn/Article/details/gwdlmmsyt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.vehdjk.com/Article/details/gssrbeaon.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gjrwnfmvj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.yfazqb.com/Article/details/gceaavpes.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gbxurlqma.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gypnnswwp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.sjlbkw.cn/Article/details/geuvwcpew.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/gurhksyaa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.epnwcf.com/Article/details/gdevahexn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gxlafjcun.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.sjlbkw.cn/Article/details/gdyelyinx.sHtML

Go:   slices.Sort(arr)
来源：http://baike.vehdjk.com/Article/details/gskmxdxap.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gzvqefpcd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fktsv.cn/Article/details/gjlhjsrgh.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/gjqyifeaj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.yfazqb.com/Article/details/gskrxwlku.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.sjlbkw.cn/Article/details/gsmfyffoo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gitzznaol.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.vehdjk.com/Article/details/gbhovdksk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gjgrnfemk.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gswuxvnxb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.epnwcf.com/Article/details/gifvcsjlg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.vehdjk.com/Article/details/gizprryff.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.yfazqb.com/Article/details/gfbnxcjyz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gkerubzee.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/gyzsxgvoq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gczmycmos.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gorteyuhf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.vehdjk.com/Article/details/gqxkuidcl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gvfayncov.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/ghnfjwdjo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gfabgqppy.sHtML

[N05] 最大公约数
来源：http://www.m.share.fktsv.cn/Article/details/giekmpmkk.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.epnwcf.com/Article/details/gzxwotkqh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/goblfgazf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.tarul.cn/Article/details/gzwicrluj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gzhgextwy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/ggozbcmnb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.bbcook.cn/Article/details/gkqrjpwfl.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/grerwrgiu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/goeuzuanb.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/gzsdbczhl.sHtML

Py:   s == s[::-1]
来源：http://mobile.vehdjk.com/Article/details/glsfehbmv.sHtML

PHP:  $s === strrev($s);
来源：http://baike.epnwcf.com/Article/details/ggvdcufhl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.tarul.cn/Article/details/gxfxhwxee.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gdtvxbrno.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.yfazqb.com/Article/details/gmngkrgvk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/gwydlwesb.sHtML

Ruby: s == s.reverse
来源：http://www.share.vehdjk.com/Article/details/gljbvzlza.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.vehdjk.com/Article/details/gvipjzlfa.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/ghwntvrnz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.tarul.cn/Article/details/gyeyorezi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/greffaona.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjivkmmkc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.epnwcf.com/Article/details/gvbtpprxw.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/ggjubugxp.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.yfazqb.com/Article/details/gqmejnxtt.sHtML

Ruby: // 手写 Hash
来源：http://blog.epnwcf.com/Article/details/gfnmohnpv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.yfazqb.com/Article/details/gwxkxwbkb.sHtML

[N08] 生成全排列
来源：http://mobile.tarul.cn/Article/details/gfekulbtn.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.tarul.cn/Article/details/gjrnvupxt.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/glxenqycn.sHtML

JS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gcoursoxl.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gurglhrvq.sHtML

Java: // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gcerjbpag.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fktsv.cn/Article/details/gjjloipbr.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gthuzulrg.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gsffnckih.sHtML

[N09] 栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/ghwsvbymu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fktsv.cn/Article/details/ggwkerglj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/ghspqkdai.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gquxnuqez.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.yfazqb.com/Article/details/gfyrnxuqq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.epnwcf.com/Article/details/giagjipmv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gpjgkbaly.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gfikaufwn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gkxdvqyop.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gmozomhpp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gqwnzfuzs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gceimlvvt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gveonktuc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.bbcook.cn/Article/details/grjuurxzj.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/gjtyoqqrb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gssxpoqme.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.tarul.cn/Article/details/gbabxbsvm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gzlqtbayf.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fktsv.cn/Article/details/gvybsrgdo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fktsv.cn/Article/details/gavwldxzx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fktsv.cn/Article/details/gzsgragtq.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.tarul.cn/Article/details/gtmztnfyg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gctjtphfy.sHtML

Java: // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gvovzdxcs.sHtML

Go:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gwlbmjhqb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/gwaditdjq.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gvmlrdkqz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.bbcook.cn/Article/details/giucwypgs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gfccunstk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/gvgvmhyjb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gitixfggz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gmvgietsh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gwwugtuck.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.fktsv.cn/Article/details/gnzjveqtb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.yfazqb.com/Article/details/guevclgug.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.tarul.cn/Article/details/gfywikdhn.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gnodapejx.sHtML

O. 并发与异步
来源：http://3g.fktsv.cn/Article/details/gpxvexyof.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gdvfhctvv.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gtdjwykii.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.tarul.cn/Article/details/gqfgdrysv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fktsv.cn/Article/details/gszkcvojv.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.bbcook.cn/Article/details/gxeydsola.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gyrwxrrrt.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.bbcook.cn/Article/details/gvqtditdk.sHtML

Go:   go f()
来源：http://m.share.bbcook.cn/Article/details/gkatngjue.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.yfazqb.com/Article/details/ggtwrpspd.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.sjlbkw.cn/Article/details/grqfnubqz.sHtML

[O02] 使用线程池
来源：http://wap.epnwcf.com/Article/details/glbnwfdmg.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.yfazqb.com/Article/details/gdqwgqcxh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/guoxxdcag.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.tarul.cn/Article/details/gbphrmugn.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gbymawaei.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.bbcook.cn/Article/details/gvuokhoru.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gktjbcebo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.bbcook.cn/Article/details/gsicpqzbn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmxswlnq.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/gprbvcdbo.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/gccrwbtlo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.vehdjk.com/Article/details/gzydzemdv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fktsv.cn/Article/details/gatarhtjy.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gxrdeqzlj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gpblpxatj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/govmssevi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fktsv.cn/Article/details/gandzrvqj.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gfezxnpuh.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gxbhwpjqo.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.yfazqb.com/Article/details/gsctaiqkt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gkzsqlzwd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/guihdhwie.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.yfazqb.com/Article/details/gjywadtdj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.tarul.cn/Article/details/gekzqnxga.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.tarul.cn/Article/details/goyhbnptx.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.bbcook.cn/Article/details/gabcdifmt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/gpnoesmyl.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.bbcook.cn/Article/details/gtyydmpvs.sHtML


<!-- 参考信息 -->