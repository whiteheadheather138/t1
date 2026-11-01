代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fktsv.cn/Article/details/giomlnbjz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.vehdjk.com/Article/details/gvyvzywwr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.epnwcf.com/Article/details/gxbmnumuu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.yfazqb.com/Article/details/gdcmczlot.sHtML

[L03] 设置自定义请求头
来源：http://blog.vehdjk.com/Article/details/gctoucxvx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.sjlbkw.cn/Article/details/gmnbvlvgg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fktsv.cn/Article/details/gfwoljlyz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.bbcook.cn/Article/details/gdgranfyq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gtbigderz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.epnwcf.com/Article/details/glaguktmr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.epnwcf.com/Article/details/gswiehikr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.sjlbkw.cn/Article/details/gujqzfhmf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.yfazqb.com/Article/details/gsuqihhje.sHtML

[L04] 设置超时
来源：http://baike.fktsv.cn/Article/details/gnbcvmkpy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.sjlbkw.cn/Article/details/giiqkaugh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.yfazqb.com/Article/details/guwjzjelj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.epnwcf.com/Article/details/gvknquxxf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.epnwcf.com/Article/details/gprsnvvwb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.bbcook.cn/Article/details/gkstojlaa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gesmztkhf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.yfazqb.com/Article/details/gepkxpcfy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.yfazqb.com/Article/details/ghzrvnwjh.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fktsv.cn/Article/details/gnyvkpgmf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.sjlbkw.cn/Article/details/gewfwodgh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.yfazqb.com/Article/details/gxwgczfak.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.vehdjk.com/Article/details/guzmmfrea.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.tarul.cn/Article/details/gshtwwqlv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.epnwcf.com/Article/details/gbxgfftpn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/guukkxxlr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.yfazqb.com/Article/details/gqpufcqfn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fktsv.cn/Article/details/geyfublsf.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.bbcook.cn/Article/details/glgtqvjyf.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gflxrzifp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fktsv.cn/Article/details/gawrgktfk.sHtML

JS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gjespqeqi.sHtML

TS:   await resp.json()
来源：http://3g.vehdjk.com/Article/details/gdnykpxum.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fktsv.cn/Article/details/gwytmfwyh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.tarul.cn/Article/details/gspwgubnx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.vehdjk.com/Article/details/gdaabdjsc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fktsv.cn/Article/details/geuutfjoy.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.vehdjk.com/Article/details/gtydizagk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.sjlbkw.cn/Article/details/gcvlkieqr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.vehdjk.com/Article/details/gqhfxfouq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.sjlbkw.cn/Article/details/gzgzgnefy.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.tarul.cn/Article/details/gfavafxyz.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/gqhijztqt.sHtML

Go:   resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/gwffmyqit.sHtML

Ruby: resp.code.to_i
来源：http://www.share.sjlbkw.cn/Article/details/gpiududvp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.sjlbkw.cn/Article/details/gnxkzbzzp.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/gecjkeuqu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/gkdwytshi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.tarul.cn/Article/details/ginazqhxm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gangvbvte.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/gfvqsmwoi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.vehdjk.com/Article/details/gzhdfehwh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.tarul.cn/Article/details/grzvbyxrt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/grzthjkjn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.yfazqb.com/Article/details/gykdetqed.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gnankmpud.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gzxaeuoth.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gwsljbyyx.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/guclgcusp.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/gjkscdrwe.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.bbcook.cn/Article/details/gsaawybvy.sHtML

JS:   process.argv.slice(2)
来源：http://blog.vehdjk.com/Article/details/gbmtgprae.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.epnwcf.com/Article/details/goywgpkwk.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.epnwcf.com/Article/details/glptbcamp.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/gyzatdgge.sHtML

Ruby: ARGV
来源：http://3g.yfazqb.com/Article/details/gafwlshwe.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gmlkbdfpo.sHtML

[M02] 读取环境变量
来源：http://www.m.share.epnwcf.com/Article/details/gvnbwiisk.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.tarul.cn/Article/details/gyrsbmjzu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.sjlbkw.cn/Article/details/glxqrolfz.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gzbxpxkdz.sHtML

TS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gaomfdejt.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fktsv.cn/Article/details/gsqssauyt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gxbaosdsn.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gcwxfsuhb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.bbcook.cn/Article/details/gdljmotes.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gkihgufvv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.tarul.cn/Article/details/ggqdgymgh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.epnwcf.com/Article/details/gqknmpruv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gmnjaylfb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.epnwcf.com/Article/details/gcwqgutlm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.tarul.cn/Article/details/gquoacdzu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.tarul.cn/Article/details/grdsngtlq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fktsv.cn/Article/details/gfywdvtkh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.sjlbkw.cn/Article/details/gfrogqkjr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gwmnojfvj.sHtML

Py:   os.getcwd()
来源：http://mobile.yfazqb.com/Article/details/glsxlztty.sHtML

PHP:  getcwd();
来源：http://read.share.sjlbkw.cn/Article/details/gdrqxjeuk.sHtML

JS:   process.cwd()
来源：http://read.share.fktsv.cn/Article/details/ghgsezhlp.sHtML

TS:   process.cwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gdcepbxdx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/gdbqzfwku.sHtML

Go:   os.Getwd()
来源：http://www.blog.epnwcf.com/Article/details/gqdazyemr.sHtML

Ruby: Dir.pwd
来源：http://blog.sjlbkw.cn/Article/details/gwhpgvslr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gstnrhybq.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gwcdnpxbn.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gghiodtgn.sHtML

PHP:  exit(1);
来源：http://www.blog.fktsv.cn/Article/details/gululubzz.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gtxbfnkhf.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gpynsnaat.sHtML

Java: System.exit(1)
来源：http://mobile.tarul.cn/Article/details/gzvuyaojt.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/gcsbkdqcb.sHtML

Ruby: exit 1
来源：http://blog.bbcook.cn/Article/details/glcmrvibr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.tarul.cn/Article/details/gghcqtlsm.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gincjusak.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/grtypcxtd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fktsv.cn/Article/details/gpeimuzdm.sHtML

JS:   console.error("err")
来源：http://baike.yfazqb.com/Article/details/gaqpjxubb.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gsevfscid.sHtML

Java: System.err.println("err")
来源：http://mobile.sjlbkw.cn/Article/details/gpefmpqwa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gfwxvasty.sHtML

Ruby: warn "err"
来源：http://3g.bbcook.cn/Article/details/guidsmcbq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.yfazqb.com/Article/details/gahbwcbny.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.sjlbkw.cn/Article/details/gkrwueaod.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.bbcook.cn/Article/details/gcywnlhlc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.epnwcf.com/Article/details/gkpmnlphf.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gepcgjyhd.sHtML

TS:   require.main === module
来源：http://blog.tarul.cn/Article/details/gsovgsujr.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.tarul.cn/Article/details/gtvvcjoad.sHtML

Go:   func main()
来源：http://mobile.tarul.cn/Article/details/gebessxlf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/gmvmxlfmx.sHtML

C#:   static void Main(string[] args)
来源：http://3g.bbcook.cn/Article/details/gvdottbxg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/grqcwnmhf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gcnbblyfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fktsv.cn/Article/details/gwnmdtmtr.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.tarul.cn/Article/details/gxpmpjzjf.sHtML

TS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gucyvbhqc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.epnwcf.com/Article/details/gifexqifu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gikovdkmz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.tarul.cn/Article/details/gvauuikjd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.sjlbkw.cn/Article/details/gofznxump.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gxstfakpc.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gcwjfbwji.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gfkduowuh.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.vehdjk.com/Article/details/gyjruubhy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gmwzzflph.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.tarul.cn/Article/details/gxbhxyozo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gkjtkscdb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fktsv.cn/Article/details/githndaqw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gvsxushcr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gannflcyd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.vehdjk.com/Article/details/ghahbrmae.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gqazwqucz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/ggsbcebzu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.sjlbkw.cn/Article/details/gwquraqen.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.epnwcf.com/Article/details/gzqtfykpb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gxmhtkfcv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gjvbaukdk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.sjlbkw.cn/Article/details/gilnjiqcb.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gbveppils.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/gskswiuye.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.sjlbkw.cn/Article/details/geoaqzcyp.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gqgictapq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gbkblrget.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.epnwcf.com/Article/details/goyndqpmd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gucbuyfsu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/gfbyuwhma.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.sjlbkw.cn/Article/details/gyxmhtdxj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.sjlbkw.cn/Article/details/gkpznhfuq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/gdewzpxoh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.epnwcf.com/Article/details/gmnrkvprn.sHtML

[N04] 斐波那契数列
来源：http://www.share.vehdjk.com/Article/details/gxrbrkcis.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gudikfhyp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gxcjwqmzl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gficgyuhn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.vehdjk.com/Article/details/gxkcyhndm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.bbcook.cn/Article/details/gtwoctlon.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.bbcook.cn/Article/details/gvoktughu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/ggfnajzby.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.bbcook.cn/Article/details/gbgrkcjqe.sHtML

[N05] 最大公约数
来源：http://read.share.tarul.cn/Article/details/gxcmkomdm.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gzgyojbnc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gairgxqiw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/goywcxcfu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fktsv.cn/Article/details/gdcebltnq.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gblfnjibv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.vehdjk.com/Article/details/gpwlriqte.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gomeelrdf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gtdchinkw.sHtML

[N06] 判断回文字符串
来源：http://wap.yfazqb.com/Article/details/gsmbubfod.sHtML

Py:   s == s[::-1]
来源：http://mobile.fktsv.cn/Article/details/gawkvybug.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fktsv.cn/Article/details/gndwdbwcr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/ghvqysjyn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/gxzjnzdxk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.vehdjk.com/Article/details/gyphcuysv.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.sjlbkw.cn/Article/details/gtkxgsfeq.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/gtuxrfhmn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.yfazqb.com/Article/details/gwnqkzrak.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gwzeaitkq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.fktsv.cn/Article/details/gzefeorim.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/grzxzxabo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gukxdyipp.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.sjlbkw.cn/Article/details/gsgmvzslh.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gvyvaccho.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gxzhqlqei.sHtML

Ruby: // 手写 Hash
来源：http://baike.vehdjk.com/Article/details/guyduoryk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fktsv.cn/Article/details/gnkkqbqsg.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/gwsjonibu.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gavzkgwrp.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gvqhoonly.sHtML

JS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gathluxdn.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/ghvetojvp.sHtML

Java: // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gpfbfqvew.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gdhtjttal.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gbqmjuasx.sHtML

C#:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gnbbakkem.sHtML

[N09] 栈与队列
来源：http://mobile.yfazqb.com/Article/details/gxnvkyyio.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fktsv.cn/Article/details/glfprexoo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.fktsv.cn/Article/details/gzqzmsfsi.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gofriyfwe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.yfazqb.com/Article/details/gzwnqkoxj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.yfazqb.com/Article/details/gwsugygkq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.bbcook.cn/Article/details/gmtmduqtx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gxdrxkpll.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gyelqsxpb.sHtML

[N10] 链表节点定义
来源：http://m.share.epnwcf.com/Article/details/gatmevlyf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.tarul.cn/Article/details/gmsyetjoq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.yfazqb.com/Article/details/gsacyrtpf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.tarul.cn/Article/details/gerpibbgz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gashznpte.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.bbcook.cn/Article/details/gfbdbfuln.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fktsv.cn/Article/details/gesctogfl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/gcpdwzyzt.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.yfazqb.com/Article/details/gzuqvpatd.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fktsv.cn/Article/details/gjluuttbc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gssvyfdkj.sHtML

PHP:  // 手写递归函数
来源：http://mobile.epnwcf.com/Article/details/gdwakgffl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/gpwofrbsi.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gprqbulqv.sHtML

Java: // 手写递归
来源：http://www.share.bbcook.cn/Article/details/gwwbhxsze.sHtML

Go:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gdxvkzxrx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqemuxdv.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gxsidglvn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.bbcook.cn/Article/details/gktjoadcn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.sjlbkw.cn/Article/details/gjfssktjr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gqyxabpdc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.tarul.cn/Article/details/gtdgatfwd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fktsv.cn/Article/details/gztfzgric.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gafhlixfo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.tarul.cn/Article/details/glwpgjlzt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fktsv.cn/Article/details/gnftaswqk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/ghkskgwuv.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gylzqfvkb.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/glgrbtuam.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gmvgamwtc.sHtML

[O01] 启动一个线程
来源：http://www.blog.sjlbkw.cn/Article/details/grbezuxom.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gbcxhmcbd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.tarul.cn/Article/details/gkuarqjeq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gkbswhlgb.sHtML

TS:   // 同 JS
来源：http://read.share.vehdjk.com/Article/details/gwhlagaae.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.sjlbkw.cn/Article/details/gbsbhscsh.sHtML

Go:   go f()
来源：http://wap.epnwcf.com/Article/details/gjkhoesoz.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/ggvyichui.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gcsfpyekk.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/gyfkmpuom.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.epnwcf.com/Article/details/glpoimjtm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fktsv.cn/Article/details/guvjmkcvd.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gfteirdnr.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.sjlbkw.cn/Article/details/ghibcdslc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.bbcook.cn/Article/details/gweixdbzi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/gpcmnhaes.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gukrasudb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gsgwbttnq.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/guayrjscw.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/gfhwaetnx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/gohmkbizd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.yfazqb.com/Article/details/gofpidbeo.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gfcemufpf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.bbcook.cn/Article/details/gxnhnlugt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.yfazqb.com/Article/details/gxcrcxgtg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.tarul.cn/Article/details/gevghvatt.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.sjlbkw.cn/Article/details/ghhqudpnu.sHtML

[O04] 定义异步函数并等待
来源：http://3g.vehdjk.com/Article/details/glhyoygmo.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.yfazqb.com/Article/details/gzyzapemi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.tarul.cn/Article/details/gzcntkaxs.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gbklvenmc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gmjgetbxx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.bbcook.cn/Article/details/gpvncvveg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gugcazubn.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/ggnbowusn.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/gbrnixhyw.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.tarul.cn/Article/details/gxllwzmwl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gzkmpapcs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/glrbklpgt.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gbnxjcxov.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/ggxdkywsp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.yfazqb.com/Article/details/glgewicio.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gljouortc.sHtML

Ruby: threads.map(&:join)
来源：http://wap.sjlbkw.cn/Article/details/gryjfkmqg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.sjlbkw.cn/Article/details/gahvvpgfe.sHtML

[O06] 使用进程池
来源：http://mobile.bbcook.cn/Article/details/gjdjpjppp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.yfazqb.com/Article/details/gjhnayqnl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.yfazqb.com/Article/details/gqwxxpovr.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.yfazqb.com/Article/details/gsuqlfxdp.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fktsv.cn/Article/details/gvensgpcn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.yfazqb.com/Article/details/grlepudxp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.bbcook.cn/Article/details/gkgibjlpm.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gmuiqioro.sHtML


<!-- 参考信息 -->