代发 wailian999

L. 网络请求
来源：http://www.share.bbcook.cn/Article/details/grvwcfbte.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gixxqfdka.sHtML

[L01] 发送 GET 请求
来源：http://3g.epnwcf.com/Article/details/gqiepvmfl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.vehdjk.com/Article/details/gdykmjank.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.yfazqb.com/Article/details/gmxuhvnuz.sHtML

JS:   await fetch(url)
来源：http://3g.tarul.cn/Article/details/gfwjfjviv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fktsv.cn/Article/details/gtcthfahp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.epnwcf.com/Article/details/gtbazpurq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.bbcook.cn/Article/details/gaafbrzwb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fktsv.cn/Article/details/grxwigcvm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.epnwcf.com/Article/details/givgdcxnw.sHtML

[L02] 发送 POST JSON
来源：http://m.share.bbcook.cn/Article/details/geejgtgzw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.tarul.cn/Article/details/gzkgxbiam.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.sjlbkw.cn/Article/details/guvrfczav.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.tarul.cn/Article/details/gznnnciov.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.sjlbkw.cn/Article/details/gkppuupge.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.bbcook.cn/Article/details/giswbpjyr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.tarul.cn/Article/details/gaoyvoizf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.yfazqb.com/Article/details/gvrplweon.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gmcmmldqb.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fktsv.cn/Article/details/gylymyjxk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.tarul.cn/Article/details/gpimlzmet.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.sjlbkw.cn/Article/details/giwexhwng.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fktsv.cn/Article/details/gahjccqox.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.vehdjk.com/Article/details/gicwsxlhu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.epnwcf.com/Article/details/gozmleyqz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gdwyezwgs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.epnwcf.com/Article/details/gwmxgqxte.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.tarul.cn/Article/details/gnxvwgicq.sHtML

[L04] 设置超时
来源：http://www.m.share.yfazqb.com/Article/details/guooyfkax.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.bbcook.cn/Article/details/gzpzfqczh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.sjlbkw.cn/Article/details/giyrivphp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.sjlbkw.cn/Article/details/glzbzbsfe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gitawmmyu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.yfazqb.com/Article/details/grcgutlvj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.yfazqb.com/Article/details/gxzfezoou.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fktsv.cn/Article/details/gqzbmrkia.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.vehdjk.com/Article/details/guefjmyvs.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.epnwcf.com/Article/details/gbnsarocz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.epnwcf.com/Article/details/gdrrhwhtn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.sjlbkw.cn/Article/details/glqxkfbyu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.vehdjk.com/Article/details/gkzochgai.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gxqaccyja.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fktsv.cn/Article/details/gfbrqytcr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fktsv.cn/Article/details/gnykxnxel.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fktsv.cn/Article/details/gvyratcge.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/gyqymtilh.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.tarul.cn/Article/details/gbfyuhlnc.sHtML

Py:   resp.json()
来源：http://www.share.tarul.cn/Article/details/goyuhzrgx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gvuxjsdlm.sHtML

JS:   await resp.json()
来源：http://baike.tarul.cn/Article/details/gpcuqxgub.sHtML

TS:   await resp.json()
来源：http://www.blog.epnwcf.com/Article/details/gsphgqqzw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.sjlbkw.cn/Article/details/grtpmultt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.tarul.cn/Article/details/gddrgtwzw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.epnwcf.com/Article/details/gulwvrxzq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gzoqlvcne.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.tarul.cn/Article/details/giefqhqfm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fktsv.cn/Article/details/gmpvhamlk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.tarul.cn/Article/details/gxhrbjusk.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.vehdjk.com/Article/details/glhszrjax.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gzpzzuhaw.sHtML

Java: resp.statusCode()
来源：http://mobile.tarul.cn/Article/details/gjtkvlahr.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gphfxewtk.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gptoitwsu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/gtaeqvcry.sHtML

[L08] 并发请求多个地址
来源：http://wap.tarul.cn/Article/details/gwqxrllji.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/ghvnrfchd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.vehdjk.com/Article/details/gjdakzouo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gdvqiudfs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.bbcook.cn/Article/details/gfqubwkyy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.tarul.cn/Article/details/ggqcsvpmm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/gmostcjyw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gtefyccne.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.epnwcf.com/Article/details/gmjutvnfz.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gcxrkwhvw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.vehdjk.com/Article/details/gnrknefyt.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/ghwqeudtl.sHtML

[M01] 读取命令行参数
来源：http://3g.vehdjk.com/Article/details/ghqqyonuv.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/gqfrrvxrp.sHtML

PHP:  $argv;  $argc;
来源：http://blog.epnwcf.com/Article/details/gxgdphaee.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fktsv.cn/Article/details/gbdgjdecc.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gfasmhcaa.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/glmdsqbop.sHtML

Go:   os.Args[1:]
来源：http://m.share.vehdjk.com/Article/details/gcvhgkonk.sHtML

Ruby: ARGV
来源：http://www.m.share.sjlbkw.cn/Article/details/gbnzdnbir.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.bbcook.cn/Article/details/gjypopsul.sHtML

[M02] 读取环境变量
来源：http://mobile.tarul.cn/Article/details/gyttcuoly.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.yfazqb.com/Article/details/ggyfreqso.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.tarul.cn/Article/details/gplrcsepf.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/ginibygtb.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/guwyjfhsd.sHtML

Java: System.getenv("HOME")
来源：http://www.share.epnwcf.com/Article/details/gpmtgyhnd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gfejwbkkg.sHtML

Ruby: ENV["HOME"]
来源：http://3g.vehdjk.com/Article/details/gyatsppgd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.tarul.cn/Article/details/gotfmiiid.sHtML

[M03] 执行外部命令
来源：http://blog.fktsv.cn/Article/details/giuljifiv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gbwfhijts.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gcxhvlyrp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/gjtycjvto.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.yfazqb.com/Article/details/gdnvxyauk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.epnwcf.com/Article/details/gabuvhdde.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.bbcook.cn/Article/details/gsxhuorno.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fktsv.cn/Article/details/gmmepgmqp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.tarul.cn/Article/details/givqldxqx.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fktsv.cn/Article/details/goguleawj.sHtML

Py:   os.getcwd()
来源：http://wap.bbcook.cn/Article/details/guyprstia.sHtML

PHP:  getcwd();
来源：http://read.share.bbcook.cn/Article/details/gjxoccnar.sHtML

JS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gavnqoxpx.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gwbwwgpfv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gueywgaqw.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/gsrjlotum.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gpuylbbxq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.epnwcf.com/Article/details/gmtymolld.sHtML

[M05] 设置退出码
来源：http://read.share.epnwcf.com/Article/details/gffycsrzy.sHtML

Py:   sys.exit(1)
来源：http://3g.epnwcf.com/Article/details/gorwkdjll.sHtML

PHP:  exit(1);
来源：http://wap.sjlbkw.cn/Article/details/gqaywcuxq.sHtML

JS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gprzitxzb.sHtML

TS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gtxeysqyf.sHtML

Java: System.exit(1)
来源：http://www.share.vehdjk.com/Article/details/gbksyzmzi.sHtML

Go:   os.Exit(1)
来源：http://m.share.yfazqb.com/Article/details/gwxuyinhv.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/ghhvwomxk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fktsv.cn/Article/details/gppumtvxa.sHtML

[M06] 向标准错误输出
来源：http://m.share.yfazqb.com/Article/details/gjyykacxa.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.yfazqb.com/Article/details/gfvxwzgzd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.yfazqb.com/Article/details/gwalcymgz.sHtML

JS:   console.error("err")
来源：http://www.blog.epnwcf.com/Article/details/gpgsuqijg.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gbvejjiuh.sHtML

Java: System.err.println("err")
来源：http://mobile.vehdjk.com/Article/details/gemradezg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.tarul.cn/Article/details/girufvivq.sHtML

Ruby: warn "err"
来源：http://wap.fktsv.cn/Article/details/gpekvmrfn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fktsv.cn/Article/details/guhyacldq.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/gbjqkslmh.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gawiyhhre.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.sjlbkw.cn/Article/details/gcxigfbfd.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gatmbewwv.sHtML

TS:   require.main === module
来源：http://wap.tarul.cn/Article/details/gclbodvri.sHtML

Java: public static void main(String[] args)
来源：http://blog.bbcook.cn/Article/details/gcyctgyiq.sHtML

Go:   func main()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwkfkbfez.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/golqotbmn.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gnwcthpqe.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.vehdjk.com/Article/details/ggwgiojek.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.vehdjk.com/Article/details/glbykaffi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/grjnjjksu.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gzxnhbaje.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/ghaferhiv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gsvqbhtlo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.yfazqb.com/Article/details/gjhxdmxua.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.vehdjk.com/Article/details/gfybrpsve.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gnnyltqou.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gdliluwtp.sHtML

N. 数据结构与算法
来源：http://www.m.share.sjlbkw.cn/Article/details/gdrbugtki.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gmbtidszk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gzpvdmqex.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.vehdjk.com/Article/details/gkjhdbpmz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fktsv.cn/Article/details/gmsirqakb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gctrzkzxy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gltunyvtc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.tarul.cn/Article/details/gyapnivvz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gafrhuesn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.sjlbkw.cn/Article/details/gswsvvpbv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.epnwcf.com/Article/details/gaipojdav.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/gsxfkhgeb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gsogczygs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gfhrotpgi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.vehdjk.com/Article/details/gzaantekd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gsfecjqik.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.sjlbkw.cn/Article/details/gewogulbv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gnredqylh.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gridcdkdv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.sjlbkw.cn/Article/details/ghhboslfd.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.sjlbkw.cn/Article/details/gbewwefbm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.epnwcf.com/Article/details/gblbkrneo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.yfazqb.com/Article/details/gdtklgqtz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/grebrohul.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gbxirzwxx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.sjlbkw.cn/Article/details/gerbdiqil.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.yfazqb.com/Article/details/gsgpdcssx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.bbcook.cn/Article/details/gebfktxiu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gvlmpnrbe.sHtML

[N04] 斐波那契数列
来源：http://m.share.epnwcf.com/Article/details/gniawktrk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gzqwiqsxh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.bbcook.cn/Article/details/grfjcqfmx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.vehdjk.com/Article/details/gdkrkisri.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gzmkcrhwv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.bbcook.cn/Article/details/gcmftnzqt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.sjlbkw.cn/Article/details/gtroqdrms.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gpqkisuxk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/gakrtqbmi.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gaolgvlnx.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.yfazqb.com/Article/details/grrfviccv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.vehdjk.com/Article/details/gzkskeego.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gdwbnuvdl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gukdtycuu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gpbvgtdys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/gaxsizryj.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/gxoglnkmo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.epnwcf.com/Article/details/gmnruklhy.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fktsv.cn/Article/details/gnoarylon.sHtML

Py:   s == s[::-1]
来源：http://www.blog.sjlbkw.cn/Article/details/ghcnxlqrj.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/glqmhtews.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.vehdjk.com/Article/details/gcfszgsvq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gezshoigb.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fktsv.cn/Article/details/gjvjjyvha.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.tarul.cn/Article/details/gjuvaxezm.sHtML

Ruby: s == s.reverse
来源：http://wap.tarul.cn/Article/details/ggiccqbmt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fktsv.cn/Article/details/goiuwynir.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.tarul.cn/Article/details/gghglpiwv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.sjlbkw.cn/Article/details/gbbbgjzid.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/ggwiaoivf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.vehdjk.com/Article/details/ghlpyiora.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fktsv.cn/Article/details/gamlyotsw.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/gwbnqlgtd.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gozwxsqxl.sHtML

Ruby: // 手写 Hash
来源：http://m.share.bbcook.cn/Article/details/gycwkdjrs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gnlezemhw.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gquhtpcjn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/gvaoizyrj.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.tarul.cn/Article/details/gdlalgjjw.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gcnojzekb.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gwustjbdq.sHtML

Java: // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gpxcyfizc.sHtML

Go:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gqtedurvc.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.sjlbkw.cn/Article/details/gvblhudvn.sHtML

C#:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gyxwjhgvm.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/glytiumsv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gvrwpdqme.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.yfazqb.com/Article/details/ghvkqnchn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gbitotubz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/gezzhnpbe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gyowsvlto.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/guywpmitk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/ghnxmlfqk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.yfazqb.com/Article/details/gxhlgpvdp.sHtML

[N10] 链表节点定义
来源：http://read.share.sjlbkw.cn/Article/details/goqrkpemc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.vehdjk.com/Article/details/gqsyywwwp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fktsv.cn/Article/details/gqkbpjgtv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/guhnmjaco.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fktsv.cn/Article/details/gcctaiddn.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/ggetkyrbs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fktsv.cn/Article/details/gvawquspc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gxiwcrltr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gerjumwth.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.epnwcf.com/Article/details/gldzbshwy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.tarul.cn/Article/details/geuzqggld.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gsihlsbkb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gqkupqgxb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.vehdjk.com/Article/details/gglugstjx.sHtML

Java: // 手写递归
来源：http://www.share.fktsv.cn/Article/details/ghfcjkqje.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gixczazch.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.vehdjk.com/Article/details/gypjhadnc.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/gqvmeypbl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gruwqrpkg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.bbcook.cn/Article/details/gcnlsqhab.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/gchnpches.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.tarul.cn/Article/details/gjafvpryj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/ggzkbcxop.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fktsv.cn/Article/details/glpvihvbw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/grhnewzcs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.yfazqb.com/Article/details/gyaujrfes.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.tarul.cn/Article/details/gsdtjpial.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gopvryupx.sHtML

O. 并发与异步
来源：http://baike.tarul.cn/Article/details/gtxgltyui.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gcislcoti.sHtML

[O01] 启动一个线程
来源：http://blog.epnwcf.com/Article/details/gcyqcgdpd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.epnwcf.com/Article/details/gvnpbuany.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gglekpekx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fktsv.cn/Article/details/gqqbmcshr.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gfgjbglqt.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fktsv.cn/Article/details/gruaqztko.sHtML

Go:   go f()
来源：http://www.m.share.tarul.cn/Article/details/gyarrhtor.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/ganudwuik.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.vehdjk.com/Article/details/gpiddspue.sHtML

[O02] 使用线程池
来源：http://read.share.fktsv.cn/Article/details/gqhdlkjwr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.fktsv.cn/Article/details/gqthcwspb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.tarul.cn/Article/details/gsdxesmrv.sHtML

JS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/ggophdjmb.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.fktsv.cn/Article/details/gmyewxcrr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fktsv.cn/Article/details/ghdsklgxr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.tarul.cn/Article/details/grxrlbybv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.sjlbkw.cn/Article/details/gispeajcp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.sjlbkw.cn/Article/details/gqzqmlefe.sHtML

[O03] 加锁保护共享数据
来源：http://3g.yfazqb.com/Article/details/gkxevnhfq.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gjgctquek.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.sjlbkw.cn/Article/details/gdzowlfvf.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gzoueouqv.sHtML

TS:   // 同 JS
来源：http://www.m.share.fktsv.cn/Article/details/gmsenxqlw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gytpvwpor.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/gtpmjrady.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gjuzxvqjz.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.bbcook.cn/Article/details/gvkibiyrv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gqhdvjphg.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.epnwcf.com/Article/details/gaivclwlq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.vehdjk.com/Article/details/gharvykvs.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/grvbwahib.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.bbcook.cn/Article/details/glfcxgnrz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/gjqzntnjd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.tarul.cn/Article/details/gmnvxvshd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.epnwcf.com/Article/details/geisynrgg.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.tarul.cn/Article/details/gpemmybew.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.sjlbkw.cn/Article/details/gvzkrjvwt.sHtML


<!-- 参考信息 -->