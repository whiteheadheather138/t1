代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fktsv.cn/Article/details/gpkkipxkz.sHtML

JS:   await fetch(url)
来源：http://mobile.bbcook.cn/Article/details/gmlukfjtt.sHtML

TS:   await fetch(url)
来源：http://blog.fktsv.cn/Article/details/gnpexxjfs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.vehdjk.com/Article/details/gwqcpirpo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgjmtfih.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/gwjninyvh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.bbcook.cn/Article/details/gewwjtvjm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/gxrqsumpy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.yfazqb.com/Article/details/gqapldaxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.sjlbkw.cn/Article/details/glyvkhovr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.yfazqb.com/Article/details/gummbkzmi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fktsv.cn/Article/details/glohzxktf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.yfazqb.com/Article/details/gldqsnuoi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.vehdjk.com/Article/details/grbbeeogw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.yfazqb.com/Article/details/glaolsllx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.bbcook.cn/Article/details/gdrlenvql.sHtML

[L03] 设置自定义请求头
来源：http://blog.yfazqb.com/Article/details/gjquyxcmb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.bbcook.cn/Article/details/gowewecfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.yfazqb.com/Article/details/gqmvqmdlp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.bbcook.cn/Article/details/gzbfaxohj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.vehdjk.com/Article/details/gybgoslcc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.sjlbkw.cn/Article/details/gnfwouupg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.epnwcf.com/Article/details/gzdrayjbz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fktsv.cn/Article/details/gzxlbkmjy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.vehdjk.com/Article/details/gpxpcstsd.sHtML

[L04] 设置超时
来源：http://www.share.yfazqb.com/Article/details/gjfdxqddb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.tarul.cn/Article/details/gakxnbpsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fktsv.cn/Article/details/gqrjzrtab.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.vehdjk.com/Article/details/gzdrwekii.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.yfazqb.com/Article/details/gqqbqnxnm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.bbcook.cn/Article/details/gjiesehiy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.epnwcf.com/Article/details/gnmcycywk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/gsjqbjfti.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.vehdjk.com/Article/details/gzjmigcag.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gjeontnbk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.vehdjk.com/Article/details/grkczltbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.epnwcf.com/Article/details/gjqzgzpjl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.vehdjk.com/Article/details/gpurmbldo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.bbcook.cn/Article/details/gvfsuupgu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.tarul.cn/Article/details/gigiuvgsu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.tarul.cn/Article/details/gcifenwak.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.bbcook.cn/Article/details/gxjzbdkwm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.epnwcf.com/Article/details/gbhdgqzoa.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.sjlbkw.cn/Article/details/gluphbgmh.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/gwakhzipv.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gpgsxznbc.sHtML

JS:   await resp.json()
来源：http://3g.epnwcf.com/Article/details/gwmugiahg.sHtML

TS:   await resp.json()
来源：http://baike.yfazqb.com/Article/details/gwutkwyim.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.epnwcf.com/Article/details/gosuudech.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.epnwcf.com/Article/details/gmbvqccha.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.sjlbkw.cn/Article/details/gvrgtgtel.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/gfgotaaza.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.yfazqb.com/Article/details/gtbsndzvo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.sjlbkw.cn/Article/details/grfcckjzp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.sjlbkw.cn/Article/details/gmubqtnkh.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.epnwcf.com/Article/details/gzdnhepcv.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gkzjszrhy.sHtML

Java: resp.statusCode()
来源：http://www.blog.tarul.cn/Article/details/gevdqcrgt.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gjvtfzkgm.sHtML

Ruby: resp.code.to_i
来源：http://blog.fktsv.cn/Article/details/gmqungnms.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gcofhguuz.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvuuocme.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.epnwcf.com/Article/details/gwwowqrke.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fktsv.cn/Article/details/gehizsnkr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.vehdjk.com/Article/details/gyrkzigxv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.yfazqb.com/Article/details/gmylsiuik.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/gwvkmypbo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gshowzqnh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.yfazqb.com/Article/details/gmcipvisu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.tarul.cn/Article/details/gzqojqwsy.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gjaxtedtv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fktsv.cn/Article/details/ggevtovct.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/ganmqanvk.sHtML

[M01] 读取命令行参数
来源：http://3g.sjlbkw.cn/Article/details/gfnbxifnj.sHtML

Py:   sys.argv[1:]
来源：http://blog.yfazqb.com/Article/details/gvfxfnhgq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.epnwcf.com/Article/details/gsjyslqsb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.bbcook.cn/Article/details/gphyrobmo.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gifqumjvk.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gerxfjxwq.sHtML

Go:   os.Args[1:]
来源：http://wap.tarul.cn/Article/details/grknrevkx.sHtML

Ruby: ARGV
来源：http://read.share.bbcook.cn/Article/details/gifuaytxm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gzxinvpim.sHtML

[M02] 读取环境变量
来源：http://blog.bbcook.cn/Article/details/gnsexrzwy.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fktsv.cn/Article/details/gjvvyvmfa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/grtdwpkhx.sHtML

JS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gmflvwpku.sHtML

TS:   process.env.HOME
来源：http://www.blog.bbcook.cn/Article/details/gpkocrwoz.sHtML

Java: System.getenv("HOME")
来源：http://read.share.bbcook.cn/Article/details/ggxshubiw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/gaxzgfltt.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gmfbilyqh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/goxipavgg.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gtwruifno.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.vehdjk.com/Article/details/gaxmoqxnk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.epnwcf.com/Article/details/gwigshzsy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/gpbukigxo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/garvqavud.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.tarul.cn/Article/details/gjuoqkovz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gsogdctie.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.epnwcf.com/Article/details/grcoejukv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fktsv.cn/Article/details/gvgxizlbm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.sjlbkw.cn/Article/details/gmcuhiouh.sHtML

Py:   os.getcwd()
来源：http://www.share.fktsv.cn/Article/details/gmjiiaiis.sHtML

PHP:  getcwd();
来源：http://3g.epnwcf.com/Article/details/gzgzkwgyy.sHtML

JS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/glrieeper.sHtML

TS:   process.cwd()
来源：http://3g.sjlbkw.cn/Article/details/gaxcfcdfd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.bbcook.cn/Article/details/gedmmyehr.sHtML

Go:   os.Getwd()
来源：http://blog.tarul.cn/Article/details/gainasnqf.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gpnqohoxq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/gktdqpfrp.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gdcegnwex.sHtML

Py:   sys.exit(1)
来源：http://blog.fktsv.cn/Article/details/gekeyvdjy.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/gfaeqmshf.sHtML

JS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gzktfvajp.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gviwqnqcg.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/gvvgorzco.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gabwhwoej.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/grdmflqsh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gqxbfiade.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gtamuavzq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.epnwcf.com/Article/details/glvlnvpbw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gqwvitbjl.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gvptmodoj.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gxxviwhhk.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gjdopumue.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gwhkmyqnl.sHtML

Ruby: warn "err"
来源：http://m.share.sjlbkw.cn/Article/details/godpkuean.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/glkwmpxsj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gtvejnayg.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/ghuepbxeg.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gzjkfptzm.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gpczdgnbk.sHtML

TS:   require.main === module
来源：http://blog.bbcook.cn/Article/details/gzretdqgt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.bbcook.cn/Article/details/gkruauohx.sHtML

Go:   func main()
来源：http://3g.yfazqb.com/Article/details/gyfrxwtqj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.sjlbkw.cn/Article/details/gizrsvwio.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gnugqwdpd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.bbcook.cn/Article/details/gcjfyvqyj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gptwuxhit.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fktsv.cn/Article/details/gcqvjfpyy.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/ghcukvatm.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gzjojhjrf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/glxybszfs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.yfazqb.com/Article/details/ghvveymit.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.epnwcf.com/Article/details/gkgyzrakx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.tarul.cn/Article/details/ghfafeghi.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gakafmsod.sHtML

N. 数据结构与算法
来源：http://www.share.yfazqb.com/Article/details/gukhxxruj.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gtfrribtq.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gqvlyitcz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fktsv.cn/Article/details/ghmaxrtgl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.bbcook.cn/Article/details/gupbcnmrz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdncwcgpe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/ghfzialiw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/gbrpccuni.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gchpceomj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.tarul.cn/Article/details/gwtrugdyo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gfsfraoce.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.epnwcf.com/Article/details/gznrxavbo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.vehdjk.com/Article/details/govzkpxqh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gvcecebrr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/gfcodynbr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gkekdgyno.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.sjlbkw.cn/Article/details/gaffhjjfm.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.sjlbkw.cn/Article/details/genclglja.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gsommwbga.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/ggfdutzxw.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.vehdjk.com/Article/details/gikltkgux.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gbsjzagkw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.vehdjk.com/Article/details/grnhgupce.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/godlcmiha.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gdtdftvyr.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/gqposqtyj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gkqzpjiyt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.tarul.cn/Article/details/gbnmyrrpq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.epnwcf.com/Article/details/gwdkjixzb.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fktsv.cn/Article/details/gdfuytytx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gnszkevms.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gicyrtuzp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fktsv.cn/Article/details/gdjhrgcbh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gqqkytdmd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.bbcook.cn/Article/details/ggsnpfpsj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.yfazqb.com/Article/details/gtsmafseo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/ggpisnolh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/grromnwke.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/gkwgfwubk.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.sjlbkw.cn/Article/details/gzwpjwswg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fktsv.cn/Article/details/gxqxwcdxg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gltkpqruu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gagrkuixj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.yfazqb.com/Article/details/ggbecatru.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/gfgmkyfno.sHtML

Ruby: a.gcd(b)
来源：http://3g.epnwcf.com/Article/details/gyeyurksh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/glyhpvakw.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gswtrnuen.sHtML

Py:   s == s[::-1]
来源：http://read.share.fktsv.cn/Article/details/gcrmgphac.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gnfwthqnl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/gqrsebzjs.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.vehdjk.com/Article/details/gtraqegnd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gbhshjzah.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/glqufgdqu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.yfazqb.com/Article/details/gjblgzurd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.epnwcf.com/Article/details/gsaezuqax.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.sjlbkw.cn/Article/details/grzqbhtuz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gsnretgjd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.tarul.cn/Article/details/grufexeut.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/gfvjvgqlj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.tarul.cn/Article/details/ghsxqqhhv.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gvagojlbc.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gvxyxdnpw.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.sjlbkw.cn/Article/details/grdztbpsl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.vehdjk.com/Article/details/gkacidonp.sHtML

[N08] 生成全排列
来源：http://3g.epnwcf.com/Article/details/gntgqcusy.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gzemlucft.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gftvmegdb.sHtML

JS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/grrgaecla.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gnuedsvab.sHtML

Java: // 手写回溯递归
来源：http://m.share.epnwcf.com/Article/details/glxhrnyhh.sHtML

Go:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gwcrjuvrt.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.yfazqb.com/Article/details/gkehtqxlq.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gokdcbwmx.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gbmdccgqw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.yfazqb.com/Article/details/gwqdvcfun.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gywqfissc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gpdaddqzh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gsrxutluq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fktsv.cn/Article/details/gocnwwawb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/gwktmxtvt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gssfmwaba.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/gffxrfult.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gbnhfxwnv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fktsv.cn/Article/details/grqlqagrs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.sjlbkw.cn/Article/details/gzotgutcg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.bbcook.cn/Article/details/gdrmbtdah.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fktsv.cn/Article/details/ggjwirfnt.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.yfazqb.com/Article/details/givcbxxtz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fktsv.cn/Article/details/gqnczvdnj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/gtcjbvkzf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.vehdjk.com/Article/details/gsptvevun.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fktsv.cn/Article/details/giemazkkh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gkyjkbhzt.sHtML

PHP:  // 手写递归函数
来源：http://mobile.vehdjk.com/Article/details/gnnphwfnr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gtliozvck.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gvghsrnxu.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gutzefnut.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gywmkfgqa.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.tarul.cn/Article/details/gherpuuab.sHtML

C#:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gczvqlvsq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.sjlbkw.cn/Article/details/grxwimifn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fktsv.cn/Article/details/gnbszyxkv.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.sjlbkw.cn/Article/details/glkwbntus.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gedhlrjdi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.sjlbkw.cn/Article/details/gxealucwr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gmqjpkadp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.vehdjk.com/Article/details/gjiqpsfox.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.bbcook.cn/Article/details/gwijzzksu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gbzphjdak.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/grbwezjlh.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gyphsfdlf.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gcxxktjtj.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gtfqolqce.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.epnwcf.com/Article/details/geldzuzau.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.sjlbkw.cn/Article/details/ggxwzmzwp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/gkhuaiwtr.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gxvfoytqz.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/gxuhahzlo.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gsrctwntf.sHtML

Ruby: Thread.new { f }
来源：http://mobile.tarul.cn/Article/details/gotofnrda.sHtML

C#:   Task.Run(() => F());
来源：http://wap.bbcook.cn/Article/details/gawbidzei.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gnkjvaycd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gdputnoau.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.vehdjk.com/Article/details/gpcoaweza.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gndyklmyu.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/grnigfpeu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fktsv.cn/Article/details/gmspallcn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.tarul.cn/Article/details/gjlyrabap.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fktsv.cn/Article/details/gybnkxrzq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.yfazqb.com/Article/details/gmnyxwerj.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gamatlomk.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/gslenbijj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fktsv.cn/Article/details/gletgzayr.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.yfazqb.com/Article/details/gcargregy.sHtML

TS:   // 同 JS
来源：http://www.share.vehdjk.com/Article/details/gddhhnuad.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.vehdjk.com/Article/details/gxpzrjhdc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.epnwcf.com/Article/details/gnzxkgvds.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.yfazqb.com/Article/details/gsuzikown.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gmpvhrmpn.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gsjllogfl.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.bbcook.cn/Article/details/gpegmhtgl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.vehdjk.com/Article/details/gbwmwfuwi.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.vehdjk.com/Article/details/gztxptmck.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gyeenzvil.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.yfazqb.com/Article/details/grbsqjdqh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.yfazqb.com/Article/details/gaivzjuot.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.sjlbkw.cn/Article/details/gojeiaqoa.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gnfhewzel.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/gscohbkok.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.bbcook.cn/Article/details/gyneenqtl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/googivkvh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gqdrrduru.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/guizfsurh.sHtML


<!-- 参考信息 -->