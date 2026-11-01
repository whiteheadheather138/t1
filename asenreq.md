代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gtqacucif.sHtML

JS:   await fetch(url)
来源：http://m.share.vehdjk.com/Article/details/ghmmezrnw.sHtML

TS:   await fetch(url)
来源：http://www.share.bbcook.cn/Article/details/gzbcvlxac.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.yfazqb.com/Article/details/gpxxnegwm.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.tarul.cn/Article/details/giutvczmr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.tarul.cn/Article/details/ginodxqgd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.sjlbkw.cn/Article/details/gtzrbchcb.sHtML

[L02] 发送 POST JSON
来源：http://m.share.vehdjk.com/Article/details/gaskofpyn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.epnwcf.com/Article/details/gwruundbo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.vehdjk.com/Article/details/gvqdzhwuz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.epnwcf.com/Article/details/ghulawdgg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.epnwcf.com/Article/details/gkvuajxfp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fktsv.cn/Article/details/gvodotncg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.bbcook.cn/Article/details/gyvkceblf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.epnwcf.com/Article/details/gksmtyqvn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.epnwcf.com/Article/details/gtkoglydg.sHtML

[L03] 设置自定义请求头
来源：http://read.share.sjlbkw.cn/Article/details/gxusgvohe.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.epnwcf.com/Article/details/gbpfdvuii.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.vehdjk.com/Article/details/ghprgogek.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.bbcook.cn/Article/details/gsxbnrvaw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.yfazqb.com/Article/details/ginixmyqj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.epnwcf.com/Article/details/gjyhfhqgn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.sjlbkw.cn/Article/details/gvekqbgoz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.epnwcf.com/Article/details/gyytxbddz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.sjlbkw.cn/Article/details/ggkfrpmua.sHtML

[L04] 设置超时
来源：http://www.share.yfazqb.com/Article/details/geolddhus.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gponxtgin.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.yfazqb.com/Article/details/gpgrefynz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fktsv.cn/Article/details/gelqvkcvz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/ghnoqmmjc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.epnwcf.com/Article/details/gyzaycbqu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.bbcook.cn/Article/details/gapyvwwqk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.tarul.cn/Article/details/gvexubbxh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.sjlbkw.cn/Article/details/gmvueqiwa.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.yfazqb.com/Article/details/gxshxfpzo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.sjlbkw.cn/Article/details/giaekavzs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.epnwcf.com/Article/details/glxtkmddl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/goyjachpl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.bbcook.cn/Article/details/gyhztfxlg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.bbcook.cn/Article/details/gtmeswyft.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fktsv.cn/Article/details/gpktclseg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gjizruqze.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.tarul.cn/Article/details/geemqilbq.sHtML

[L06] 解析响应为 JSON
来源：http://baike.epnwcf.com/Article/details/gubnbteqw.sHtML

Py:   resp.json()
来源：http://baike.vehdjk.com/Article/details/giiftvsas.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/grfvnshnz.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gejqlvlhu.sHtML

TS:   await resp.json()
来源：http://www.share.tarul.cn/Article/details/gzjfvkgsf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gpkjfvhih.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.sjlbkw.cn/Article/details/gowrmutnk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gfjlclcij.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.vehdjk.com/Article/details/gukcjbtum.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/guotzptui.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.vehdjk.com/Article/details/gmyvyhkpe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.bbcook.cn/Article/details/grjsykige.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.epnwcf.com/Article/details/gejblzzlp.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.tarul.cn/Article/details/gwbxlqiap.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gflrhbpmq.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.bbcook.cn/Article/details/gfdmqkmeo.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gitjkhwed.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gelbudwhf.sHtML

[L08] 并发请求多个地址
来源：http://read.share.tarul.cn/Article/details/gsghkznxd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fktsv.cn/Article/details/gliqizvdq.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.bbcook.cn/Article/details/gstnvmvgu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gvajszasu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.sjlbkw.cn/Article/details/gdidonlcm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.tarul.cn/Article/details/grleihudg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.epnwcf.com/Article/details/gcfuzneab.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.tarul.cn/Article/details/gfxcshcsf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.vehdjk.com/Article/details/gfpqkbtbj.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/geennrkfx.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/ghninfqfr.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gttxltzsy.sHtML

[M01] 读取命令行参数
来源：http://blog.bbcook.cn/Article/details/gvwreabqh.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.yfazqb.com/Article/details/gfffzfraj.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.tarul.cn/Article/details/gxlqsaxgf.sHtML

JS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gnsbcnvti.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/gorqtjzcx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.yfazqb.com/Article/details/gdnklbrcd.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gewxaekzo.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/gsqfeoacn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gjeknxrdf.sHtML

[M02] 读取环境变量
来源：http://www.m.share.vehdjk.com/Article/details/gmidckkhj.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gkxmmgndn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gyhkywxnb.sHtML

JS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gqjdgoamu.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gopzmiwjl.sHtML

Java: System.getenv("HOME")
来源：http://3g.fktsv.cn/Article/details/ghvcqojxn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gaaysffti.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/gdzzqblxg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.yfazqb.com/Article/details/gnrrjynsv.sHtML

[M03] 执行外部命令
来源：http://read.share.tarul.cn/Article/details/guptqadkq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.bbcook.cn/Article/details/giszbjiat.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gaaboetvo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fktsv.cn/Article/details/ghzgnxzho.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfwuhjle.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gdwxnbmwc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gkiqcoxtt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.epnwcf.com/Article/details/gahzwkebz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.bbcook.cn/Article/details/gerfxpijq.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gqnkkpsii.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/gixstzodk.sHtML

PHP:  getcwd();
来源：http://blog.tarul.cn/Article/details/gtimagtgw.sHtML

JS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gtnkscbkh.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gqceqfzth.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gpkrzfcsz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.vehdjk.com/Article/details/glxomklwz.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gbuqefoaz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.tarul.cn/Article/details/guakoicei.sHtML

[M05] 设置退出码
来源：http://www.share.tarul.cn/Article/details/ggoguxrln.sHtML

Py:   sys.exit(1)
来源：http://wap.yfazqb.com/Article/details/grlofmzmv.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gbanfgswg.sHtML

JS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gzabxjoil.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gkolkwgow.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/gpfjhqdmh.sHtML

Go:   os.Exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gcxoflzya.sHtML

Ruby: exit 1
来源：http://mobile.vehdjk.com/Article/details/gttmtwdrh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.bbcook.cn/Article/details/ggspmxovo.sHtML

[M06] 向标准错误输出
来源：http://blog.vehdjk.com/Article/details/gonznacbm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.sjlbkw.cn/Article/details/gzybcawyk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gbdgjwgnf.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gdeymttum.sHtML

TS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/ggeaxboay.sHtML

Java: System.err.println("err")
来源：http://baike.vehdjk.com/Article/details/glcemhmxi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.vehdjk.com/Article/details/gimepbgcp.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gasksmvbu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/guzabnemz.sHtML

[M07] 判断是否为主入口
来源：http://blog.vehdjk.com/Article/details/gsfvswmox.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fktsv.cn/Article/details/gbvfnuoij.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.bbcook.cn/Article/details/grwzscrjb.sHtML

JS:   require.main === module
来源：http://wap.vehdjk.com/Article/details/gaahktyoj.sHtML

TS:   require.main === module
来源：http://blog.fktsv.cn/Article/details/gbvcvjdfx.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fktsv.cn/Article/details/guakzyawa.sHtML

Go:   func main()
来源：http://m.share.tarul.cn/Article/details/gtqowzmce.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.bbcook.cn/Article/details/ghzdzamyc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.tarul.cn/Article/details/grhozbusf.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.bbcook.cn/Article/details/gsyhvvawt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.epnwcf.com/Article/details/gqdkfnsje.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/goyqwqrdc.sHtML

JS:   process.platform;  process.version
来源：http://blog.fktsv.cn/Article/details/glxzsceyo.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gxotbeafl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gjsmuwhvt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/gjwlskbns.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.epnwcf.com/Article/details/gpmgphqlb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.sjlbkw.cn/Article/details/gfueiaqts.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gocwgdpts.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/guprelwmz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/ggfmvkdzd.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gigihtcme.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.tarul.cn/Article/details/gnlbylyph.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.epnwcf.com/Article/details/gbxfsnfgr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gibhdiiop.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/glqjvcgbl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gzplaiqpg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gqtgpaspj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.yfazqb.com/Article/details/ghowlputb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/grkewezvo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.epnwcf.com/Article/details/gvlhzsaxv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gsjymekte.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gcycrutvc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.bbcook.cn/Article/details/gqpjctlsj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gcanzgdox.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gadzafoun.sHtML

Go:   slices.Sort(arr)
来源：http://blog.epnwcf.com/Article/details/gkmhmdlek.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gqowlvxyk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fktsv.cn/Article/details/goeldphlx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.tarul.cn/Article/details/giyweuiev.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.tarul.cn/Article/details/gnloafdvw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.sjlbkw.cn/Article/details/gxwhnmdvd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fktsv.cn/Article/details/gzkrqimjy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/ghlukrvbx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.bbcook.cn/Article/details/gkkdjdifx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/ggdmgrecs.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gmzmyhihv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.tarul.cn/Article/details/geepuwhdp.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gjsdvknxs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/ghfybskdi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gnayyxmkl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gsbtnrkuu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/ghxyqegwm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gyxuxihxw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gvmlyfahj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gdzpxxmwn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gnykqeloe.sHtML

[N05] 最大公约数
来源：http://mobile.sjlbkw.cn/Article/details/gqbkupqvt.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fktsv.cn/Article/details/gjeajenqo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.yfazqb.com/Article/details/gqaosbyov.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gyhkovqif.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fktsv.cn/Article/details/gkgnglpfn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.sjlbkw.cn/Article/details/gqqgzavkv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.epnwcf.com/Article/details/govswwzkl.sHtML

Ruby: a.gcd(b)
来源：http://wap.tarul.cn/Article/details/gnbtxgsdi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gfwkcdqoj.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gpdwbnwcl.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gumabsvxn.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.sjlbkw.cn/Article/details/garpowyik.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fktsv.cn/Article/details/gpdyszeux.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.sjlbkw.cn/Article/details/gqxalbuwg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gbvijjzsf.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.fktsv.cn/Article/details/gltshkjus.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/guqlbblfl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gxpulxuhu.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/giosxhwxs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.yfazqb.com/Article/details/gtywpchwc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.epnwcf.com/Article/details/gviemryze.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.tarul.cn/Article/details/gibydyobl.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.bbcook.cn/Article/details/gkqasdkdy.sHtML

Java: // 手写 HashMap
来源：http://baike.bbcook.cn/Article/details/gwtutekuy.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gkiojavho.sHtML

Ruby: // 手写 Hash
来源：http://read.share.tarul.cn/Article/details/gtwyipxup.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gabtjgbce.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/guhobgosd.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.bbcook.cn/Article/details/ghzzjzfcg.sHtML

PHP:  // 手写递归交换
来源：http://3g.yfazqb.com/Article/details/glgudvrdn.sHtML

JS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gtibaghcu.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gazhssiey.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkgtbhlc.sHtML

Go:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/grsdeatrx.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gdfwqezdr.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gbqwzsmwf.sHtML

[N09] 栈与队列
来源：http://www.m.share.vehdjk.com/Article/details/gkkvyndas.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gbcjaexox.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/gjujrtuny.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/ghaovlfpt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.vehdjk.com/Article/details/ghvnolsdb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gblpabsgu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/gyhibteex.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fktsv.cn/Article/details/gxflibgfu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gbhxravza.sHtML

[N10] 链表节点定义
来源：http://wap.epnwcf.com/Article/details/gxcgqvyeg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/goyqkxpdq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.bbcook.cn/Article/details/gpaltevnb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.fktsv.cn/Article/details/gkxcjlhmr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.bbcook.cn/Article/details/grldcmbpf.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.yfazqb.com/Article/details/gzmvpzrlt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gvbjtntqh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/gzhtfuhqx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/gxkazyeyf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.vehdjk.com/Article/details/gkzwxvkxv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.epnwcf.com/Article/details/gwojhlelc.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gqijrnfam.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fktsv.cn/Article/details/gqxyejrkp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/gboirqawy.sHtML

Java: // 手写递归
来源：http://www.share.yfazqb.com/Article/details/gfplshgnj.sHtML

Go:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gricfjiqv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.epnwcf.com/Article/details/gbwqupesl.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/ghpmeofhn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.tarul.cn/Article/details/gozmtlelr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gcayhuqca.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwxkzpome.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gqmnobdlp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/ghyeilssr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gstdjtssn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.vehdjk.com/Article/details/guwxqbmjw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gqehjrrzm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gmlyspykt.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gyqmtoqtj.sHtML

O. 并发与异步
来源：http://www.share.sjlbkw.cn/Article/details/glyssfhqy.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/grbqdunvo.sHtML

[O01] 启动一个线程
来源：http://wap.vehdjk.com/Article/details/giyehhcad.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.sjlbkw.cn/Article/details/gzbmmloda.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fktsv.cn/Article/details/gzkovlhmc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.vehdjk.com/Article/details/gllpobnqm.sHtML

TS:   // 同 JS
来源：http://www.m.share.sjlbkw.cn/Article/details/gixltuzqt.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.yfazqb.com/Article/details/gxsrtdvnp.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gsknfhfgd.sHtML

Ruby: Thread.new { f }
来源：http://mobile.vehdjk.com/Article/details/guvjbxbgb.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gaakuraue.sHtML

[O02] 使用线程池
来源：http://www.share.vehdjk.com/Article/details/ghfldcgvk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.tarul.cn/Article/details/gpgpsnxxo.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.sjlbkw.cn/Article/details/grwjfyena.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gsngaisuk.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/giodrhzes.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gchcipndz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.yfazqb.com/Article/details/gahqsosls.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.sjlbkw.cn/Article/details/gqjqatnzk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.epnwcf.com/Article/details/gxcprwrqd.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/gdfbcgvzg.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gicavxctc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.epnwcf.com/Article/details/gneypeume.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.fktsv.cn/Article/details/gqydfumyg.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gixuabmbf.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gnpwozfap.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gxulveinw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gwnudbkaf.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gfhpzxflk.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gulrmczla.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.sjlbkw.cn/Article/details/gykhmyxvj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.epnwcf.com/Article/details/gjbvsfmoo.sHtML

JS:   async function f() { await g(); }
来源：http://blog.vehdjk.com/Article/details/gffgtttot.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gikassvet.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.bbcook.cn/Article/details/gwgsrvcgn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/glrbufzhs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.yfazqb.com/Article/details/gfmytkqwr.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gpgjeunry.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/giorgchug.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.bbcook.cn/Article/details/gxvstqlnn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.sjlbkw.cn/Article/details/glklbhwac.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.sjlbkw.cn/Article/details/gpvtvvizv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gfrbpxocv.sHtML


<!-- 参考信息 -->