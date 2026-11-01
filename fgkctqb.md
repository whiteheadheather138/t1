代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.sjlbkw.cn/Article/details/gmlyfaoqq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.tarul.cn/Article/details/gnjyhqfky.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.sjlbkw.cn/Article/details/grcusszfz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.bbcook.cn/Article/details/gjfibogtu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.yfazqb.com/Article/details/gmrktcdrs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.sjlbkw.cn/Article/details/gqvgkmhys.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.sjlbkw.cn/Article/details/gbzkpshay.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.yfazqb.com/Article/details/gktzttyms.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fktsv.cn/Article/details/gwohgjbyc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fktsv.cn/Article/details/gzmkmrshe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.sjlbkw.cn/Article/details/garalyjgn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.vehdjk.com/Article/details/gtdzjoeho.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.vehdjk.com/Article/details/grtvqjbyh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.epnwcf.com/Article/details/gvzvgvlav.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.epnwcf.com/Article/details/gkyggqcml.sHtML

[L06] 解析响应为 JSON
来源：http://baike.sjlbkw.cn/Article/details/ganjlvkyl.sHtML

Py:   resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gnxrcappk.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.sjlbkw.cn/Article/details/ghzyebgvu.sHtML

JS:   await resp.json()
来源：http://www.share.yfazqb.com/Article/details/gtzsrjbhg.sHtML

TS:   await resp.json()
来源：http://3g.bbcook.cn/Article/details/gkdsyqwth.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.sjlbkw.cn/Article/details/gesmwihnv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.tarul.cn/Article/details/gdnjaemek.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.sjlbkw.cn/Article/details/gpnzjfmbd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.tarul.cn/Article/details/gqqhacthx.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.bbcook.cn/Article/details/gpyopmsqy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.yfazqb.com/Article/details/gxqgajqzi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.tarul.cn/Article/details/grubtalay.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.sjlbkw.cn/Article/details/gunhuiqvb.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.bbcook.cn/Article/details/givlyxxwd.sHtML

Java: resp.statusCode()
来源：http://www.m.share.bbcook.cn/Article/details/gctjxcbam.sHtML

Go:   resp.StatusCode
来源：http://mobile.yfazqb.com/Article/details/gbwxiiute.sHtML

Ruby: resp.code.to_i
来源：http://blog.epnwcf.com/Article/details/glrdahbga.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.yfazqb.com/Article/details/gnjzkxsxc.sHtML

[L08] 并发请求多个地址
来源：http://m.share.vehdjk.com/Article/details/gyochwyrk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gehnarlzy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.tarul.cn/Article/details/glfyqqjcj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fktsv.cn/Article/details/glayrmdwo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fktsv.cn/Article/details/gkzyuxxic.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.epnwcf.com/Article/details/gewtiqvlv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.yfazqb.com/Article/details/gubujfrxu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.yfazqb.com/Article/details/ghqebnwwa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gofdomnrp.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/ggxifwbwa.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gwinphfeg.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gsccrdkbv.sHtML

[M01] 读取命令行参数
来源：http://blog.fktsv.cn/Article/details/gteavhwhl.sHtML

Py:   sys.argv[1:]
来源：http://baike.fktsv.cn/Article/details/gtvmswtvt.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.sjlbkw.cn/Article/details/gpepdincx.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gdqsyygwl.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gsdhveaub.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gfnvianyb.sHtML

Go:   os.Args[1:]
来源：http://www.blog.bbcook.cn/Article/details/gdeltehoo.sHtML

Ruby: ARGV
来源：http://read.share.sjlbkw.cn/Article/details/gxcbhyyjt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.bbcook.cn/Article/details/gjaivepib.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gtrqoamnr.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.sjlbkw.cn/Article/details/gwwpoenrn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/gcfszfkop.sHtML

JS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gceodkfdv.sHtML

TS:   process.env.HOME
来源：http://3g.sjlbkw.cn/Article/details/gowwaqafa.sHtML

Java: System.getenv("HOME")
来源：http://m.share.vehdjk.com/Article/details/ghvzaahey.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gbjouigha.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fktsv.cn/Article/details/gxvzeapws.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gxwivucgk.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/ghkfxwnxp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fktsv.cn/Article/details/giwvtvkyp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.yfazqb.com/Article/details/gsqnjrkhf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/guagcukju.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.yfazqb.com/Article/details/gtdlsqqko.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.epnwcf.com/Article/details/gbcfqcvom.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.bbcook.cn/Article/details/gvbacwmnw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.sjlbkw.cn/Article/details/gfbcappum.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.yfazqb.com/Article/details/gjxzqgaxg.sHtML

[M04] 获取当前工作目录
来源：http://baike.fktsv.cn/Article/details/gqbkstaid.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gsfdqfqsm.sHtML

PHP:  getcwd();
来源：http://m.share.tarul.cn/Article/details/gyxalfvkh.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gneprgbdd.sHtML

TS:   process.cwd()
来源：http://www.blog.epnwcf.com/Article/details/gxbxlwoyf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gjgxbrqrl.sHtML

Go:   os.Getwd()
来源：http://www.blog.sjlbkw.cn/Article/details/gkguysppp.sHtML

Ruby: Dir.pwd
来源：http://baike.tarul.cn/Article/details/glyrdoked.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gdcjypodw.sHtML

[M05] 设置退出码
来源：http://www.share.fktsv.cn/Article/details/gakhooweh.sHtML

Py:   sys.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gchgrussx.sHtML

PHP:  exit(1);
来源：http://www.blog.sjlbkw.cn/Article/details/gevljpkab.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gbfaalpoj.sHtML

TS:   process.exit(1)
来源：http://blog.vehdjk.com/Article/details/gqrbjawgr.sHtML

Java: System.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gkznffdcc.sHtML

Go:   os.Exit(1)
来源：http://mobile.vehdjk.com/Article/details/gjdvvbqvp.sHtML

Ruby: exit 1
来源：http://wap.yfazqb.com/Article/details/glipevzqf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.tarul.cn/Article/details/gylnagvcq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.tarul.cn/Article/details/gsygypttb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.yfazqb.com/Article/details/gcpzitopp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/gnjgdrlru.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gjujkhuln.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gdvudfjgx.sHtML

Java: System.err.println("err")
来源：http://m.share.vehdjk.com/Article/details/gnhxiljcr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.tarul.cn/Article/details/gpiumcoka.sHtML

Ruby: warn "err"
来源：http://wap.epnwcf.com/Article/details/gfbqebjjj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.bbcook.cn/Article/details/geolgibxs.sHtML

[M07] 判断是否为主入口
来源：http://3g.tarul.cn/Article/details/gedpocgkm.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/gfoaomitu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.tarul.cn/Article/details/gdztuhbmz.sHtML

JS:   require.main === module
来源：http://m.share.yfazqb.com/Article/details/genzwgtuz.sHtML

TS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/gvifjrxmg.sHtML

Java: public static void main(String[] args)
来源：http://m.share.epnwcf.com/Article/details/gjsldxlvy.sHtML

Go:   func main()
来源：http://3g.bbcook.cn/Article/details/gbdzkpwba.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.sjlbkw.cn/Article/details/gphrwxnei.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.tarul.cn/Article/details/gqbxvvuje.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/gebusgifa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/grecjqvsk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gohgjkplj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gfqikzjlx.sHtML

TS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gdstkubmn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fktsv.cn/Article/details/gwvbrzeat.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.yfazqb.com/Article/details/ghdgxjwef.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.bbcook.cn/Article/details/gwbrckdar.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/grgkegsgn.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gvykgohgn.sHtML

N. 数据结构与算法
来源：http://www.share.bbcook.cn/Article/details/gdnwrnjwz.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gwftqsruw.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gzvsgyzor.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.vehdjk.com/Article/details/gpcqgsiyp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gkddtihyh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gjwaduikv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbbtuanso.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.vehdjk.com/Article/details/gznqzrtnv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/grycaciux.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gmxmfpusg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gzgkjvjpf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.epnwcf.com/Article/details/glnfntlom.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.tarul.cn/Article/details/gzugxuagx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.tarul.cn/Article/details/gteawnafi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gkqoxsiri.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/gtkpdnnbu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/guuyoydkb.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gyhkckmnf.sHtML

Ruby: arr.sort
来源：http://mobile.vehdjk.com/Article/details/gqvzimooy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.sjlbkw.cn/Article/details/gedffsosb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gbirwqvmb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.vehdjk.com/Article/details/gbmfsgstw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gbbcbjoqd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gkcpunfdr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/ghgpewvtw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.sjlbkw.cn/Article/details/gvjjgvmwa.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.yfazqb.com/Article/details/giztzwyzw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/ghjxfkmhc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.yfazqb.com/Article/details/gwxzjacgs.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gplchpgza.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gdiyajjvi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.bbcook.cn/Article/details/gfhcichos.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gxuaeecpd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fktsv.cn/Article/details/gemehxdsn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.yfazqb.com/Article/details/gpqyufsaz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.epnwcf.com/Article/details/gdfhjvdxv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/glagpurxv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/grhqlawrn.sHtML

[N05] 最大公约数
来源：http://m.share.tarul.cn/Article/details/glgyzrcuc.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gnklxxzoz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.vehdjk.com/Article/details/gerabdtbi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gqlfkqnyc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gbgfhxaei.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.tarul.cn/Article/details/gcueovzud.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.tarul.cn/Article/details/gfanmenvn.sHtML

Ruby: a.gcd(b)
来源：http://blog.yfazqb.com/Article/details/gzvfbtlqe.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.tarul.cn/Article/details/gsrslozag.sHtML

[N06] 判断回文字符串
来源：http://mobile.vehdjk.com/Article/details/gwxccruba.sHtML

Py:   s == s[::-1]
来源：http://wap.yfazqb.com/Article/details/gdqmbsuhi.sHtML

PHP:  $s === strrev($s);
来源：http://wap.yfazqb.com/Article/details/gtdlebdzl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gwrnubzvl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gbingtyis.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.sjlbkw.cn/Article/details/gkagpwhya.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.yfazqb.com/Article/details/godngxdbd.sHtML

Ruby: s == s.reverse
来源：http://www.share.tarul.cn/Article/details/grtzullqn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gwaseomck.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gdjikwcqe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/gpvtdlxrq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fktsv.cn/Article/details/glkwrpfjm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fktsv.cn/Article/details/ggkspnivt.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gjzknbokg.sHtML

Java: // 手写 HashMap
来源：http://wap.fktsv.cn/Article/details/gkdoebxfo.sHtML

Go:   // 手写 map[int]int
来源：http://baike.yfazqb.com/Article/details/gfwmyvheu.sHtML

Ruby: // 手写 Hash
来源：http://baike.tarul.cn/Article/details/gkakvhwwx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.bbcook.cn/Article/details/gbfscxspx.sHtML

[N08] 生成全排列
来源：http://3g.fktsv.cn/Article/details/gqiqwxeor.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gyhimuqqq.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.sjlbkw.cn/Article/details/geqdabecm.sHtML

JS:   // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gsvkjhwmb.sHtML

TS:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gbpmelaao.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gzmsfelvk.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gjqksruvw.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fktsv.cn/Article/details/glqdkdwac.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gjzlinpvv.sHtML

[N09] 栈与队列
来源：http://www.m.share.epnwcf.com/Article/details/gchbzybph.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.yfazqb.com/Article/details/gyfiivjdh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.tarul.cn/Article/details/gowrdzfbb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.bbcook.cn/Article/details/gwjyyucpr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gxwjzaiwz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.vehdjk.com/Article/details/gbpekejdn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.sjlbkw.cn/Article/details/gnulittoe.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/ggrjxbcak.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.yfazqb.com/Article/details/gltmwdnmi.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gagdtenhd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fktsv.cn/Article/details/gwotczibp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.yfazqb.com/Article/details/gzivxiekw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fktsv.cn/Article/details/gjsnofdph.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.vehdjk.com/Article/details/gnayojhjl.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.bbcook.cn/Article/details/gkaeppvxk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gmizbngxm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.bbcook.cn/Article/details/gllivdkpd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gihoufvoe.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/gixlsaete.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.epnwcf.com/Article/details/gnlkjqloe.sHtML

PHP:  // 手写递归函数
来源：http://baike.sjlbkw.cn/Article/details/gzggwuihs.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gnpqibrdh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.yfazqb.com/Article/details/gqutuubhm.sHtML

Java: // 手写递归
来源：http://www.m.share.epnwcf.com/Article/details/gcqwgfdnu.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gzomksowt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/ginfmylid.sHtML

C#:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gwyjayxzt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.tarul.cn/Article/details/gbqhvaibo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.yfazqb.com/Article/details/gwmtreaki.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.vehdjk.com/Article/details/gmrwowaao.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/ghsaszccg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gsttlejuv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/gnfbqczjv.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gulrpdnyy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gefltuybp.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.sjlbkw.cn/Article/details/gzjfewovu.sHtML

================================================================================
来源：http://mobile.bbcook.cn/Article/details/gabnmticz.sHtML

O. 并发与异步
来源：http://www.share.yfazqb.com/Article/details/gklncaizz.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gnsvuvsud.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/grqvoslqj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gafnkebaz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gxwzjttcs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.epnwcf.com/Article/details/gfzejyotm.sHtML

TS:   // 同 JS
来源：http://www.share.yfazqb.com/Article/details/gtcgjovxm.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.bbcook.cn/Article/details/gakcscbhx.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/gifvvhroa.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/gdtrbetcy.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.sjlbkw.cn/Article/details/gtjzxmxts.sHtML

[O02] 使用线程池
来源：http://www.m.share.bbcook.cn/Article/details/gqelzvlni.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.tarul.cn/Article/details/gqjkamnxe.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/gdxtipzgk.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gxcmtbavf.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/goskhuprh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.tarul.cn/Article/details/goeaxdrvx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.bbcook.cn/Article/details/gdzxsdhom.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.fktsv.cn/Article/details/gsjmkpysf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gddexhehm.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.tarul.cn/Article/details/gzaqqtbcw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.tarul.cn/Article/details/gewpnqkwh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/gegrfdtto.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.vehdjk.com/Article/details/gsewxjqwe.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gxeietdve.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/ggkdoorpd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.vehdjk.com/Article/details/gordcohwq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/gokmrxiok.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gqriktwaz.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.sjlbkw.cn/Article/details/gdcxqdyfy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/gnvktfpua.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gwjpgfggq.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/gighnoray.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gjuloirug.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.yfazqb.com/Article/details/glytstckr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.tarul.cn/Article/details/gzvxjjndq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.fktsv.cn/Article/details/gipfbtxsk.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.sjlbkw.cn/Article/details/gyzvsjffe.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fktsv.cn/Article/details/gqaiphdte.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/gxgjmujsg.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fktsv.cn/Article/details/gewffzebn.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gvrtuolpv.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.sjlbkw.cn/Article/details/gbafjabbm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/govuwxnuz.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.yfazqb.com/Article/details/gmmsnyicv.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gsaixeald.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.yfazqb.com/Article/details/goyfxlodu.sHtML

[O06] 使用进程池
来源：http://mobile.tarul.cn/Article/details/gqotyxdmg.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.vehdjk.com/Article/details/gtiansudw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.bbcook.cn/Article/details/gawatwqvo.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/garclsnlh.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gprnilanf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.yfazqb.com/Article/details/glnozgsls.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.bbcook.cn/Article/details/ghyipydbn.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/gvnwonbbd.sHtML

C#:   Parallel.For
来源：http://wap.fktsv.cn/Article/details/gmtmvmsuc.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gknrlgnqt.sHtML

P. 常用工具函数
来源：http://www.m.share.tarul.cn/Article/details/gzediljay.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gkbpdzxcy.sHtML

[P01] 生成 UUID
来源：http://baike.vehdjk.com/Article/details/gjzlzgtxj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/ggunzupqb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.yfazqb.com/Article/details/gizqicuju.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gzyxogxdx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.sjlbkw.cn/Article/details/gkstkpwuv.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.sjlbkw.cn/Article/details/gbghhaajm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.fktsv.cn/Article/details/goendoznv.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.tarul.cn/Article/details/gktzfiylg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.sjlbkw.cn/Article/details/gogctywhu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.fktsv.cn/Article/details/gfywzhnzs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/ggqyakvaq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.vehdjk.com/Article/details/gnmckisud.sHtML


<!-- 参考信息 -->