代发 wailian999

[L03] 设置自定义请求头
来源：http://www.share.vehdjk.com/Article/details/gttdombbg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.bbcook.cn/Article/details/gckyxhnjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.tarul.cn/Article/details/gpxnaltsw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.epnwcf.com/Article/details/gfvtvilyi.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.vehdjk.com/Article/details/ggrvvlczy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.yfazqb.com/Article/details/gwvfpltya.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fktsv.cn/Article/details/gmikvvzfr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.vehdjk.com/Article/details/grdqjvjpe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fktsv.cn/Article/details/glevlyjlp.sHtML

[L04] 设置超时
来源：http://read.share.yfazqb.com/Article/details/gnqccbhlh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.vehdjk.com/Article/details/gpjfbdfda.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.sjlbkw.cn/Article/details/gpzmxtaqv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.tarul.cn/Article/details/gyrdojgts.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gmxgasacb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.tarul.cn/Article/details/gfpuyumuf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.yfazqb.com/Article/details/gngoocqgi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.yfazqb.com/Article/details/gyrljbmro.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.bbcook.cn/Article/details/gnmhqeqnf.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.vehdjk.com/Article/details/gbjfkjsbs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.sjlbkw.cn/Article/details/gkieqgodd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.sjlbkw.cn/Article/details/ggdymypuo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fktsv.cn/Article/details/gechfnpqf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/gitiayhre.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.sjlbkw.cn/Article/details/gefqsssio.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fktsv.cn/Article/details/ghowctvsb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.vehdjk.com/Article/details/govzzjdgu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/gwipktqro.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.epnwcf.com/Article/details/gwbaoezwq.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/gindidyxd.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.yfazqb.com/Article/details/gcqsbplix.sHtML

JS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gyixnjsqp.sHtML

TS:   await resp.json()
来源：http://www.m.share.yfazqb.com/Article/details/gtnkmabwg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.sjlbkw.cn/Article/details/gcjwryunp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.yfazqb.com/Article/details/gjzdinmas.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fktsv.cn/Article/details/gwihmzopz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.epnwcf.com/Article/details/ggtahdgat.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.tarul.cn/Article/details/gvqfghenn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.vehdjk.com/Article/details/gfahxnqzv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.sjlbkw.cn/Article/details/gbagtbkpu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.yfazqb.com/Article/details/giktwwoyl.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.bbcook.cn/Article/details/gdmkkqque.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/gdtposppe.sHtML

Go:   resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gqebupsuv.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.epnwcf.com/Article/details/gvzawxsbr.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gvjhzehgq.sHtML

[L08] 并发请求多个地址
来源：http://blog.bbcook.cn/Article/details/gebbgzizd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.yfazqb.com/Article/details/gdgrutokp.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.vehdjk.com/Article/details/gmaceaxnr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gglveubjn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.tarul.cn/Article/details/gbwraljjc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.vehdjk.com/Article/details/gltocjmdz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.epnwcf.com/Article/details/gfmxyygcq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.epnwcf.com/Article/details/gfyvlmvpy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.tarul.cn/Article/details/gdzjjkiyb.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gembhhrue.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gyklwferd.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/grjjkrnny.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gelmfgllq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.sjlbkw.cn/Article/details/gcyobudam.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.yfazqb.com/Article/details/gygfxqkle.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/glwrjverm.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gtcgopxli.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gzmymfmxb.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gnvjpdfsh.sHtML

Ruby: ARGV
来源：http://www.m.share.fktsv.cn/Article/details/gglwgosuj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gurdphjmc.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/gibonzjci.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.vehdjk.com/Article/details/gcstrpcip.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.yfazqb.com/Article/details/gliacipgt.sHtML

JS:   process.env.HOME
来源：http://blog.yfazqb.com/Article/details/gqtnhdphf.sHtML

TS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/gfmtncvud.sHtML

Java: System.getenv("HOME")
来源：http://mobile.vehdjk.com/Article/details/gchnshygp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.bbcook.cn/Article/details/glztyynrn.sHtML

Ruby: ENV["HOME"]
来源：http://3g.tarul.cn/Article/details/gxdzupdvp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.tarul.cn/Article/details/gdhsrmqov.sHtML

[M03] 执行外部命令
来源：http://mobile.yfazqb.com/Article/details/gwrunreeg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.vehdjk.com/Article/details/gbzvdtuft.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.vehdjk.com/Article/details/gnxvovgas.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gvewkfslk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gqferocaf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.epnwcf.com/Article/details/gywunfrgk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gylfrcmek.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/gploldgng.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/gohofjbaz.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/ghbepveof.sHtML

Py:   os.getcwd()
来源：http://blog.bbcook.cn/Article/details/gfnhvozvp.sHtML

PHP:  getcwd();
来源：http://www.m.share.yfazqb.com/Article/details/gfqkcunme.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gopxvbehy.sHtML

TS:   process.cwd()
来源：http://mobile.fktsv.cn/Article/details/gkhphuwco.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gdofduqaw.sHtML

Go:   os.Getwd()
来源：http://3g.tarul.cn/Article/details/giyudbcdn.sHtML

Ruby: Dir.pwd
来源：http://m.share.epnwcf.com/Article/details/gcmoccoov.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.tarul.cn/Article/details/gencwfvbs.sHtML

[M05] 设置退出码
来源：http://www.m.share.vehdjk.com/Article/details/gidkvnrqt.sHtML

Py:   sys.exit(1)
来源：http://baike.yfazqb.com/Article/details/gyrafidcj.sHtML

PHP:  exit(1);
来源：http://www.share.bbcook.cn/Article/details/gpeexxayj.sHtML

JS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gkrijsnqr.sHtML

TS:   process.exit(1)
来源：http://baike.tarul.cn/Article/details/gtdlbeiuw.sHtML

Java: System.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/glldkefyz.sHtML

Go:   os.Exit(1)
来源：http://read.share.vehdjk.com/Article/details/gakcnifbz.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gdlukgnkr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.epnwcf.com/Article/details/ggsmdrugi.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gcelcoefz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.sjlbkw.cn/Article/details/gncggqrxz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.sjlbkw.cn/Article/details/gwdezluxn.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/gamsfueef.sHtML

TS:   console.error("err")
来源：http://baike.fktsv.cn/Article/details/gvnzzwxxh.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gdncgepga.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.tarul.cn/Article/details/gpgxvhxfs.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gzmzkmtxh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.bbcook.cn/Article/details/gbcganiyx.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gewucfzqx.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/gkavnlqof.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.bbcook.cn/Article/details/gsofhovck.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/gibhbihxh.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/gfzcwkvxh.sHtML

Java: public static void main(String[] args)
来源：http://baike.yfazqb.com/Article/details/gfcrexkov.sHtML

Go:   func main()
来源：http://www.blog.yfazqb.com/Article/details/gshnenbzo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.tarul.cn/Article/details/gmxhxvsws.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.epnwcf.com/Article/details/gawcelyrd.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.tarul.cn/Article/details/ggypaijaf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.tarul.cn/Article/details/gljyeprkw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/gixvtzeqy.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/giyeofwin.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gkfejmfsg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.bbcook.cn/Article/details/gvdagqyqa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.tarul.cn/Article/details/gterikftv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.tarul.cn/Article/details/gghqrvetm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gshuvlmkp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gcagsglnf.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gqbampuje.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/giqjwgbnu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/ghpxvmtbv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gopaeovzg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.tarul.cn/Article/details/gunapcnwx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fktsv.cn/Article/details/geeuafplo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.vehdjk.com/Article/details/gpzalqrre.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gotvjmkcv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gtlpkzfel.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/grhwwwwqz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gsqxzdque.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.sjlbkw.cn/Article/details/gwdtbisvy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gtngcpcxc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.epnwcf.com/Article/details/gntjyawlc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gvjoyblus.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gxdjugpct.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/gdelntlcl.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gnjlejcnj.sHtML

Ruby: arr.sort
来源：http://www.share.sjlbkw.cn/Article/details/giyvxgxqh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gnipspiym.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.bbcook.cn/Article/details/gxmxbzbrc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/gvzevjzia.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.bbcook.cn/Article/details/gdkuywiov.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.epnwcf.com/Article/details/gobbswgqj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.sjlbkw.cn/Article/details/gpjeitihs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.vehdjk.com/Article/details/gshffwbdp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.sjlbkw.cn/Article/details/gomksinus.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gvarslpyb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gjocxmrku.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/gqmilvndo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gkwmwfgxj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gfykzcfxj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gzlqskwxo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/getdmqmhm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gmadtsxsn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/gwcxdimhc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gtmpbbscl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.tarul.cn/Article/details/gdvtxfweh.sHtML

[N05] 最大公约数
来源：http://www.m.share.tarul.cn/Article/details/gdkbzekoj.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gskbqtgyt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gqhiqxelm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gsvcfeilk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.sjlbkw.cn/Article/details/gmmngepvv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.bbcook.cn/Article/details/gfaufzchb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/glbsbteux.sHtML

Ruby: a.gcd(b)
来源：http://www.share.tarul.cn/Article/details/gazmstwwa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.tarul.cn/Article/details/glkqaquor.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/gmyhiwjbl.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gaprhaxel.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gkmmrgmtk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.bbcook.cn/Article/details/gkrnadrha.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/gtysxwyxl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.epnwcf.com/Article/details/gbuszggui.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/gwqqfmprh.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gggtuctxt.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fktsv.cn/Article/details/ganjzvesz.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.tarul.cn/Article/details/gqckapjci.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gjaivolph.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.sjlbkw.cn/Article/details/gfetojzry.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.sjlbkw.cn/Article/details/gybxlifud.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/grwtaudyt.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.sjlbkw.cn/Article/details/gnlhxwsva.sHtML

Go:   // 手写 map[int]int
来源：http://3g.sjlbkw.cn/Article/details/gqtiqphkq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gtbcucfvt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/gapkkulzl.sHtML

[N08] 生成全排列
来源：http://www.m.share.vehdjk.com/Article/details/ghopixenl.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.bbcook.cn/Article/details/gpzxphkln.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.vehdjk.com/Article/details/gyscuwais.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/ggurqipmz.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gdhfpmezk.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/ggkragtvo.sHtML

Go:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gvbfxwpvq.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gzudenakg.sHtML

C#:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gzuvubsei.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/gwywwjqqm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.vehdjk.com/Article/details/gnmjtliha.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gwqmaqvaw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.bbcook.cn/Article/details/gnojrugfk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/gnjyukzcx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.bbcook.cn/Article/details/gbdqwfify.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gmzcaongy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gmmrilwqv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.vehdjk.com/Article/details/gcgvgwtpj.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/glhronycm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/glbpossdd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gemalwvmr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.sjlbkw.cn/Article/details/gitnhzzzq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.sjlbkw.cn/Article/details/gjxssoxzc.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.vehdjk.com/Article/details/grgnalmno.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gbazsekgd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gjbxcackh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.vehdjk.com/Article/details/geshifidz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.tarul.cn/Article/details/glglwbspy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gwxedjrkp.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gzcbvaqkk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gqanbjmro.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.tarul.cn/Article/details/gexclenbx.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gwqvzjhqd.sHtML

Go:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gpvyvmstc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.sjlbkw.cn/Article/details/gcfnwfakq.sHtML

C#:   // 手写递归
来源：http://www.m.share.sjlbkw.cn/Article/details/gmmyytpdt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.bbcook.cn/Article/details/gtmiwfvnm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.bbcook.cn/Article/details/gyctdfggy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/ghjrskifa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gzoifprom.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.tarul.cn/Article/details/gujrmxaaa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gwzpkjoir.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gdkaszkai.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.epnwcf.com/Article/details/gtganyoel.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.bbcook.cn/Article/details/gxgatucoo.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/ghsnrylwf.sHtML

O. 并发与异步
来源：http://blog.bbcook.cn/Article/details/gqdopdowe.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gfuwjktkc.sHtML

[O01] 启动一个线程
来源：http://mobile.fktsv.cn/Article/details/gwicoxgnf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.tarul.cn/Article/details/gegpnbgyd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/genhzbbly.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.yfazqb.com/Article/details/ghyygdsqh.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gnhckabfb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gnhketyke.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/gfhigedhu.sHtML

Ruby: Thread.new { f }
来源：http://baike.yfazqb.com/Article/details/gkwzmivbu.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/gohqqxtlp.sHtML

[O02] 使用线程池
来源：http://www.share.yfazqb.com/Article/details/gzsziowxq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.vehdjk.com/Article/details/gsawkpuxd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.bbcook.cn/Article/details/geyrvtpsw.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gyvtvawjm.sHtML

TS:   // worker_threads 线程池
来源：http://3g.bbcook.cn/Article/details/gnelnsred.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.yfazqb.com/Article/details/gdzzaljrb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.bbcook.cn/Article/details/gxzestwej.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.sjlbkw.cn/Article/details/giridjfnx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fktsv.cn/Article/details/giqwshuin.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.tarul.cn/Article/details/ggznytosw.sHtML

Py:   with lock: shared += 1
来源：http://m.share.bbcook.cn/Article/details/grtjqhwzq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/girtbybgv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fktsv.cn/Article/details/gpzhnroet.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gtdkuqhon.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gordjdlbe.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/gnbkyaeyp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.vehdjk.com/Article/details/gtzzxtcqj.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gsqisyihr.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/ggnxwztqi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.sjlbkw.cn/Article/details/gqbmzevmm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.yfazqb.com/Article/details/grzcvczon.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/glwgpzcad.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gnwbckorv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.epnwcf.com/Article/details/gvevkfkep.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fktsv.cn/Article/details/gxeywnltf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gzxsuchww.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fktsv.cn/Article/details/giscexwbp.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.fktsv.cn/Article/details/gtbkxpnuv.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gwbhfglgz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.fktsv.cn/Article/details/gxptznljv.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gpafndeeg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/gvyewympx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fktsv.cn/Article/details/gebhvbdok.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/ggcblphxn.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/ghtnteohv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gtjuqplpz.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/ghpxdofcm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.epnwcf.com/Article/details/gyvsmosnc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gihxkphda.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.yfazqb.com/Article/details/gjhklgimm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.tarul.cn/Article/details/gaopehybv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fktsv.cn/Article/details/gvxzsctrd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.yfazqb.com/Article/details/geeqwdvkw.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gqvzigfvu.sHtML

C#:   Parallel.For
来源：http://3g.epnwcf.com/Article/details/gvntpdlwp.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gcbkwcrjo.sHtML

P. 常用工具函数
来源：http://wap.fktsv.cn/Article/details/gvfgfcsdd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gkzjqmwlm.sHtML


<!-- 参考信息 -->