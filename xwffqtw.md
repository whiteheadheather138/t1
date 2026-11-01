代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.vehdjk.com/Article/details/gzdtzdmdl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fktsv.cn/Article/details/gxfkugule.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.vehdjk.com/Article/details/gcxdyetbr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.bbcook.cn/Article/details/gajitftbg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.bbcook.cn/Article/details/guihynaxs.sHtML

[L04] 设置超时
来源：http://read.share.bbcook.cn/Article/details/girkzmpff.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gncnlozrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.epnwcf.com/Article/details/gfsegtfph.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.sjlbkw.cn/Article/details/gkdywcmgm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.bbcook.cn/Article/details/gkhcjwcsl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.epnwcf.com/Article/details/ggohfaycb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.sjlbkw.cn/Article/details/gdssbffdp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gctcqylti.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.vehdjk.com/Article/details/gebnorlmz.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.tarul.cn/Article/details/gcoetzsnb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.vehdjk.com/Article/details/gqhpzxvsc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fktsv.cn/Article/details/gnxxuhukj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.epnwcf.com/Article/details/grpsagzck.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.vehdjk.com/Article/details/gqmyvxnti.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.sjlbkw.cn/Article/details/gtejpllzj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.epnwcf.com/Article/details/gisrnqdno.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.epnwcf.com/Article/details/glynaoxrr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.bbcook.cn/Article/details/gsbhlhjop.sHtML

[L06] 解析响应为 JSON
来源：http://wap.epnwcf.com/Article/details/grmxphqzp.sHtML

Py:   resp.json()
来源：http://m.share.epnwcf.com/Article/details/gtbfkxqvx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/gmfetmkeg.sHtML

JS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/glvwxpqnw.sHtML

TS:   await resp.json()
来源：http://m.share.epnwcf.com/Article/details/geyvkaoog.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gwiactkwo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.sjlbkw.cn/Article/details/gxneucrfk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.sjlbkw.cn/Article/details/gfpuuteuj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.yfazqb.com/Article/details/gzienksdb.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gtgbxbdul.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.tarul.cn/Article/details/gsoksazth.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.tarul.cn/Article/details/gcelzomym.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.yfazqb.com/Article/details/genlpatky.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.bbcook.cn/Article/details/gtcfcdbzt.sHtML

Java: resp.statusCode()
来源：http://3g.yfazqb.com/Article/details/grlnszrgn.sHtML

Go:   resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/grbdvlxdn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.epnwcf.com/Article/details/gwkohhvul.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.vehdjk.com/Article/details/ggojehgbm.sHtML

[L08] 并发请求多个地址
来源：http://blog.vehdjk.com/Article/details/gtpdzcoqo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gmtthflzk.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fktsv.cn/Article/details/gydcsicwk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.epnwcf.com/Article/details/gyxewmdmk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.vehdjk.com/Article/details/ggzakcgdr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gnpsqkvnt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gwgzqagua.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/gvgwrzcvc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gzdzzwsdm.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/giuijcxpq.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gxjxaqybs.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/genacjyiz.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/gdofdudst.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gbhzfodvu.sHtML

PHP:  $argv;  $argc;
来源：http://wap.vehdjk.com/Article/details/gaphjcmzz.sHtML

JS:   process.argv.slice(2)
来源：http://3g.tarul.cn/Article/details/gulspdyar.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gxetibxbj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.vehdjk.com/Article/details/glmfrmtqb.sHtML

Go:   os.Args[1:]
来源：http://3g.tarul.cn/Article/details/gicqihyig.sHtML

Ruby: ARGV
来源：http://wap.vehdjk.com/Article/details/gftuihscf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/gxjwseeyt.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gvrtnkafa.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/ghxmllwox.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.sjlbkw.cn/Article/details/gwvmvrblw.sHtML

JS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gpzwzqrjz.sHtML

TS:   process.env.HOME
来源：http://www.share.sjlbkw.cn/Article/details/glpdcprhi.sHtML

Java: System.getenv("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gbhpaxdjs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gvpellqjd.sHtML

Ruby: ENV["HOME"]
来源：http://3g.sjlbkw.cn/Article/details/gdtwfyjkl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.vehdjk.com/Article/details/gfqtwllyf.sHtML

[M03] 执行外部命令
来源：http://read.share.fktsv.cn/Article/details/ghduzpxnc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.bbcook.cn/Article/details/gahdnnkda.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/grrrgdwgi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gnwpuokwf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/ggguwcvmr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.vehdjk.com/Article/details/goppvcriw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.epnwcf.com/Article/details/gingpoqfw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/gxxohbhyn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.vehdjk.com/Article/details/gixukpfxa.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/gnjoesrvb.sHtML

Py:   os.getcwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gkyxmqilj.sHtML

PHP:  getcwd();
来源：http://read.share.fktsv.cn/Article/details/gbbjahhbo.sHtML

JS:   process.cwd()
来源：http://mobile.yfazqb.com/Article/details/ghgsrdngv.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/gvkjjxbcp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gatltbabf.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/gyjknjktd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.tarul.cn/Article/details/gvymgrqve.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gkonxvkaq.sHtML

[M05] 设置退出码
来源：http://www.m.share.epnwcf.com/Article/details/gbomarrrt.sHtML

Py:   sys.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gmiascmyr.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/gtclcokmv.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gyekdhehh.sHtML

TS:   process.exit(1)
来源：http://www.blog.tarul.cn/Article/details/gtuegrmgo.sHtML

Java: System.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gzmixppmr.sHtML

Go:   os.Exit(1)
来源：http://blog.fktsv.cn/Article/details/glexlkznf.sHtML

Ruby: exit 1
来源：http://www.blog.yfazqb.com/Article/details/gmnzmgvun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gwfydjdiq.sHtML

[M06] 向标准错误输出
来源：http://www.share.fktsv.cn/Article/details/gynbgpmvy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.sjlbkw.cn/Article/details/gqahluudx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fktsv.cn/Article/details/gmjgmwhsk.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gaqrkpthv.sHtML

TS:   console.error("err")
来源：http://mobile.sjlbkw.cn/Article/details/gxmemcnem.sHtML

Java: System.err.println("err")
来源：http://www.blog.yfazqb.com/Article/details/gqtvosjvo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fktsv.cn/Article/details/gpdnttkzr.sHtML

Ruby: warn "err"
来源：http://read.share.yfazqb.com/Article/details/gltkmvnuq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.vehdjk.com/Article/details/gjlfxxmou.sHtML

[M07] 判断是否为主入口
来源：http://wap.sjlbkw.cn/Article/details/gsgzezarz.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.epnwcf.com/Article/details/gsgtgstdv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.epnwcf.com/Article/details/gyxbpbvko.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/getffxzfd.sHtML

TS:   require.main === module
来源：http://read.share.epnwcf.com/Article/details/gnfarwejg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.tarul.cn/Article/details/gcthqsxfy.sHtML

Go:   func main()
来源：http://3g.fktsv.cn/Article/details/gnkgebymk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.epnwcf.com/Article/details/gpmtgeupz.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.yfazqb.com/Article/details/ganzeqnjx.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fktsv.cn/Article/details/grkmwxkzn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.epnwcf.com/Article/details/gpwfsprcu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.sjlbkw.cn/Article/details/gcgbudrwr.sHtML

JS:   process.platform;  process.version
来源：http://wap.yfazqb.com/Article/details/gshqynich.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gdgjvveho.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.vehdjk.com/Article/details/giwonnafu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/gheknvzlb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.epnwcf.com/Article/details/goylhvpau.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gkguuzssw.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gucjvjvrl.sHtML

N. 数据结构与算法
来源：http://www.blog.bbcook.cn/Article/details/gwlkcrgsb.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdwcaaghz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.epnwcf.com/Article/details/gsbhajrhu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.yfazqb.com/Article/details/goarkqzjq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/glsurgyvs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gzynfuzau.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gbezirgsi.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.vehdjk.com/Article/details/gxepitdqy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ghjjrjhad.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.tarul.cn/Article/details/gwthvmlft.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/gxkenanmg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.vehdjk.com/Article/details/gwvvjwnwv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gjcvrtbjj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gzfjktbjo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.epnwcf.com/Article/details/gydukjdzq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gaklpxybq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/gfbwimwph.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gsnjlptam.sHtML

Ruby: arr.sort
来源：http://m.share.tarul.cn/Article/details/gssyaalhj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/ggqqcvohk.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.sjlbkw.cn/Article/details/gnzewfgvn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.epnwcf.com/Article/details/gradsefvq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fktsv.cn/Article/details/gnlpxhpxs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gytcehcrb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/ggwpwcdib.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gphmtktlu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.tarul.cn/Article/details/gibgrylqt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.vehdjk.com/Article/details/gldvilekm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.tarul.cn/Article/details/gmltkzjuj.sHtML

[N04] 斐波那契数列
来源：http://mobile.vehdjk.com/Article/details/gormnodgj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.vehdjk.com/Article/details/gjhndraif.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/gemtndmpz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gtzvswklt.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gnrkmdtvd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gjycccrhg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gbwqgjxtg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gcsogciua.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.sjlbkw.cn/Article/details/gavbcomfa.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gpwvfisfp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.yfazqb.com/Article/details/gaaogppii.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.bbcook.cn/Article/details/gvbwkcgon.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gnobbyvtu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fktsv.cn/Article/details/gvhkfxtdg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.sjlbkw.cn/Article/details/gqawjmuki.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.yfazqb.com/Article/details/gipxwoybj.sHtML

Ruby: a.gcd(b)
来源：http://baike.sjlbkw.cn/Article/details/gfimsuzsl.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.vehdjk.com/Article/details/gvoynnuod.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/ghwllseoq.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/gcdhbtzfq.sHtML

PHP:  $s === strrev($s);
来源：http://blog.epnwcf.com/Article/details/gnnfpjyry.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gasbyzudx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gdctgitqf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.vehdjk.com/Article/details/gqotqbkxa.sHtML

Go:   // 双指针从两端比较
来源：http://blog.bbcook.cn/Article/details/gujhoxhgr.sHtML

Ruby: s == s.reverse
来源：http://3g.bbcook.cn/Article/details/gxqsnbkax.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.vehdjk.com/Article/details/gfcpsenax.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.bbcook.cn/Article/details/glikwxxev.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.yfazqb.com/Article/details/gzfzdrpyr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/geociscxj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gbsafdtcc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.sjlbkw.cn/Article/details/gbwdrkyhx.sHtML

Java: // 手写 HashMap
来源：http://blog.vehdjk.com/Article/details/gfialcord.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.sjlbkw.cn/Article/details/gbewgfjjm.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gzkzcawyv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.epnwcf.com/Article/details/gujpczrou.sHtML

[N08] 生成全排列
来源：http://3g.fktsv.cn/Article/details/gnwhlxejt.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gwzqhkxgd.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/getzokyrv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/ggyojrctv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gmxnpfbda.sHtML

Java: // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gcpaegwls.sHtML

Go:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gbnifgcqz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.bbcook.cn/Article/details/gjskjetxx.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gvfhaxgfz.sHtML

[N09] 栈与队列
来源：http://read.share.fktsv.cn/Article/details/ggnaauepx.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gxxwasizg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gjcnjqpza.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gsywxgdie.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fktsv.cn/Article/details/giqvqepxw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gksijpqhi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fktsv.cn/Article/details/gspudcrvj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.vehdjk.com/Article/details/goueobyxq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fktsv.cn/Article/details/gnyxzpoqt.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gfrwqcbmz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.epnwcf.com/Article/details/gkfknaiby.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gkrcusppr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.yfazqb.com/Article/details/goovflgee.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gbcqwpcxj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.bbcook.cn/Article/details/gcflrwxkl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.sjlbkw.cn/Article/details/gibewbyjw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/gpvcnacru.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.vehdjk.com/Article/details/gbgmotiau.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.bbcook.cn/Article/details/gbqiydbhm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gwlndwcyd.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/gkirijezo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/geoonaolq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gixdkseqy.sHtML

Java: // 手写递归
来源：http://blog.yfazqb.com/Article/details/goxvyrejh.sHtML

Go:   // 手写递归
来源：http://www.share.fktsv.cn/Article/details/ghklzimny.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/gfgzuqxep.sHtML

C#:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gpbjhdiyo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.yfazqb.com/Article/details/gvifhxthj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gmnxdbxhf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.tarul.cn/Article/details/glehsivbr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/ghhtvoldr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.vehdjk.com/Article/details/gtqhulyqf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gzcwkrdca.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gcxaxdftv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.sjlbkw.cn/Article/details/gqpjnuukd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/ghmfwetnv.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/guoezxaja.sHtML

O. 并发与异步
来源：http://wap.yfazqb.com/Article/details/glvwvtyqg.sHtML

================================================================================
来源：http://baike.fktsv.cn/Article/details/gchnlpcjo.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/gecfcqxbo.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.bbcook.cn/Article/details/gdzvisqxr.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/gecoawbga.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.bbcook.cn/Article/details/grbilboxd.sHtML

TS:   // 同 JS
来源：http://www.m.share.yfazqb.com/Article/details/giqepvcca.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.vehdjk.com/Article/details/gvjpsfidh.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gzuhqwggz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.bbcook.cn/Article/details/gtoxycmob.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fktsv.cn/Article/details/gfaligqbk.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gjrwmkuly.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gqpecbnji.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.sjlbkw.cn/Article/details/gsewpytlm.sHtML

JS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gxwycqdke.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gkwgtjemv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/giwaqnorj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.sjlbkw.cn/Article/details/gpuvdcxqh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.tarul.cn/Article/details/gaepsswnb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.fktsv.cn/Article/details/gntdzpabc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.epnwcf.com/Article/details/ghbwuzyaq.sHtML

Py:   with lock: shared += 1
来源：http://baike.yfazqb.com/Article/details/gxzjuukxk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.sjlbkw.cn/Article/details/gchrcxber.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.epnwcf.com/Article/details/gkwkklmfp.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gszjsiupl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.epnwcf.com/Article/details/gqgibhtys.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/gzszqlxyz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.vehdjk.com/Article/details/giisrdtaz.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkrjrepkg.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gmxtxuprp.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.epnwcf.com/Article/details/gukgmazgo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.sjlbkw.cn/Article/details/gsgctrvab.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/gziobfnlq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gdordzvcv.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.epnwcf.com/Article/details/gnfnxpxhy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gjkzflvbk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/ghjerpagv.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.vehdjk.com/Article/details/gjmqxcosc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fktsv.cn/Article/details/gbtfjjczw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.epnwcf.com/Article/details/givclnehh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/gxvgppdlk.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gpsfvtcvr.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gzojxurkl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaasxmdeb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/gazpzltxs.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/ghukrnfgo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gupeyoxil.sHtML

[O06] 使用进程池
来源：http://www.blog.yfazqb.com/Article/details/gypeayrdi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/gtbmutlod.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fktsv.cn/Article/details/gypffmpmc.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/goglujknv.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/gcyurfdmy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gcjpqnexd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.bbcook.cn/Article/details/giezmazvt.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gxkzfhhxu.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/gpfyusjxm.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gecbkqzpc.sHtML

P. 常用工具函数
来源：http://mobile.vehdjk.com/Article/details/gybrvjuwa.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gupmuwtdl.sHtML

[P01] 生成 UUID
来源：http://3g.vehdjk.com/Article/details/gnunxyrtp.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.yfazqb.com/Article/details/gzwvixsvv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.yfazqb.com/Article/details/gwoviltib.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gbteidjei.sHtML


<!-- 参考信息 -->