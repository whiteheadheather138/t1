代发 wailian999

L. 网络请求
来源：http://www.share.yfazqb.com/Article/details/gunbmepyu.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/geatnnxtd.sHtML

[L01] 发送 GET 请求
来源：http://m.share.tarul.cn/Article/details/gmtnwppie.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.vehdjk.com/Article/details/gnvsrrbqs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.tarul.cn/Article/details/gsmdibyoq.sHtML

JS:   await fetch(url)
来源：http://www.share.vehdjk.com/Article/details/gposvnjvc.sHtML

TS:   await fetch(url)
来源：http://read.share.bbcook.cn/Article/details/gvnqpgpbi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.epnwcf.com/Article/details/glgrdlvmp.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.bbcook.cn/Article/details/gksjrwncl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.sjlbkw.cn/Article/details/gcgrjwanl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.tarul.cn/Article/details/gdlwrglqi.sHtML

[L02] 发送 POST JSON
来源：http://mobile.yfazqb.com/Article/details/godsqhcym.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fktsv.cn/Article/details/gkwiegwfo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.epnwcf.com/Article/details/gdcnonrjb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gjeygyojt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.bbcook.cn/Article/details/geosgvgva.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.epnwcf.com/Article/details/gkahxpryq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.epnwcf.com/Article/details/gryalbret.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.yfazqb.com/Article/details/gscfjpwhe.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fktsv.cn/Article/details/gcxhzoaem.sHtML

[L03] 设置自定义请求头
来源：http://www.share.sjlbkw.cn/Article/details/gyqfxzxuf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.sjlbkw.cn/Article/details/goatwoytz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/gywruvuhf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.epnwcf.com/Article/details/gmgkjahra.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fktsv.cn/Article/details/gmanhwvlr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fktsv.cn/Article/details/gbjbqebjh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fktsv.cn/Article/details/gnkgzdqqd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.vehdjk.com/Article/details/guopxvnlg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.yfazqb.com/Article/details/glzyquovz.sHtML

[L04] 设置超时
来源：http://www.blog.yfazqb.com/Article/details/gldnxfrdc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.epnwcf.com/Article/details/gazcvkuls.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.epnwcf.com/Article/details/gyrhjwfcr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.bbcook.cn/Article/details/griqkewct.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfqqhwbg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.tarul.cn/Article/details/gykzbqxxk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.epnwcf.com/Article/details/gdvauxdpa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gayyokbrz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.epnwcf.com/Article/details/gdhsytuzl.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fktsv.cn/Article/details/gzzksmamm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gwuagsvuj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/gkrccuqlm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.epnwcf.com/Article/details/gkpdfzqwp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.yfazqb.com/Article/details/glearwngd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.sjlbkw.cn/Article/details/glbkhbigb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.sjlbkw.cn/Article/details/gglrcvqal.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.sjlbkw.cn/Article/details/gcpfczmem.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.vehdjk.com/Article/details/gpwgcuxdh.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.epnwcf.com/Article/details/gifyviwrg.sHtML

Py:   resp.json()
来源：http://www.blog.yfazqb.com/Article/details/guoylyhci.sHtML

PHP:  json_decode($body, true);
来源：http://wap.tarul.cn/Article/details/gumgmbffl.sHtML

JS:   await resp.json()
来源：http://m.share.bbcook.cn/Article/details/gshohpomy.sHtML

TS:   await resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gkmkytzqr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fktsv.cn/Article/details/grkmyundv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.sjlbkw.cn/Article/details/gbhpnfssv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.sjlbkw.cn/Article/details/gdrbswptm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.tarul.cn/Article/details/gbqgtcice.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gkqjzlbop.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.sjlbkw.cn/Article/details/gilrgdtvu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/gzrifqrvy.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gqcplbkxi.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gmlzwvwxy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.sjlbkw.cn/Article/details/goucxbmqz.sHtML

Go:   resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gbaspzcrf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.tarul.cn/Article/details/gfzcrrfcf.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gsfjcqywf.sHtML

[L08] 并发请求多个地址
来源：http://m.share.sjlbkw.cn/Article/details/guodpqwih.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gjcrkraml.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.tarul.cn/Article/details/ggfohfanf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gmobzkedf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fktsv.cn/Article/details/gqbvvpvjj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gvwdgasqv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gkdnahobj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.vehdjk.com/Article/details/grqmfnzes.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.sjlbkw.cn/Article/details/ghdfefmmx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gukiyuxsc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.bbcook.cn/Article/details/gkwcnzxpb.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gegjxckdb.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gbrpatynn.sHtML

Py:   sys.argv[1:]
来源：http://baike.sjlbkw.cn/Article/details/gcmamzqbm.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gozflueax.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gmoynjlpz.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gsgmbmyse.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/guunafcwu.sHtML

Go:   os.Args[1:]
来源：http://www.share.vehdjk.com/Article/details/gbpkizkrb.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gemiwlqmw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gcndswtrg.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gjcefvefa.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gqsbpjaan.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/graqzxpys.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/guxjkywcg.sHtML

TS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/gucatxhov.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/glaioxxky.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.epnwcf.com/Article/details/gbcmihkcn.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.bbcook.cn/Article/details/gmeuoigxj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gxnlqklao.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gdbiemrjg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.sjlbkw.cn/Article/details/gxzaigtod.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.sjlbkw.cn/Article/details/gqqqwxipe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/geckmcgfs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.epnwcf.com/Article/details/gecojmfta.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.yfazqb.com/Article/details/geaqktizh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.sjlbkw.cn/Article/details/gwytmqlgm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fktsv.cn/Article/details/gtvkqcusn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gfskyquok.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gamdzweda.sHtML

Py:   os.getcwd()
来源：http://baike.bbcook.cn/Article/details/gwgrrqask.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gxhxaohpr.sHtML

JS:   process.cwd()
来源：http://read.share.vehdjk.com/Article/details/gvowhamyz.sHtML

TS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gtabfbwdf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gfxzjmrjc.sHtML

Go:   os.Getwd()
来源：http://3g.yfazqb.com/Article/details/ggsqzcmud.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gsdbotjzs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.sjlbkw.cn/Article/details/grgvvboqk.sHtML

[M05] 设置退出码
来源：http://blog.vehdjk.com/Article/details/gpnjsvsyo.sHtML

Py:   sys.exit(1)
来源：http://3g.vehdjk.com/Article/details/gfoqdvcik.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gvwoeduii.sHtML

JS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gwzqfsupw.sHtML

TS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/guokzexat.sHtML

Java: System.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gxzeboamt.sHtML

Go:   os.Exit(1)
来源：http://3g.tarul.cn/Article/details/gklzvkznj.sHtML

Ruby: exit 1
来源：http://www.m.share.vehdjk.com/Article/details/gkulebxyz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.yfazqb.com/Article/details/gvfcihibs.sHtML

[M06] 向标准错误输出
来源：http://read.share.sjlbkw.cn/Article/details/gsiyjlgcp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.yfazqb.com/Article/details/gwyzsdgrm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gvqtipxsx.sHtML

JS:   console.error("err")
来源：http://3g.yfazqb.com/Article/details/gggairrwg.sHtML

TS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gkljfmgnb.sHtML

Java: System.err.println("err")
来源：http://wap.bbcook.cn/Article/details/gdiftisha.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.yfazqb.com/Article/details/gthyxuxci.sHtML

Ruby: warn "err"
来源：http://www.m.share.sjlbkw.cn/Article/details/gaoichtbm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/guwgvjpfc.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.bbcook.cn/Article/details/gspoabmik.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.vehdjk.com/Article/details/ghvibmugl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gbucwxqwy.sHtML

JS:   require.main === module
来源：http://wap.fktsv.cn/Article/details/gskhfekec.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gdldpescl.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.yfazqb.com/Article/details/gunzumfkf.sHtML

Go:   func main()
来源：http://baike.vehdjk.com/Article/details/gwkegqgdt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gkyidqhyy.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gugaivqfs.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.sjlbkw.cn/Article/details/guzxcfejz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gagggznpp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.yfazqb.com/Article/details/gytdrqrwz.sHtML

JS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gcpkcbtgs.sHtML

TS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gubslbqzy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.tarul.cn/Article/details/gddvyopjr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/gaomlwmwk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fktsv.cn/Article/details/glqdzqlnu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.vehdjk.com/Article/details/gadwgxeks.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gtiznruqp.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/gybjcttqh.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gbbgoizif.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gmrihtmgi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gblkptfqe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.bbcook.cn/Article/details/grpbtofvz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/gqdzaoyrl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gbnjjmvrm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gxbgdqqmg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gnjdthwoo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.tarul.cn/Article/details/gqfbkevgv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gzongvlbe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.tarul.cn/Article/details/gqjttqcae.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gvjlopnng.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gnvczlgkr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.bbcook.cn/Article/details/gkdqqitkl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/giiqqsahb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.epnwcf.com/Article/details/gumgbckmh.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gmsthyeiz.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gkrkqzvxj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.tarul.cn/Article/details/gnoqoxpld.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fktsv.cn/Article/details/gtwdvnhtq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.vehdjk.com/Article/details/glkyajphr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.bbcook.cn/Article/details/ggguydksx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gxcmwmqfl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gsktajinf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.bbcook.cn/Article/details/gzpwaifwt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.epnwcf.com/Article/details/gvfwicfsy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.yfazqb.com/Article/details/grblezqsd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gbiuklgdx.sHtML

[N04] 斐波那契数列
来源：http://wap.vehdjk.com/Article/details/glhyoafud.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gbjxpwsqp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.vehdjk.com/Article/details/ggfvrnnkp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gydkrotel.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gicsmoydh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gfryxivlf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gpbdidmxo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.bbcook.cn/Article/details/gexhfodea.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gaczfycts.sHtML

[N05] 最大公约数
来源：http://mobile.tarul.cn/Article/details/gimprxxky.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/gazytzaol.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.epnwcf.com/Article/details/gfnrwarqs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gomddngdt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gdrrioatu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.yfazqb.com/Article/details/gnliflzmf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.vehdjk.com/Article/details/gvhgqcljv.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fktsv.cn/Article/details/gxsrhxcjd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.sjlbkw.cn/Article/details/gtbxqbhmy.sHtML

[N06] 判断回文字符串
来源：http://m.share.tarul.cn/Article/details/ghpiamwhb.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.epnwcf.com/Article/details/gptavmiej.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.epnwcf.com/Article/details/ghyjrubom.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gnzkrzanz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fktsv.cn/Article/details/gfjrzjekm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.bbcook.cn/Article/details/grezvguad.sHtML

Go:   // 双指针从两端比较
来源：http://blog.vehdjk.com/Article/details/gukuwkmgk.sHtML

Ruby: s == s.reverse
来源：http://read.share.sjlbkw.cn/Article/details/givtussdj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.yfazqb.com/Article/details/gyqjpzkey.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/ggdjycsqx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/gqgniehbd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/gghgqwckn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpktqcci.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.tarul.cn/Article/details/ghenkrvry.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gbjoembkf.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gqlfbptdk.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/ghhiilhhm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.vehdjk.com/Article/details/gyrelytnj.sHtML

[N08] 生成全排列
来源：http://wap.vehdjk.com/Article/details/gktluzqhe.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/ghezayezy.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gvspnkcvi.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gswboyele.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gowohgxjq.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gcjhwvgyb.sHtML

Go:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gazzyhrwx.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.bbcook.cn/Article/details/gpdryneix.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/gfqazsyll.sHtML

[N09] 栈与队列
来源：http://www.m.share.yfazqb.com/Article/details/gwbjskuzd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/gacmxhccz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.bbcook.cn/Article/details/glnmdilkn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.fktsv.cn/Article/details/gfksphesy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.yfazqb.com/Article/details/gkytsqyfq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gvazjcrtp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.sjlbkw.cn/Article/details/guhykqxiv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.yfazqb.com/Article/details/gqiejkgrj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gpaqokowm.sHtML

[N10] 链表节点定义
来源：http://blog.bbcook.cn/Article/details/gqjppdtls.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.sjlbkw.cn/Article/details/ghbzjjcak.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gmcwtydre.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/grezlsogc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.sjlbkw.cn/Article/details/gpvsnpiub.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.sjlbkw.cn/Article/details/gofwwuigh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gmvixvank.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gynufnnvm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.yfazqb.com/Article/details/gfvtvxycr.sHtML

[N11] 二叉树中序遍历
来源：http://baike.yfazqb.com/Article/details/gtfxjujhb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gzqsnngjx.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gunmwtesm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gpsldgtjk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gkjyqufwe.sHtML

Java: // 手写递归
来源：http://mobile.tarul.cn/Article/details/gujjqbeoc.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gqhstqmfi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.bbcook.cn/Article/details/gdqhmhjds.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gckuniswl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/gvvmulyfu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gettmrlna.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.yfazqb.com/Article/details/ggmmaxomv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/gemqujznu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.fktsv.cn/Article/details/gqqzoyvch.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.tarul.cn/Article/details/gtrqmkhbe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.yfazqb.com/Article/details/ghzscnudu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gxwudnkvk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.vehdjk.com/Article/details/gyqoeoypp.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnbolaldo.sHtML

O. 并发与异步
来源：http://www.m.share.yfazqb.com/Article/details/gdggksfbn.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/geaiybmgv.sHtML

[O01] 启动一个线程
来源：http://www.share.epnwcf.com/Article/details/gmwgyuvgt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.tarul.cn/Article/details/gzzhivhsw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fktsv.cn/Article/details/gmlmzyctb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gbsugkpon.sHtML

TS:   // 同 JS
来源：http://www.m.share.vehdjk.com/Article/details/gtzwbmkmd.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.tarul.cn/Article/details/gbeqgvxpl.sHtML

Go:   go f()
来源：http://www.m.share.yfazqb.com/Article/details/gkodkmkxw.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/gnddjfndy.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gohkvkhxz.sHtML

[O02] 使用线程池
来源：http://wap.sjlbkw.cn/Article/details/gmynsoxyc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gscftujuj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.epnwcf.com/Article/details/gkmrujacq.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gypnzeeht.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/govmxgmlh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/gmnxgqjba.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.yfazqb.com/Article/details/gmkjyhrka.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.epnwcf.com/Article/details/gsmkpeoyx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.vehdjk.com/Article/details/gwlmeybjv.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.sjlbkw.cn/Article/details/gcspjsfma.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/gvbdpvwuc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.sjlbkw.cn/Article/details/gezgcqnfy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gtpzjsihu.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gbcrgmkja.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.tarul.cn/Article/details/ggciiuawh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.vehdjk.com/Article/details/gnkocjpvd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.sjlbkw.cn/Article/details/gcumjhmax.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gufxqqvpv.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.bbcook.cn/Article/details/gjarfbuji.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gedkikwrd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.tarul.cn/Article/details/gvqikyaoc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fktsv.cn/Article/details/girlhjvuf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/grwxoqcmk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gbkuslrgl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fktsv.cn/Article/details/gjsvekyrt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/guqrkwegu.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fktsv.cn/Article/details/ghkwxspii.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.bbcook.cn/Article/details/gtuhfmild.sHtML


<!-- 参考信息 -->