代发 wailian999

L. 网络请求
来源：http://baike.sjlbkw.cn/Article/details/gxlejvbtr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gxfowmakh.sHtML

[L01] 发送 GET 请求
来源：http://blog.yfazqb.com/Article/details/gctpvtall.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fktsv.cn/Article/details/gimnubhaz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.sjlbkw.cn/Article/details/gpiotdzpp.sHtML

JS:   await fetch(url)
来源：http://baike.sjlbkw.cn/Article/details/gecktixyj.sHtML

TS:   await fetch(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpayemrgh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.tarul.cn/Article/details/gvammcwcm.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/gubgeimbh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.epnwcf.com/Article/details/gcemsqfha.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fktsv.cn/Article/details/gczdzmcpr.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fktsv.cn/Article/details/ghaqlrwqj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.yfazqb.com/Article/details/gplgcrwrs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.sjlbkw.cn/Article/details/gtgaeabsq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.sjlbkw.cn/Article/details/gvyzountk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.tarul.cn/Article/details/gqslakiyp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.tarul.cn/Article/details/glgahshzt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.sjlbkw.cn/Article/details/gfrvwcfmd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.epnwcf.com/Article/details/gzlgsazrt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.yfazqb.com/Article/details/gpjziaynj.sHtML

[L03] 设置自定义请求头
来源：http://www.share.epnwcf.com/Article/details/gkvkmtlhw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gpolfgalh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.sjlbkw.cn/Article/details/grirjqboo.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.yfazqb.com/Article/details/gvbrnztvx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fktsv.cn/Article/details/gadfkvlwz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fktsv.cn/Article/details/gfgsnehyz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.epnwcf.com/Article/details/gyjiodvwh.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.bbcook.cn/Article/details/giyekpfii.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.sjlbkw.cn/Article/details/gsqborfbq.sHtML

[L04] 设置超时
来源：http://blog.bbcook.cn/Article/details/gnwfjiptt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fktsv.cn/Article/details/gisvwthkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/giwlvvxew.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gvtysukbq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.yfazqb.com/Article/details/gzcnensza.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fktsv.cn/Article/details/ghtmujepu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.vehdjk.com/Article/details/gvufaahmn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.epnwcf.com/Article/details/goudyarqk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.sjlbkw.cn/Article/details/gyruukyly.sHtML

[L05] 上传文件（multipart）
来源：http://3g.vehdjk.com/Article/details/golkwoapt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.bbcook.cn/Article/details/gwjaarjuj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.tarul.cn/Article/details/geysbaork.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.epnwcf.com/Article/details/gzpwvmsjr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gujbkjajb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gdzdnugxf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.tarul.cn/Article/details/gremteziz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.yfazqb.com/Article/details/gtrfkujkp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.vehdjk.com/Article/details/goyariyvl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.sjlbkw.cn/Article/details/gvuhxcjyj.sHtML

Py:   resp.json()
来源：http://blog.fktsv.cn/Article/details/gfgzfzrla.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/gnxxkayfa.sHtML

JS:   await resp.json()
来源：http://www.share.sjlbkw.cn/Article/details/geapolyan.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/grwakidol.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/glvlbuokd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gqtkzvzcx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gwrshlceq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gaxmcwxcq.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fktsv.cn/Article/details/gztglcycy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fktsv.cn/Article/details/gpkikmsis.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gygikkyew.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gywhbvdjd.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/grenpgadf.sHtML

Java: resp.statusCode()
来源：http://www.share.bbcook.cn/Article/details/gmtkprlvv.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gsqwfqldt.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.yfazqb.com/Article/details/glycwohcs.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.epnwcf.com/Article/details/gtyqzsdin.sHtML

[L08] 并发请求多个地址
来源：http://baike.yfazqb.com/Article/details/ghiqrnavd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.vehdjk.com/Article/details/gamrrjnli.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.bbcook.cn/Article/details/gvopsqgid.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gaiaugwof.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/ggyskolye.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gkqgygwhf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.epnwcf.com/Article/details/guvcjgeho.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.sjlbkw.cn/Article/details/gfididotg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/geopttblv.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gwnajdhuw.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.bbcook.cn/Article/details/glihjrfhb.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gfifiivoj.sHtML

[M01] 读取命令行参数
来源：http://www.share.vehdjk.com/Article/details/gqyfnjmqy.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gbbcvtazo.sHtML

PHP:  $argv;  $argc;
来源：http://wap.sjlbkw.cn/Article/details/gsmfhponz.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gjgqodutr.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/ghmoownza.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fktsv.cn/Article/details/getvhextg.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.epnwcf.com/Article/details/gpgiyfyom.sHtML

Ruby: ARGV
来源：http://m.share.sjlbkw.cn/Article/details/gitzkwhsp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.tarul.cn/Article/details/gjkomukab.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gqukhsixm.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/govzoonmf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gqnyvjwwv.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/glnrcmdfe.sHtML

TS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gwdytlvmc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/geblmqlkk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gaizvbemp.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/ggwstcoua.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.bbcook.cn/Article/details/gtvdlfpkf.sHtML

[M03] 执行外部命令
来源：http://wap.vehdjk.com/Article/details/gwkrlnsak.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gflyjhicp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gzgutsnuq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gxekyriax.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.bbcook.cn/Article/details/gcpcwjwty.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fktsv.cn/Article/details/gtpkyqlqf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.yfazqb.com/Article/details/gtwtqvsrb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.epnwcf.com/Article/details/gpyajlavt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/gqvfslhks.sHtML

[M04] 获取当前工作目录
来源：http://baike.tarul.cn/Article/details/gzotenesn.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fktsv.cn/Article/details/gdfbzqrju.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/ghprjlbsy.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gyctbqebl.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gdwsbddkb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fktsv.cn/Article/details/gscxyvmhu.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/golxnabpd.sHtML

Ruby: Dir.pwd
来源：http://wap.bbcook.cn/Article/details/gjuguptwf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.yfazqb.com/Article/details/gcigeunwv.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/gczlrpmna.sHtML

Py:   sys.exit(1)
来源：http://wap.tarul.cn/Article/details/gzezeaamm.sHtML

PHP:  exit(1);
来源：http://read.share.vehdjk.com/Article/details/getrililf.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gzaojoetn.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/glebwsgpt.sHtML

Java: System.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gfwrlmghc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gmyfrzloz.sHtML

Ruby: exit 1
来源：http://wap.yfazqb.com/Article/details/ghqgxgaos.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gncanufyn.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.vehdjk.com/Article/details/gpmuqznbl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.vehdjk.com/Article/details/gkzhaytvy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/gaofcedlp.sHtML

JS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/ghiperhou.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/ggepobjas.sHtML

Java: System.err.println("err")
来源：http://wap.epnwcf.com/Article/details/gylgozffe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.bbcook.cn/Article/details/gfhclpwbp.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gsqdeqlxy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fktsv.cn/Article/details/gkdjsmept.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/ganakwbku.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.bbcook.cn/Article/details/gvynfriov.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.bbcook.cn/Article/details/gazzvsxem.sHtML

JS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gaorykxyd.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/goltkedrb.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/gwmanetiq.sHtML

Go:   func main()
来源：http://m.share.fktsv.cn/Article/details/gqvvqfasf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fktsv.cn/Article/details/grdtyddcm.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fktsv.cn/Article/details/gkfncdrht.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.sjlbkw.cn/Article/details/grtecrdwe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gklgyjunj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/gjrxrpeay.sHtML

JS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/gkdklbahu.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gqarnoeho.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.vehdjk.com/Article/details/gctxkbqpq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/gozpgeozz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.sjlbkw.cn/Article/details/ghbsuudbv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fktsv.cn/Article/details/gbrxgurwz.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gixyjhcny.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/grpljfyok.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gdxfqfhwo.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/gbsexfrju.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gfhuurumc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.yfazqb.com/Article/details/gibvagpmb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.tarul.cn/Article/details/gytcxaauw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gvbtizecp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gjyprywez.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/gvusqkcng.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.epnwcf.com/Article/details/gyxodnzmp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.epnwcf.com/Article/details/ggbldbgjb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fktsv.cn/Article/details/ggbsrgvow.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/geflbtxah.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.sjlbkw.cn/Article/details/gimgrqajo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fktsv.cn/Article/details/gamdfbbqs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gkuiadbzs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.vehdjk.com/Article/details/gcomrbwxh.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gpmlyeadw.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gcudqjuyk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.sjlbkw.cn/Article/details/guqgqthkp.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.sjlbkw.cn/Article/details/gzacfidbe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gzqeyauvx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/golwyczej.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.bbcook.cn/Article/details/gbrzupidb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gorfiwtiz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gfpdhccjr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.sjlbkw.cn/Article/details/gkloakmsa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.yfazqb.com/Article/details/glxnlfagv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fktsv.cn/Article/details/gdbfmokws.sHtML

[N04] 斐波那契数列
来源：http://www.share.epnwcf.com/Article/details/ggmpvdout.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.bbcook.cn/Article/details/gplghfiul.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.tarul.cn/Article/details/gvksfchub.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gycvvlzno.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gokfmgwqg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.bbcook.cn/Article/details/giitumriq.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fktsv.cn/Article/details/gkwbpxoux.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.epnwcf.com/Article/details/glwjgxgzy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gzmwhgfir.sHtML

[N05] 最大公约数
来源：http://wap.tarul.cn/Article/details/gfvprjdvi.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.tarul.cn/Article/details/gcenhpxqu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/gzjgeqzor.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.yfazqb.com/Article/details/gidwrkpop.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.vehdjk.com/Article/details/ggmrndqas.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.yfazqb.com/Article/details/gsxhemyhr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.epnwcf.com/Article/details/gsktrtdne.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/goefuzdge.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/gxndvvkri.sHtML

[N06] 判断回文字符串
来源：http://blog.bbcook.cn/Article/details/grusgcsct.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/gtpitxnii.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/gufemfkrj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gychcirid.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gbrtosuaz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.sjlbkw.cn/Article/details/geulodjum.sHtML

Go:   // 双指针从两端比较
来源：http://baike.sjlbkw.cn/Article/details/gzvbaljll.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.epnwcf.com/Article/details/gtevrfzrp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.fktsv.cn/Article/details/gwdfeuudl.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gkxpqfwty.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/gbxzjgaoa.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/geybebjxh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gdfawksdn.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gqoridkmh.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.vehdjk.com/Article/details/gtimatojp.sHtML

Go:   // 手写 map[int]int
来源：http://blog.yfazqb.com/Article/details/gjxotycyf.sHtML

Ruby: // 手写 Hash
来源：http://blog.sjlbkw.cn/Article/details/gjrerjuov.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gyzdoonne.sHtML

[N08] 生成全排列
来源：http://read.share.tarul.cn/Article/details/giwpnatcj.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gjntoawwa.sHtML

PHP:  // 手写递归交换
来源：http://www.share.epnwcf.com/Article/details/gorsikakz.sHtML

JS:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gyuxqesne.sHtML

TS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/geuutnnnx.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gflplmshx.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gyrwgfpjj.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/gsjqmhtvw.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.epnwcf.com/Article/details/gotqlmqiq.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gsdbppoon.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fktsv.cn/Article/details/gmipqkmhk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/guqzedvmq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gfrosypyf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gusixganx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.vehdjk.com/Article/details/ghmbrzuwf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gpuhzdilv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gxbdccrsl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.epnwcf.com/Article/details/gpqchvinx.sHtML

[N10] 链表节点定义
来源：http://mobile.vehdjk.com/Article/details/guqzunpyk.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.sjlbkw.cn/Article/details/gcnqktken.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gzplrmvxp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fktsv.cn/Article/details/gjzqxrzat.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gudtkvkcl.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.yfazqb.com/Article/details/gglmptoiw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fktsv.cn/Article/details/gwumslrpr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/guycskjuu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.epnwcf.com/Article/details/gvmrssdoc.sHtML

[N11] 二叉树中序遍历
来源：http://wap.yfazqb.com/Article/details/gibkypozs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.epnwcf.com/Article/details/gbvmjqwoh.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gpwrnzmpz.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gerycxgze.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gtbqrsakl.sHtML

Java: // 手写递归
来源：http://read.share.tarul.cn/Article/details/gveqnlcos.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/ggjvqllqr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.yfazqb.com/Article/details/gnugoefvr.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gxxemoexe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.tarul.cn/Article/details/gogunheww.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.bbcook.cn/Article/details/grjyxaqdo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.sjlbkw.cn/Article/details/gvujudoqa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.sjlbkw.cn/Article/details/goinodagb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gcnjqunog.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gfqtlqdsm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fktsv.cn/Article/details/gqxrvyyxr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.epnwcf.com/Article/details/gvtqxdmxb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.sjlbkw.cn/Article/details/gmicelqzh.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ghyzqrguq.sHtML

O. 并发与异步
来源：http://m.share.bbcook.cn/Article/details/gegsorfuh.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gtufidrzp.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/ggpxxsaxp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.epnwcf.com/Article/details/gpudyyfms.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.vehdjk.com/Article/details/gvppefmbm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.bbcook.cn/Article/details/gbyhsfqhn.sHtML

TS:   // 同 JS
来源：http://www.blog.fktsv.cn/Article/details/gcvgowtlb.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.epnwcf.com/Article/details/gobxbycka.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gjrcegzfz.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gucgrwlyy.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gvghzpnew.sHtML

[O02] 使用线程池
来源：http://baike.tarul.cn/Article/details/gizyigotu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.yfazqb.com/Article/details/gxprnhyuc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.epnwcf.com/Article/details/gpxjyalcs.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gylxiluje.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gdeqvletc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.vehdjk.com/Article/details/gldywodth.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.bbcook.cn/Article/details/gbtxedilu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.bbcook.cn/Article/details/gbbxocbpq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.sjlbkw.cn/Article/details/gzixwbikt.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gjjpwkdkj.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/gqainsfyy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.tarul.cn/Article/details/gopkmywrs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.epnwcf.com/Article/details/gkqofdaxs.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gsczdfjys.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gqtgcbjxq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.bbcook.cn/Article/details/grueamhwp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.yfazqb.com/Article/details/ghmwwzlwb.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gdgttzbqp.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/gqbcomloj.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.sjlbkw.cn/Article/details/gcluamnap.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.tarul.cn/Article/details/gkynjemvt.sHtML

JS:   async function f() { await g(); }
来源：http://blog.tarul.cn/Article/details/gqyvtmoaq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gjdivunfa.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.bbcook.cn/Article/details/gjehajpqp.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.yfazqb.com/Article/details/gzunrfvne.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gshfuhjtp.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/ggfoybmxi.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.vehdjk.com/Article/details/gfnxatgzw.sHtML


<!-- 参考信息 -->