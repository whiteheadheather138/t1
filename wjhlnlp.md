代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.bbcook.cn/Article/details/gilhriaii.sHtML

[L04] 设置超时
来源：http://read.share.vehdjk.com/Article/details/glvzvoswo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.bbcook.cn/Article/details/gnnvcbdko.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.yfazqb.com/Article/details/gmslhiqdi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.epnwcf.com/Article/details/gxcsapckf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.epnwcf.com/Article/details/gbqqgsafw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.sjlbkw.cn/Article/details/gawlpelgy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fktsv.cn/Article/details/gatimtffa.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.yfazqb.com/Article/details/gglhiuzwf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.epnwcf.com/Article/details/gojiwxyjf.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.bbcook.cn/Article/details/gwjibtvwh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.yfazqb.com/Article/details/gtgcdqlnt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fktsv.cn/Article/details/gppcneauy.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gvaerwciz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.yfazqb.com/Article/details/gsomqyobo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.yfazqb.com/Article/details/gxuftgizb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.tarul.cn/Article/details/gxzvayuwx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.tarul.cn/Article/details/goqnbypub.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.bbcook.cn/Article/details/gaxxqmaza.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.tarul.cn/Article/details/gzfhypgcl.sHtML

Py:   resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gpwtllvpe.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.tarul.cn/Article/details/gjcahcktz.sHtML

JS:   await resp.json()
来源：http://blog.yfazqb.com/Article/details/gvhpuzold.sHtML

TS:   await resp.json()
来源：http://read.share.fktsv.cn/Article/details/gikoexetm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.sjlbkw.cn/Article/details/geajdubkt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.bbcook.cn/Article/details/gnpvpmsmf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.bbcook.cn/Article/details/gnysufvoe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.tarul.cn/Article/details/gvynowafe.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fktsv.cn/Article/details/gytbnqgpa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.bbcook.cn/Article/details/gntnncyuf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.tarul.cn/Article/details/galtnzyvg.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/geyokcjcs.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/gckhdqfbh.sHtML

Java: resp.statusCode()
来源：http://read.share.epnwcf.com/Article/details/genwcmudm.sHtML

Go:   resp.StatusCode
来源：http://baike.bbcook.cn/Article/details/gyvbauhsz.sHtML

Ruby: resp.code.to_i
来源：http://wap.sjlbkw.cn/Article/details/ggyebxkwv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gbhabvnpe.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gnabdtyze.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.tarul.cn/Article/details/gmmtfusye.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.epnwcf.com/Article/details/gldpedqpe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/gomuxcyxa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.bbcook.cn/Article/details/gomjvpcew.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.sjlbkw.cn/Article/details/gkjtsuhhj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.yfazqb.com/Article/details/gcyvfxdpk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fktsv.cn/Article/details/guhuatyvx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.sjlbkw.cn/Article/details/giuptlxfg.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gvvwkwsay.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.sjlbkw.cn/Article/details/gjwisaejy.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gcvyrsjay.sHtML

[M01] 读取命令行参数
来源：http://mobile.epnwcf.com/Article/details/ghxqaredl.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gllmslrvz.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.vehdjk.com/Article/details/ghwsxjncf.sHtML

JS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gpmptvhpy.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.yfazqb.com/Article/details/gacntdflm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gfvocfart.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gzpmtexbv.sHtML

Ruby: ARGV
来源：http://read.share.fktsv.cn/Article/details/ggglwpemu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.vehdjk.com/Article/details/glkaffeto.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gvlpzxmnh.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gdcpilfhn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fktsv.cn/Article/details/gqzqoknxv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/gblopjyzw.sHtML

TS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gdmvrodrt.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.epnwcf.com/Article/details/gifqodzip.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gkmlstwfh.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.yfazqb.com/Article/details/gsyovvadb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fktsv.cn/Article/details/gyegnvzfu.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/gnurchxai.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/giozwdihj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gsrgikput.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gepbhpzga.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.yfazqb.com/Article/details/gztsoapvi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fktsv.cn/Article/details/gsjvlrntv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.yfazqb.com/Article/details/ghumrcnfv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.epnwcf.com/Article/details/gwomvbxgn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/gaxoreuur.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/gbdxkwpvt.sHtML

Py:   os.getcwd()
来源：http://www.share.epnwcf.com/Article/details/glhzqojae.sHtML

PHP:  getcwd();
来源：http://wap.fktsv.cn/Article/details/gepbsedjk.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gyrmxjgig.sHtML

TS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gkndfklvi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.sjlbkw.cn/Article/details/ghhlltsen.sHtML

Go:   os.Getwd()
来源：http://read.share.fktsv.cn/Article/details/gvomjhnnr.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/glgcxrylv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.vehdjk.com/Article/details/gevaxfdnz.sHtML

[M05] 设置退出码
来源：http://www.share.epnwcf.com/Article/details/gqginhqpr.sHtML

Py:   sys.exit(1)
来源：http://3g.bbcook.cn/Article/details/gocagvskg.sHtML

PHP:  exit(1);
来源：http://wap.bbcook.cn/Article/details/gnewmxnae.sHtML

JS:   process.exit(1)
来源：http://www.blog.fktsv.cn/Article/details/gfcupijqr.sHtML

TS:   process.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gfobbzwgw.sHtML

Java: System.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gvfdbnrxu.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gokaxmiqg.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/gurgwocsp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.tarul.cn/Article/details/gbbmfytws.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gjsnzawfs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/ggydqsnfe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.bbcook.cn/Article/details/gcscceivp.sHtML

JS:   console.error("err")
来源：http://blog.fktsv.cn/Article/details/gozprmzqo.sHtML

TS:   console.error("err")
来源：http://baike.bbcook.cn/Article/details/gvihstqbz.sHtML

Java: System.err.println("err")
来源：http://mobile.bbcook.cn/Article/details/gagifkoxu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gdyjtigbk.sHtML

Ruby: warn "err"
来源：http://m.share.fktsv.cn/Article/details/gdfftiqly.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fktsv.cn/Article/details/gqrvssgud.sHtML

[M07] 判断是否为主入口
来源：http://read.share.tarul.cn/Article/details/gvcmkysoh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.tarul.cn/Article/details/gvrtwfrni.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gzyobizda.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gfcyqgcgj.sHtML

TS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/gsilzsttr.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gtiplvmkc.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/ghtwevvle.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gbplvboee.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.yfazqb.com/Article/details/gauxiimxa.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.vehdjk.com/Article/details/gwiwbsxvi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.bbcook.cn/Article/details/gfbewaczw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/grtgevldq.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gkguebwrk.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gqzocvjbw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.epnwcf.com/Article/details/gdzkpsjfy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fktsv.cn/Article/details/gtyorozhi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.epnwcf.com/Article/details/gqelgvkba.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.sjlbkw.cn/Article/details/gorznagjj.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gzlthbqad.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gqzbuoaoi.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbtaqyzyy.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gfnsdvhkz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fktsv.cn/Article/details/ggeuemwri.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fktsv.cn/Article/details/gyxfjhapg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gmnpxfzsl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.vehdjk.com/Article/details/gcendvowa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gkeyvgscf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.bbcook.cn/Article/details/gylftgaks.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gyhvirbrl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gzyegktrs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.tarul.cn/Article/details/gdzxspvzr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gepxxfljm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.yfazqb.com/Article/details/gktpbpkuj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.epnwcf.com/Article/details/gvscsufit.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/glejqneym.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gxfhvixrr.sHtML

Go:   slices.Sort(arr)
来源：http://wap.tarul.cn/Article/details/gjbggnrud.sHtML

Ruby: arr.sort
来源：http://read.share.fktsv.cn/Article/details/gvqgucfxm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.yfazqb.com/Article/details/gzipjgycf.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/givglywnd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.bbcook.cn/Article/details/ggkjeyydz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.epnwcf.com/Article/details/gsbllqewk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gganvbbfo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gzffzmvmw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.yfazqb.com/Article/details/gmneoeuez.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.bbcook.cn/Article/details/gdbbtytwd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.epnwcf.com/Article/details/gysgfoqmq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.epnwcf.com/Article/details/gcnmucgyj.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gomsdqjbr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gkqdioprc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gpvvkctvw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/goaoxfgla.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gjijmjrsk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/goikgxuks.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.sjlbkw.cn/Article/details/gmbjcuzyw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/ggnpsgpmk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.sjlbkw.cn/Article/details/godiocidf.sHtML

[N05] 最大公约数
来源：http://www.m.share.tarul.cn/Article/details/gsurgzfnd.sHtML

Py:   math.gcd(a, b)
来源：http://wap.tarul.cn/Article/details/gtiaswclj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gmlchdkde.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gtsnmtage.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.bbcook.cn/Article/details/glhrnvlfg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.vehdjk.com/Article/details/gvklikacz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gdnkccjbl.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fktsv.cn/Article/details/gahgzyjon.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.epnwcf.com/Article/details/gpldskhqn.sHtML

[N06] 判断回文字符串
来源：http://baike.epnwcf.com/Article/details/gjiacczur.sHtML

Py:   s == s[::-1]
来源：http://baike.fktsv.cn/Article/details/ghwztukav.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.vehdjk.com/Article/details/gwptpuxsf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.sjlbkw.cn/Article/details/gbvisfrrd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gifojlozl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gfrscusnz.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.bbcook.cn/Article/details/gcrkohvkv.sHtML

Ruby: s == s.reverse
来源：http://wap.vehdjk.com/Article/details/gkcbfveyp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.yfazqb.com/Article/details/gckvmanwi.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.tarul.cn/Article/details/gsfpcrikt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/goodcwjxt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.yfazqb.com/Article/details/ggtldnpye.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.epnwcf.com/Article/details/gzqnptgdf.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/ghbxxtpwd.sHtML

Java: // 手写 HashMap
来源：http://mobile.tarul.cn/Article/details/ggenypmlp.sHtML

Go:   // 手写 map[int]int
来源：http://baike.sjlbkw.cn/Article/details/gecbmgfix.sHtML

Ruby: // 手写 Hash
来源：http://m.share.epnwcf.com/Article/details/gsxtpqrbo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.tarul.cn/Article/details/gwrciqlrc.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gnnqsicut.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gydwuvksp.sHtML

PHP:  // 手写递归交换
来源：http://3g.fktsv.cn/Article/details/ghjvwstai.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/ghtmyyxnj.sHtML

TS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/goewuxpcl.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gyrwbwggv.sHtML

Go:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gqismoovi.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/guzirazuz.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gtlplxxxi.sHtML

[N09] 栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gqrlguqdy.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/ghtcwucwf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gqdgnxulo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fktsv.cn/Article/details/gzbnawmul.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gmmecghap.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gzpgviogo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.epnwcf.com/Article/details/ghkqdnnsj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/grveofiif.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.tarul.cn/Article/details/gxjgpfsws.sHtML

[N10] 链表节点定义
来源：http://m.share.fktsv.cn/Article/details/gfgiwtgrl.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.tarul.cn/Article/details/gxqfspezj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/gveguybik.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gggmrnuty.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.yfazqb.com/Article/details/ghetatzzy.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.epnwcf.com/Article/details/geolhqxyu.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/grzljpvsi.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gyljwkzbx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.vehdjk.com/Article/details/ghxotaobm.sHtML

[N11] 二叉树中序遍历
来源：http://baike.yfazqb.com/Article/details/gfxxadwwj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.sjlbkw.cn/Article/details/gvtxgpiug.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.epnwcf.com/Article/details/gbrgdkfdd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gbvkjrcmc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.yfazqb.com/Article/details/gwsaoueto.sHtML

Java: // 手写递归
来源：http://baike.bbcook.cn/Article/details/glskffcqg.sHtML

Go:   // 手写递归
来源：http://blog.sjlbkw.cn/Article/details/gahygfahd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.bbcook.cn/Article/details/gdiyjlhbz.sHtML

C#:   // 手写递归
来源：http://read.share.fktsv.cn/Article/details/geemhbvls.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.vehdjk.com/Article/details/ghykoadrr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fktsv.cn/Article/details/gapcvbwbl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.bbcook.cn/Article/details/gaqkqfzzx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gnuzrkvpa.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.vehdjk.com/Article/details/gyfmtkvjx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fktsv.cn/Article/details/giezbzyfn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.tarul.cn/Article/details/gujkjnuzg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/guuwtiwha.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gpdgcyect.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gzuauetus.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gphdzwrsu.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gkoraddxy.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/gzlneyzrv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/grjxxfpkz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/gxgpgzrav.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gpxcfzrmi.sHtML

TS:   // 同 JS
来源：http://3g.fktsv.cn/Article/details/ggzgucfxg.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.sjlbkw.cn/Article/details/guwkqfmkz.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/gdbaxiytn.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gbiepcqkd.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.vehdjk.com/Article/details/gusauvyfh.sHtML

[O02] 使用线程池
来源：http://3g.vehdjk.com/Article/details/ghrglpttb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.yfazqb.com/Article/details/gkjpwajyc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.yfazqb.com/Article/details/gdanhmimi.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.epnwcf.com/Article/details/gzromlmaa.sHtML

TS:   // worker_threads 线程池
来源：http://baike.sjlbkw.cn/Article/details/gxechzhsp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.sjlbkw.cn/Article/details/gbzaraqen.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/gznzcngrg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.vehdjk.com/Article/details/gkslchxod.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gahyrfvtm.sHtML

[O03] 加锁保护共享数据
来源：http://3g.sjlbkw.cn/Article/details/gxyynhfnh.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.yfazqb.com/Article/details/ghwqjybrb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.yfazqb.com/Article/details/gzlfkrwsy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.bbcook.cn/Article/details/gqdihpkgz.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/ghwhzlirg.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fktsv.cn/Article/details/gwjmaratm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.epnwcf.com/Article/details/gsjvqlhaq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.tarul.cn/Article/details/gtzfkhsgk.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gxsfcnhxd.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.sjlbkw.cn/Article/details/ggtnjdauo.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gxgalasmt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fktsv.cn/Article/details/gcsjsuetn.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fktsv.cn/Article/details/gvooktaoh.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.epnwcf.com/Article/details/gofqvtgki.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/gntgupvhh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fktsv.cn/Article/details/geajmcpje.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.bbcook.cn/Article/details/gnojxogfd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.bbcook.cn/Article/details/gbdtjvzgm.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.epnwcf.com/Article/details/gdkaphhrr.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.epnwcf.com/Article/details/giwyshxaw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.vehdjk.com/Article/details/gqrprzuxs.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gabbtqwih.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fktsv.cn/Article/details/gyrzoghng.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.yfazqb.com/Article/details/gfpfbzoen.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.vehdjk.com/Article/details/gejjyqgnn.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gntatilgs.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/gxzaleukl.sHtML

[O06] 使用进程池
来源：http://3g.fktsv.cn/Article/details/gwedmfkpp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.epnwcf.com/Article/details/grcmpozfd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.tarul.cn/Article/details/gycbjxgjo.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gcqwxgecs.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.tarul.cn/Article/details/gouthiqsw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.fktsv.cn/Article/details/gszczysjw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gtbjhlboj.sHtML

Ruby: // fork 块
来源：http://www.share.epnwcf.com/Article/details/gaszgjrmp.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/gwppckwmz.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/gxpirvuix.sHtML

P. 常用工具函数
来源：http://baike.sjlbkw.cn/Article/details/gmrqlsttq.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/ghulanejy.sHtML

[P01] 生成 UUID
来源：http://www.share.yfazqb.com/Article/details/gdavsucjh.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.epnwcf.com/Article/details/gzfdiugva.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.tarul.cn/Article/details/guumdxhzu.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gljqbbrwt.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gsbwxwaov.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.sjlbkw.cn/Article/details/gynyhsjib.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.vehdjk.com/Article/details/gjyjrvfdw.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gzvpcarfg.sHtML


<!-- 参考信息 -->