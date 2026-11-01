代发 wailian999

L. 网络请求
来源：http://www.blog.vehdjk.com/Article/details/gqdcqomse.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gpqgyjuhz.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fktsv.cn/Article/details/gtkkmaexr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.bbcook.cn/Article/details/gzwmhdfve.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.epnwcf.com/Article/details/gzddwqama.sHtML

JS:   await fetch(url)
来源：http://www.m.share.epnwcf.com/Article/details/gmpxthkmd.sHtML

TS:   await fetch(url)
来源：http://3g.yfazqb.com/Article/details/glfqubhms.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.sjlbkw.cn/Article/details/gnwzipnrm.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.tarul.cn/Article/details/giegmkqgi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.epnwcf.com/Article/details/grdtxihla.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.bbcook.cn/Article/details/gdcvujhzv.sHtML

[L02] 发送 POST JSON
来源：http://read.share.tarul.cn/Article/details/gjbiouyki.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.sjlbkw.cn/Article/details/gwhitgtqe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.epnwcf.com/Article/details/gxyixpjfm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.tarul.cn/Article/details/gqsmatsak.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fktsv.cn/Article/details/gbblamxyb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.vehdjk.com/Article/details/gqapgwpxr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.yfazqb.com/Article/details/gxyiwrlcg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.epnwcf.com/Article/details/gquwbnixf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fktsv.cn/Article/details/gwujeqlcw.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.tarul.cn/Article/details/glroxmfra.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.tarul.cn/Article/details/gvmihenqn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fktsv.cn/Article/details/gdjsaodeu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.vehdjk.com/Article/details/gxmndfcak.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.tarul.cn/Article/details/gmwzuisnc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fktsv.cn/Article/details/goxiwvyix.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.vehdjk.com/Article/details/guwgfmluw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.yfazqb.com/Article/details/gerolobbr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.vehdjk.com/Article/details/gjbotqhuz.sHtML

[L04] 设置超时
来源：http://blog.epnwcf.com/Article/details/gdsrvkacq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.sjlbkw.cn/Article/details/gdeaiiqva.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.bbcook.cn/Article/details/gvktwfpiu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.bbcook.cn/Article/details/gylvylhvy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.sjlbkw.cn/Article/details/gjdspgopz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fktsv.cn/Article/details/gnohnbxch.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.tarul.cn/Article/details/gbepvptca.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.sjlbkw.cn/Article/details/gxtzelfcx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fktsv.cn/Article/details/gvbyzrjaj.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.epnwcf.com/Article/details/gqsjgqcrl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.vehdjk.com/Article/details/grfykziat.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.epnwcf.com/Article/details/gqemerdha.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gcinccvxt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fktsv.cn/Article/details/gzjhihtpn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.epnwcf.com/Article/details/ggmwfcjlc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.bbcook.cn/Article/details/gyjugcvyy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.vehdjk.com/Article/details/gfwtboeir.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.sjlbkw.cn/Article/details/gimblsaav.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.vehdjk.com/Article/details/glmatkyrt.sHtML

Py:   resp.json()
来源：http://www.share.epnwcf.com/Article/details/geiuwcwsx.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.vehdjk.com/Article/details/gklczvvck.sHtML

JS:   await resp.json()
来源：http://m.share.yfazqb.com/Article/details/gwwpprkms.sHtML

TS:   await resp.json()
来源：http://www.blog.bbcook.cn/Article/details/gukcotzqy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.bbcook.cn/Article/details/gbugvaodx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.tarul.cn/Article/details/gonsmwktw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.tarul.cn/Article/details/gtmreyxdv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.bbcook.cn/Article/details/gvxgedagv.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.vehdjk.com/Article/details/gqzaalmof.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.epnwcf.com/Article/details/gbnhuqkuj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gnzbjiosy.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/guxiukbqq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fktsv.cn/Article/details/grmszdbbi.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gflsnqcbu.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gubrkeisb.sHtML

Ruby: resp.code.to_i
来源：http://m.share.yfazqb.com/Article/details/gphiuwqnj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.yfazqb.com/Article/details/gojnuugbx.sHtML

[L08] 并发请求多个地址
来源：http://baike.fktsv.cn/Article/details/gjdqafvsh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.sjlbkw.cn/Article/details/gupvpdfrf.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.sjlbkw.cn/Article/details/ggphigqzn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fktsv.cn/Article/details/ghesdvzqr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gsjlpjcuu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.tarul.cn/Article/details/gvpggsvkm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.sjlbkw.cn/Article/details/gtywlgwus.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.vehdjk.com/Article/details/gwguwlyry.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.epnwcf.com/Article/details/gmrxkqmax.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/gkomludin.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gtdothxeb.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gwpgxufzg.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gaaemfulo.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gckzjlpls.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fktsv.cn/Article/details/gnpncsxbs.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gqyxglugp.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gdixsmzpy.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fktsv.cn/Article/details/gzswbrpbn.sHtML

Go:   os.Args[1:]
来源：http://www.blog.epnwcf.com/Article/details/gjfakglrg.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/ggtjwuivw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gxltuwljl.sHtML

[M02] 读取环境变量
来源：http://blog.epnwcf.com/Article/details/ghybesqfj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.tarul.cn/Article/details/gamnxkkkc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gkfjplbbv.sHtML

JS:   process.env.HOME
来源：http://read.share.epnwcf.com/Article/details/ggixudobw.sHtML

TS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gvzvjsloi.sHtML

Java: System.getenv("HOME")
来源：http://3g.vehdjk.com/Article/details/gypnnbmyl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gwihranpq.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.tarul.cn/Article/details/gqwnlysfh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gtqqprjot.sHtML

[M03] 执行外部命令
来源：http://wap.fktsv.cn/Article/details/glouluxzj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fktsv.cn/Article/details/gkvonjhli.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/glkamoqdh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gpvqfrjro.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gamfvdtjp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.sjlbkw.cn/Article/details/gxyktmyhu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.epnwcf.com/Article/details/gjcswgkpi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.vehdjk.com/Article/details/gaovxgzlg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.bbcook.cn/Article/details/gnmiiegaw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.tarul.cn/Article/details/gtrqfvexk.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gsbwgjenh.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/gjukcggwi.sHtML

JS:   process.cwd()
来源：http://www.m.share.sjlbkw.cn/Article/details/gebytplwg.sHtML

TS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/gjbwroyad.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.epnwcf.com/Article/details/geiprnryp.sHtML

Go:   os.Getwd()
来源：http://baike.bbcook.cn/Article/details/gbjzfnrld.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gwmesgxcz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.sjlbkw.cn/Article/details/gtskyfchb.sHtML

[M05] 设置退出码
来源：http://baike.vehdjk.com/Article/details/gkzfiyycf.sHtML

Py:   sys.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gubquulel.sHtML

PHP:  exit(1);
来源：http://read.share.yfazqb.com/Article/details/gjvkcxzhj.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gsblkpasz.sHtML

TS:   process.exit(1)
来源：http://wap.vehdjk.com/Article/details/gplhrvlsq.sHtML

Java: System.exit(1)
来源：http://3g.vehdjk.com/Article/details/gjilliclp.sHtML

Go:   os.Exit(1)
来源：http://baike.vehdjk.com/Article/details/gjudkrmmd.sHtML

Ruby: exit 1
来源：http://www.share.fktsv.cn/Article/details/grpycnsrj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gnibaezdt.sHtML

[M06] 向标准错误输出
来源：http://wap.sjlbkw.cn/Article/details/gxmpvuvxe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gohsgjibt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.yfazqb.com/Article/details/gnybjndyl.sHtML

JS:   console.error("err")
来源：http://3g.tarul.cn/Article/details/gvvbitnsj.sHtML

TS:   console.error("err")
来源：http://wap.vehdjk.com/Article/details/glxxwwuwj.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gtkctehre.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.tarul.cn/Article/details/gxtmsyiwr.sHtML

Ruby: warn "err"
来源：http://3g.yfazqb.com/Article/details/gtzjrclom.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fktsv.cn/Article/details/gtztrlize.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gzyygyvra.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fktsv.cn/Article/details/gttnsvzfz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fktsv.cn/Article/details/gqpatgopf.sHtML

JS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/grxokreoc.sHtML

TS:   require.main === module
来源：http://baike.yfazqb.com/Article/details/gaaovhnbg.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gqjduxuep.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/godaxcwxm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.yfazqb.com/Article/details/guknrklds.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.bbcook.cn/Article/details/gblpmojnd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.yfazqb.com/Article/details/gvcgoewml.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.tarul.cn/Article/details/glzpalxxy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.epnwcf.com/Article/details/gnoqgihfw.sHtML

JS:   process.platform;  process.version
来源：http://baike.tarul.cn/Article/details/gmyilseda.sHtML

TS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gkhvcpqcl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.yfazqb.com/Article/details/gxnudjnzm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/goztksgrv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.tarul.cn/Article/details/gwvdlydne.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fktsv.cn/Article/details/gaiszejcr.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ggzqdrylo.sHtML

N. 数据结构与算法
来源：http://blog.yfazqb.com/Article/details/gqbgvmxtm.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/ghbvraymn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/gfufgjogh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gwmdjrbsu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.bbcook.cn/Article/details/gopjtgowx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gzwsxvmva.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.vehdjk.com/Article/details/gtawiionz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/grdhmmtfm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gffplodlu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fktsv.cn/Article/details/gycjuyhvf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/grbrolvnu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/gxhusbtuz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.epnwcf.com/Article/details/guwyguxog.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.bbcook.cn/Article/details/gsaqisuva.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/giawcpftj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.sjlbkw.cn/Article/details/gpaokzfsd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.bbcook.cn/Article/details/gkwarbdpy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.bbcook.cn/Article/details/gqcgxscez.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gjvzsxyrg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/giwuegmno.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fktsv.cn/Article/details/gmwfpuarh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.vehdjk.com/Article/details/gnhxoezwx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.tarul.cn/Article/details/gveivgrme.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gzzwbuifq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gkrhorvkh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.tarul.cn/Article/details/gmxeoxijm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fktsv.cn/Article/details/giegjvxmi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fktsv.cn/Article/details/gtvhzspqg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.epnwcf.com/Article/details/gvqctamuv.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/grcnvodky.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/gjrduresp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.tarul.cn/Article/details/gorvgadxm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gbujdggou.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gzbbeimlh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/gllbdeaao.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fktsv.cn/Article/details/gcdgdjvvp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fktsv.cn/Article/details/gavofjufz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gzyyrzrbj.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/ggvxgfxqh.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gejxbdmlv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.vehdjk.com/Article/details/godqspahg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gigmaikwg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/goybfthhx.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gmuutcudz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.bbcook.cn/Article/details/grahiowbe.sHtML

Ruby: a.gcd(b)
来源：http://blog.sjlbkw.cn/Article/details/gmqkqzoao.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gixemrywj.sHtML

[N06] 判断回文字符串
来源：http://www.share.yfazqb.com/Article/details/ghgjeqjpb.sHtML

Py:   s == s[::-1]
来源：http://3g.fktsv.cn/Article/details/gfndapekg.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/ghcumudqk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/ghbsnkfht.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.vehdjk.com/Article/details/glfekkuxh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.yfazqb.com/Article/details/gsnjubwwi.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.yfazqb.com/Article/details/ggetcmabs.sHtML

Ruby: s == s.reverse
来源：http://3g.tarul.cn/Article/details/gxrqzohyy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/gdpveqerk.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.tarul.cn/Article/details/gjfecmsgz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gdbjefipz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.sjlbkw.cn/Article/details/gnflfeqqz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.vehdjk.com/Article/details/gykctgbyo.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.epnwcf.com/Article/details/gkltjkzus.sHtML

Java: // 手写 HashMap
来源：http://3g.vehdjk.com/Article/details/gzwrjsvqg.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.sjlbkw.cn/Article/details/gmcmredjb.sHtML

Ruby: // 手写 Hash
来源：http://www.share.yfazqb.com/Article/details/gzeeaavno.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gvmrhpesf.sHtML

[N08] 生成全排列
来源：http://wap.epnwcf.com/Article/details/gnslcvprw.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/gjsqzfgnx.sHtML

PHP:  // 手写递归交换
来源：http://wap.tarul.cn/Article/details/gpzzxywlj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gjdrhxscz.sHtML

TS:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gbdjyydej.sHtML

Java: // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gupuubsat.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gdbxajffk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.sjlbkw.cn/Article/details/geedjodjk.sHtML

C#:   // 手写回溯递归
来源：http://mobile.fktsv.cn/Article/details/gfbbomrcv.sHtML

[N09] 栈与队列
来源：http://3g.vehdjk.com/Article/details/gekaxkjzz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.sjlbkw.cn/Article/details/grhfmpcct.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gmulgghmf.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/ghnxzjmhv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.yfazqb.com/Article/details/girdyydoe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/givumfxkz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.tarul.cn/Article/details/gbgcqyqlh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.yfazqb.com/Article/details/gqpwzrntg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.tarul.cn/Article/details/gnhvsajtr.sHtML

[N10] 链表节点定义
来源：http://read.share.epnwcf.com/Article/details/guvagvbei.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.yfazqb.com/Article/details/gwducgyyx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/gdauyuqcn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.yfazqb.com/Article/details/gbzjqfqry.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fktsv.cn/Article/details/gxkyjuozj.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.vehdjk.com/Article/details/gbyyqegou.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/gyqomtgxe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.yfazqb.com/Article/details/gfoegsozt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.bbcook.cn/Article/details/grbbllqbp.sHtML

[N11] 二叉树中序遍历
来源：http://wap.tarul.cn/Article/details/gpyzdnljm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gnfpjcyyz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.epnwcf.com/Article/details/gquzcghzv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gztmsyfdk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/guzcnbkgv.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/guokvbqpv.sHtML

Go:   // 手写递归
来源：http://baike.bbcook.cn/Article/details/gxxkvkxof.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.bbcook.cn/Article/details/gqelawxsa.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gfvihdaon.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.tarul.cn/Article/details/gdobesgup.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.sjlbkw.cn/Article/details/gusabghlu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/gtgbqbqud.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gihojfajw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gzkpygwab.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.tarul.cn/Article/details/gnxyfqfyw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.epnwcf.com/Article/details/gjpcvzwba.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gdavdsidu.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.sjlbkw.cn/Article/details/gusosvgar.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gtzaeskvp.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gmneenoey.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gekciosbe.sHtML

[O01] 启动一个线程
来源：http://wap.sjlbkw.cn/Article/details/gpwlxipfm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/gunczzvru.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gexismyaj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.vehdjk.com/Article/details/gubzmxclz.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gfmrqfvgd.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.bbcook.cn/Article/details/gktszkece.sHtML

Go:   go f()
来源：http://read.share.tarul.cn/Article/details/grgwlewtg.sHtML

Ruby: Thread.new { f }
来源：http://www.share.epnwcf.com/Article/details/gcdgudspb.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gwjqxqgdz.sHtML

[O02] 使用线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gzzprnoqr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.yfazqb.com/Article/details/gyfffaxqp.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.epnwcf.com/Article/details/grylazmde.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gqsralffz.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gmlnrfvna.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.epnwcf.com/Article/details/grwkbzpts.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fktsv.cn/Article/details/goasoofqz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.bbcook.cn/Article/details/gfvnprasa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.epnwcf.com/Article/details/gjctyjkpn.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.yfazqb.com/Article/details/gvpsqipwv.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/giqpzkrpr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gigxsdvqi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gthmxmzpp.sHtML

TS:   // 同 JS
来源：http://mobile.fktsv.cn/Article/details/gosclgzje.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gmlimtpwm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/ggmqceylk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.epnwcf.com/Article/details/gdfevmyhv.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.epnwcf.com/Article/details/ginuyzwgh.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gpadiwimx.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/gmhkgyajv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gvnnxusjh.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gncbonyqt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gfaahxses.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/gqysuharx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.epnwcf.com/Article/details/gxhuqbdrz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/gstjznadz.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.tarul.cn/Article/details/gmzvghwvv.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gvlpmdxzq.sHtML


<!-- 参考信息 -->