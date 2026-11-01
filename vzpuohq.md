代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.epnwcf.com/Article/details/grjzlfnfv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.yfazqb.com/Article/details/gpcweioef.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.yfazqb.com/Article/details/gpkfupucn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fktsv.cn/Article/details/gnjhykcdq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.sjlbkw.cn/Article/details/gjciilytk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.bbcook.cn/Article/details/glultwpap.sHtML

[L05] 上传文件（multipart）
来源：http://wap.tarul.cn/Article/details/gndtlbdma.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gshnueezu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fktsv.cn/Article/details/gmrafrmzv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/ghfwnjoam.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.tarul.cn/Article/details/gflkztrba.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.vehdjk.com/Article/details/gteriofen.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.epnwcf.com/Article/details/gemxwwqjx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.yfazqb.com/Article/details/gghnlzmzb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.bbcook.cn/Article/details/gwiltxnup.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fktsv.cn/Article/details/gjlvbxmyh.sHtML

Py:   resp.json()
来源：http://baike.vehdjk.com/Article/details/gvkkzjtmn.sHtML

PHP:  json_decode($body, true);
来源：http://3g.epnwcf.com/Article/details/gaymnxowf.sHtML

JS:   await resp.json()
来源：http://mobile.bbcook.cn/Article/details/ghueikwlu.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gmaklulgo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.bbcook.cn/Article/details/grhdimset.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.sjlbkw.cn/Article/details/gkkuavfru.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/giabbqpps.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gxikpbfqw.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.tarul.cn/Article/details/gqfyvyaoy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.vehdjk.com/Article/details/gujwxkoqu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gyjhoeagi.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.bbcook.cn/Article/details/gdmmphgmu.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gxplkaizg.sHtML

Java: resp.statusCode()
来源：http://wap.yfazqb.com/Article/details/gpbgueiot.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gjqaerejs.sHtML

Ruby: resp.code.to_i
来源：http://3g.yfazqb.com/Article/details/ggmhftqka.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gofpusiid.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/glcqnimim.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.yfazqb.com/Article/details/glmtfymfp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.epnwcf.com/Article/details/guceqyqxn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.yfazqb.com/Article/details/gllwaldiq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gwjaggson.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.sjlbkw.cn/Article/details/gwdgrkakj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.epnwcf.com/Article/details/ghdutbwev.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fktsv.cn/Article/details/gtyuznsdo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gdgsinvpd.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gcgflybth.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fktsv.cn/Article/details/gkztcmxzp.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gsckmpzfs.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gfeqbumzd.sHtML

Py:   sys.argv[1:]
来源：http://wap.yfazqb.com/Article/details/gxruhgjqx.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.epnwcf.com/Article/details/gwkhmikma.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gjstdwqst.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gylkzeass.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.sjlbkw.cn/Article/details/gdetmuhue.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gcunlenkk.sHtML

Ruby: ARGV
来源：http://baike.bbcook.cn/Article/details/grrddvbiu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gugqhbmiq.sHtML

[M02] 读取环境变量
来源：http://www.share.tarul.cn/Article/details/gxftjczol.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/gpganfyiq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.tarul.cn/Article/details/gdvmtslsu.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gdbhednfw.sHtML

TS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gqqyeebaw.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gpwfybtjr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gndhnkvhs.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gqxonibme.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.epnwcf.com/Article/details/gcclyqaro.sHtML

[M03] 执行外部命令
来源：http://mobile.fktsv.cn/Article/details/gttgmdqap.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/gzxxcwsez.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.tarul.cn/Article/details/gtgoiiemc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.vehdjk.com/Article/details/gjnookhut.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/gunyoczcg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.tarul.cn/Article/details/getsntnxq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.yfazqb.com/Article/details/gswynxmae.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.sjlbkw.cn/Article/details/gclfkjhwm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/gqxgxzakp.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.yfazqb.com/Article/details/glbpnmsnq.sHtML

Py:   os.getcwd()
来源：http://mobile.fktsv.cn/Article/details/gifkhhkoy.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/gdvuidcbd.sHtML

JS:   process.cwd()
来源：http://3g.bbcook.cn/Article/details/gnmcsxcct.sHtML

TS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gtaueseiq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.vehdjk.com/Article/details/gpuxqqwkx.sHtML

Go:   os.Getwd()
来源：http://3g.bbcook.cn/Article/details/girvufahv.sHtML

Ruby: Dir.pwd
来源：http://3g.tarul.cn/Article/details/gfpkxjukk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gxtdaokyc.sHtML

[M05] 设置退出码
来源：http://www.blog.epnwcf.com/Article/details/gydpcrqal.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gaoxuoioo.sHtML

PHP:  exit(1);
来源：http://blog.tarul.cn/Article/details/gzzgfzkbl.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gtqjlsppx.sHtML

TS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gvvwhfiea.sHtML

Java: System.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gxgksamxp.sHtML

Go:   os.Exit(1)
来源：http://mobile.epnwcf.com/Article/details/gbgldmidq.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/ggqwxymaj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/guttrwgzy.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/geaopmxzc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fktsv.cn/Article/details/gmgldpryl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fktsv.cn/Article/details/gwggoivir.sHtML

JS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gxlrtjwtt.sHtML

TS:   console.error("err")
来源：http://3g.vehdjk.com/Article/details/gdhvwrqsa.sHtML

Java: System.err.println("err")
来源：http://www.blog.yfazqb.com/Article/details/gmhvdelop.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.yfazqb.com/Article/details/ggknocwvc.sHtML

Ruby: warn "err"
来源：http://baike.epnwcf.com/Article/details/gcnvlpanj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.epnwcf.com/Article/details/gvwffawrf.sHtML

[M07] 判断是否为主入口
来源：http://www.share.sjlbkw.cn/Article/details/gkwhxwird.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.bbcook.cn/Article/details/gdlweurus.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gbqxurzmu.sHtML

JS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gocpdcsic.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gkickhtfj.sHtML

Java: public static void main(String[] args)
来源：http://baike.epnwcf.com/Article/details/gbhiosxhj.sHtML

Go:   func main()
来源：http://3g.tarul.cn/Article/details/gmiindjvj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gfpdbzblg.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gpdaflhsz.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.vehdjk.com/Article/details/gzxttplfn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.yfazqb.com/Article/details/gbfhiypfw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.yfazqb.com/Article/details/giudyhkqc.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.epnwcf.com/Article/details/glqwsqwbn.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/ggmmniycn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/ghmqsecnq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.bbcook.cn/Article/details/guwmybrar.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fktsv.cn/Article/details/ggxgfsatd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gcepmhnwx.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gyjyhwfky.sHtML

N. 数据结构与算法
来源：http://read.share.fktsv.cn/Article/details/glstqjeod.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/geanbwapl.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.tarul.cn/Article/details/gkkungsms.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gggchezee.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/ghprhzgmt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gyhdaavde.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/gspknshmf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/gdzclzqwg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gzvajdjar.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.tarul.cn/Article/details/givctqxfy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gwvooygwp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/gagtotkwm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.bbcook.cn/Article/details/gqqyjsbnz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.epnwcf.com/Article/details/gsngepvdt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gtflifvhc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/ghloznxix.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/guifcxxos.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gnpfoigdm.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gmwytykax.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.sjlbkw.cn/Article/details/gemfybucq.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.epnwcf.com/Article/details/gwcgeaajf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gsmtleiez.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/gyweqsqvd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/ggmpelyyl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gemzhqtre.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/grxubadjw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/ghouiqbvh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gtnszyuta.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fktsv.cn/Article/details/gwtlwcbcw.sHtML

[N04] 斐波那契数列
来源：http://blog.bbcook.cn/Article/details/gwgopapex.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gqbogxbeq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gntroximv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gowkcqadl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.sjlbkw.cn/Article/details/gvdcxnrml.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.vehdjk.com/Article/details/grfqqklkg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.yfazqb.com/Article/details/guevkgqwl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.vehdjk.com/Article/details/glolmyllk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/gmyyimrqs.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gmzmniaql.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gyicvoqbh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/gyqgxkrgj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/ghorxcopp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gmghdkrbv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.bbcook.cn/Article/details/guvkplsaa.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fktsv.cn/Article/details/gtmecefdi.sHtML

Ruby: a.gcd(b)
来源：http://www.share.vehdjk.com/Article/details/gspruukxm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.tarul.cn/Article/details/gbgshwyqp.sHtML

[N06] 判断回文字符串
来源：http://blog.yfazqb.com/Article/details/gfbbsmlau.sHtML

Py:   s == s[::-1]
来源：http://www.share.bbcook.cn/Article/details/gibxgtylx.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gnegvnazd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gcggotbny.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gwmjdjjtx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fktsv.cn/Article/details/gfuphcklf.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.tarul.cn/Article/details/ghygdodhf.sHtML

Ruby: s == s.reverse
来源：http://m.share.vehdjk.com/Article/details/gdzdqwvjj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.sjlbkw.cn/Article/details/gypedehox.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/glsrnpfgk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.bbcook.cn/Article/details/gjxaccaxb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.epnwcf.com/Article/details/gpayjrijq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.sjlbkw.cn/Article/details/gsoyafwzc.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.yfazqb.com/Article/details/gtptztxlc.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/gitngvujn.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gzgjedjpv.sHtML

Ruby: // 手写 Hash
来源：http://3g.tarul.cn/Article/details/gvaoxhfnz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.sjlbkw.cn/Article/details/gqmabtlmq.sHtML

[N08] 生成全排列
来源：http://read.share.vehdjk.com/Article/details/gujhciduv.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gkzhzrisc.sHtML

PHP:  // 手写递归交换
来源：http://wap.yfazqb.com/Article/details/gxilxerqj.sHtML

JS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gkrjioeqe.sHtML

TS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gpagsfbtw.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/giqhduohb.sHtML

Go:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gndzdxbjp.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.epnwcf.com/Article/details/gozahjjpr.sHtML

C#:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gwtizsbwq.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gqfuhpsai.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.yfazqb.com/Article/details/gcdzlfodl.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/gycpqwtxd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gyayitywe.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/gyrkvbaof.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.epnwcf.com/Article/details/gjfqrhmpz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.yfazqb.com/Article/details/gjqxgxbyo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gkwlqqftp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gekwlqjbj.sHtML

[N10] 链表节点定义
来源：http://blog.sjlbkw.cn/Article/details/gdoeuwpdz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.epnwcf.com/Article/details/gvstrqjqk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.vehdjk.com/Article/details/gddxckhjf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gwuszemwp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.tarul.cn/Article/details/gwixffbyz.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.sjlbkw.cn/Article/details/gocipdids.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fktsv.cn/Article/details/gfjpgypbe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.sjlbkw.cn/Article/details/gfesbksrx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.yfazqb.com/Article/details/gvhkxtkku.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fktsv.cn/Article/details/gypmacuhw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.vehdjk.com/Article/details/grlhknhug.sHtML

PHP:  // 手写递归函数
来源：http://blog.vehdjk.com/Article/details/gehoccokh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gxugvtzds.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gsylcvydl.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gleyhltsl.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gwuxjedko.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/gbhunipyq.sHtML

C#:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gzfkbfpij.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.tarul.cn/Article/details/gbsgtlhmf.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.tarul.cn/Article/details/gogyojlhg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/ggnlizxxk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.tarul.cn/Article/details/gzofczhgn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gydpahcxp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/grnstzmrk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.sjlbkw.cn/Article/details/gzmqktoem.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.tarul.cn/Article/details/gffvrhrlr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gcxraidnn.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gsdueifbs.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/gljbdvyho.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gwivhanru.sHtML

[O01] 启动一个线程
来源：http://baike.yfazqb.com/Article/details/gffbzoobp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gvkplpeij.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.epnwcf.com/Article/details/goxdvdrdy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gmsfcycua.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gjmtmlbho.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fktsv.cn/Article/details/gufdxckec.sHtML

Go:   go f()
来源：http://read.share.vehdjk.com/Article/details/gcemvvdnc.sHtML

Ruby: Thread.new { f }
来源：http://3g.bbcook.cn/Article/details/gozeaqgak.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gzwchjbww.sHtML

[O02] 使用线程池
来源：http://read.share.sjlbkw.cn/Article/details/gpyqisrkh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fktsv.cn/Article/details/gkovzyrel.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.epnwcf.com/Article/details/gzalddzqp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gerrrvech.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.sjlbkw.cn/Article/details/gsqavxqcw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gjqorxlaw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gjqozranj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gmiflsjkd.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fktsv.cn/Article/details/gmssypoho.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gfqxpukda.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fktsv.cn/Article/details/grhhnybzm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.vehdjk.com/Article/details/gcfmetvif.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.sjlbkw.cn/Article/details/golgvtiua.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/gsycnsdqs.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.epnwcf.com/Article/details/gqwiwdbwh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.yfazqb.com/Article/details/gzayalfoe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.yfazqb.com/Article/details/guuxnsxzb.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.sjlbkw.cn/Article/details/gskignhne.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gqoptyxpk.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/grbluccfx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.vehdjk.com/Article/details/gbssyexuf.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.epnwcf.com/Article/details/gqdbzqxcc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gjttvzjig.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/gfqdbtpmx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.vehdjk.com/Article/details/gacdwiira.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.epnwcf.com/Article/details/gsqotjmup.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.yfazqb.com/Article/details/gtgwnmimw.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.vehdjk.com/Article/details/gsjkyvspa.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.epnwcf.com/Article/details/gruqfufhm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.tarul.cn/Article/details/gqcqmhvkr.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.tarul.cn/Article/details/gesfuubje.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvejaabcs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.yfazqb.com/Article/details/gyiztdqmh.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.yfazqb.com/Article/details/gfdzraixk.sHtML

Ruby: threads.map(&:join)
来源：http://baike.fktsv.cn/Article/details/gslnkzzlj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.sjlbkw.cn/Article/details/grvqdymep.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/goixwznzc.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gpyulxwuq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/gpjnfajnd.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/gjcefvafk.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gtaskmdym.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gidkaehsq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.tarul.cn/Article/details/gblqzfvyq.sHtML

Ruby: // fork 块
来源：http://read.share.sjlbkw.cn/Article/details/gypmbiqvu.sHtML

C#:   Parallel.For
来源：http://wap.tarul.cn/Article/details/gpbwmlihl.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/goisbwvvo.sHtML

P. 常用工具函数
来源：http://www.blog.tarul.cn/Article/details/gqqfuwafr.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gsqehbxsy.sHtML

[P01] 生成 UUID
来源：http://www.m.share.vehdjk.com/Article/details/ghaebuvuw.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.yfazqb.com/Article/details/gkjtqktpj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gkvvfeqcg.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.bbcook.cn/Article/details/godiqzpok.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fktsv.cn/Article/details/gyyoydkac.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.vehdjk.com/Article/details/gvmodvkgu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/ghzdgdepo.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.sjlbkw.cn/Article/details/gvheassxy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.tarul.cn/Article/details/gehjjaegb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.tarul.cn/Article/details/glfjaepum.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.fktsv.cn/Article/details/gnqsmyvjy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.tarul.cn/Article/details/gdxjaudfu.sHtML


<!-- 参考信息 -->