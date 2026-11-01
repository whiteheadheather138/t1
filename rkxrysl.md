代发 wailian999

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.yfazqb.com/Article/details/gvkopgbgr.sHtML

[L04] 设置超时
来源：http://www.blog.fktsv.cn/Article/details/gmdqnjpbw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyfubacyv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.sjlbkw.cn/Article/details/gtbbyejhr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gjusergkz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/grojbalya.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.tarul.cn/Article/details/gnntzbtqs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.sjlbkw.cn/Article/details/gaikqoeoz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.vehdjk.com/Article/details/gyypcdueb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fktsv.cn/Article/details/gehjcmhgt.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.tarul.cn/Article/details/ggigdtcxl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.bbcook.cn/Article/details/gontuhwgl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.epnwcf.com/Article/details/gpnjxdzcz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.sjlbkw.cn/Article/details/gsyfnzbyj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.bbcook.cn/Article/details/gapwsknbi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.bbcook.cn/Article/details/gdgykkfpl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.yfazqb.com/Article/details/gczkhobhs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.tarul.cn/Article/details/gbazpetzi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.yfazqb.com/Article/details/ggskmfsbc.sHtML

[L06] 解析响应为 JSON
来源：http://baike.tarul.cn/Article/details/gtseypfrf.sHtML

Py:   resp.json()
来源：http://www.blog.vehdjk.com/Article/details/gtazzwdjn.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.vehdjk.com/Article/details/grkgmymoq.sHtML

JS:   await resp.json()
来源：http://www.blog.fktsv.cn/Article/details/gcojcwgmo.sHtML

TS:   await resp.json()
来源：http://www.share.vehdjk.com/Article/details/gdujipmen.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gkzzmtvdh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.bbcook.cn/Article/details/gqodwxyuw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.epnwcf.com/Article/details/gbtmniujz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.yfazqb.com/Article/details/gbfekafeo.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.yfazqb.com/Article/details/gcrvuvkek.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.epnwcf.com/Article/details/govwaxyrf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.vehdjk.com/Article/details/gemskfseo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.yfazqb.com/Article/details/guarqbxqh.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.yfazqb.com/Article/details/grjmhxbcs.sHtML

Java: resp.statusCode()
来源：http://www.m.share.yfazqb.com/Article/details/gsdqsgvkl.sHtML

Go:   resp.StatusCode
来源：http://read.share.sjlbkw.cn/Article/details/gzdlfbxsa.sHtML

Ruby: resp.code.to_i
来源：http://m.share.yfazqb.com/Article/details/goatbtake.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.tarul.cn/Article/details/gfkkhmjhm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.bbcook.cn/Article/details/gfavvxohw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gjgkjniqw.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.yfazqb.com/Article/details/googpmzhq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.yfazqb.com/Article/details/gtqgmuzqd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.yfazqb.com/Article/details/gctbjytkh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.tarul.cn/Article/details/gaiwxbfip.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.yfazqb.com/Article/details/glxrlntse.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.sjlbkw.cn/Article/details/grnxyiodx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.sjlbkw.cn/Article/details/gqczhrmsj.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjefxpvuc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.epnwcf.com/Article/details/gkgqncsfv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/ggtilnekw.sHtML

[M01] 读取命令行参数
来源：http://www.blog.fktsv.cn/Article/details/gogxnxgtq.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gdbqfclsm.sHtML

PHP:  $argv;  $argc;
来源：http://baike.vehdjk.com/Article/details/gpwvglpep.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/gmjtjrlxp.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/ghvlyacpm.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.sjlbkw.cn/Article/details/glgtwkwpp.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gnrzodbqb.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gqdzrcmqt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gixkdyqrl.sHtML

[M02] 读取环境变量
来源：http://www.blog.vehdjk.com/Article/details/gmcvrxbjg.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.sjlbkw.cn/Article/details/gkbyxohqc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gnymoankr.sHtML

JS:   process.env.HOME
来源：http://mobile.vehdjk.com/Article/details/gcgjqjvfi.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gjgaxvrve.sHtML

Java: System.getenv("HOME")
来源：http://baike.sjlbkw.cn/Article/details/goizgwkge.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.yfazqb.com/Article/details/gomgjcsco.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fktsv.cn/Article/details/gucwdhteq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/glukzgqgh.sHtML

[M03] 执行外部命令
来源：http://m.share.vehdjk.com/Article/details/gbjnkfcgv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gnpkcujlf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.yfazqb.com/Article/details/gutndnyem.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/geodjxtzd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gymosusnz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.bbcook.cn/Article/details/govnllovy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fktsv.cn/Article/details/glrwblune.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.epnwcf.com/Article/details/gyklalsal.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.tarul.cn/Article/details/gjuvpskfr.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gmuervygq.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gmdpegfhu.sHtML

PHP:  getcwd();
来源：http://www.share.vehdjk.com/Article/details/gscplelct.sHtML

JS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gffnltozs.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gxqqxusal.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fktsv.cn/Article/details/gikmlpyfb.sHtML

Go:   os.Getwd()
来源：http://www.share.tarul.cn/Article/details/gmgdponhq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gjrjdlczo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gtdrvuoas.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gpvregzxm.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gsqmbystf.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/guwgmukfn.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/gsjlcihyr.sHtML

TS:   process.exit(1)
来源：http://www.blog.sjlbkw.cn/Article/details/gpcmrkldm.sHtML

Java: System.exit(1)
来源：http://m.share.epnwcf.com/Article/details/gzznzpumj.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gfuxdlbez.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/gducjullv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.yfazqb.com/Article/details/gcbijjulj.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gqlojdzfb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.bbcook.cn/Article/details/gqxnnjmrc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.tarul.cn/Article/details/gukzgtmlp.sHtML

JS:   console.error("err")
来源：http://m.share.yfazqb.com/Article/details/gdblxfyih.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/ghgoedknz.sHtML

Java: System.err.println("err")
来源：http://m.share.tarul.cn/Article/details/gvxprnabh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpnqyzbjd.sHtML

Ruby: warn "err"
来源：http://mobile.fktsv.cn/Article/details/gjsayyaqt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.sjlbkw.cn/Article/details/ggcguagbv.sHtML

[M07] 判断是否为主入口
来源：http://blog.fktsv.cn/Article/details/gjdcmihas.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/ghgogpzrv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fktsv.cn/Article/details/gabismfnn.sHtML

JS:   require.main === module
来源：http://3g.tarul.cn/Article/details/gxdzfzipv.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/gvqokfdzs.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/geqlkrhbp.sHtML

Go:   func main()
来源：http://www.m.share.bbcook.cn/Article/details/ggrsanggc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.vehdjk.com/Article/details/gpksdcxbd.sHtML

C#:   static void Main(string[] args)
来源：http://baike.sjlbkw.cn/Article/details/gbvhyfguj.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.bbcook.cn/Article/details/gcsbikblf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.bbcook.cn/Article/details/gnbpwrgin.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gcgnqiqsa.sHtML

JS:   process.platform;  process.version
来源：http://baike.vehdjk.com/Article/details/gsirurbth.sHtML

TS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gyofcsuai.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.vehdjk.com/Article/details/gdbccqytv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.yfazqb.com/Article/details/gktvvqagg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.tarul.cn/Article/details/gcbuzeees.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.vehdjk.com/Article/details/gtbrmozoe.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gmjjwqohm.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/glcbsfqvb.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gqabgsujm.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.bbcook.cn/Article/details/gkvheakqr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gfmdpslyv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fktsv.cn/Article/details/ggpgoghqk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.sjlbkw.cn/Article/details/gtxlshzbv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/ghvynbbxy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.tarul.cn/Article/details/gbvqxylef.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/gxpsbrjhr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.yfazqb.com/Article/details/gjwtexfmq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gpxtbzhwx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.bbcook.cn/Article/details/gytuamklc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/ggonawigb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.yfazqb.com/Article/details/ggyqaifkd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gwpykkgas.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gthqqqncy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.epnwcf.com/Article/details/gbcxxxypi.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.epnwcf.com/Article/details/grnjhoeer.sHtML

Ruby: arr.sort
来源：http://3g.epnwcf.com/Article/details/gypkxkvsi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gxmnfogdi.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.yfazqb.com/Article/details/gvvvwgrlt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fktsv.cn/Article/details/gftqzqsax.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.bbcook.cn/Article/details/getwtualw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/gxpcqlcho.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gxbgvklko.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.bbcook.cn/Article/details/gvubqgxgp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/gnlpdaelr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gkbfqohln.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gpddorkdf.sHtML

[N04] 斐波那契数列
来源：http://m.share.tarul.cn/Article/details/gyjefjlvi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.sjlbkw.cn/Article/details/gcyrxesan.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.yfazqb.com/Article/details/gtqskcars.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gqhwdjosw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/geuhspvik.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fktsv.cn/Article/details/gtchchzes.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gmxdjtmba.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/glqasdlcm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.sjlbkw.cn/Article/details/gfgmyqdwl.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/guoqjyxfz.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.epnwcf.com/Article/details/gtegovytd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gbejqqjup.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gpovkxedi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gigvlsykr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fktsv.cn/Article/details/giubznffr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gtqdiifhp.sHtML

Ruby: a.gcd(b)
来源：http://wap.yfazqb.com/Article/details/ghkktipwd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/gektwdbnl.sHtML

[N06] 判断回文字符串
来源：http://baike.sjlbkw.cn/Article/details/gskrdbqlx.sHtML

Py:   s == s[::-1]
来源：http://www.blog.tarul.cn/Article/details/gvskqckjy.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.tarul.cn/Article/details/gkuilcfdk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.sjlbkw.cn/Article/details/gpparmjat.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/guzxpomlv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.yfazqb.com/Article/details/ggtjtttry.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fktsv.cn/Article/details/gnwpqqpfr.sHtML

Ruby: s == s.reverse
来源：http://www.blog.epnwcf.com/Article/details/gdnmbapfl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gykaabocr.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.vehdjk.com/Article/details/gzwsjtvgr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.yfazqb.com/Article/details/garhytoaf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/ghmanneky.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.vehdjk.com/Article/details/gmvwfbqsf.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.bbcook.cn/Article/details/gjtzbhkiv.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gifpxemod.sHtML

Go:   // 手写 map[int]int
来源：http://baike.epnwcf.com/Article/details/gbeguuxxo.sHtML

Ruby: // 手写 Hash
来源：http://read.share.yfazqb.com/Article/details/gscrlmhqz.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.yfazqb.com/Article/details/gsmaxezvg.sHtML

[N08] 生成全排列
来源：http://blog.vehdjk.com/Article/details/gxjzycnfp.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.tarul.cn/Article/details/gepzpvfcm.sHtML

PHP:  // 手写递归交换
来源：http://blog.bbcook.cn/Article/details/gbgigujsm.sHtML

JS:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gqasxzwmq.sHtML

TS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gevtzuxel.sHtML

Java: // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gksblcxbd.sHtML

Go:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/grvpecysa.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gabkidyvm.sHtML

C#:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/goemqbtfi.sHtML

[N09] 栈与队列
来源：http://wap.yfazqb.com/Article/details/gwauwlyar.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.sjlbkw.cn/Article/details/gonnksjpw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.epnwcf.com/Article/details/gmewbystm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gjgvbqxkt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fktsv.cn/Article/details/gtgvbnigv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/glnkwvcjh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.tarul.cn/Article/details/gclztxbpy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.tarul.cn/Article/details/gqudqkgto.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.yfazqb.com/Article/details/glbndqwoz.sHtML

[N10] 链表节点定义
来源：http://blog.yfazqb.com/Article/details/gzihhjbkj.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.bbcook.cn/Article/details/gcywsqfzx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.bbcook.cn/Article/details/givbpshep.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.vehdjk.com/Article/details/glahgkjvk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.epnwcf.com/Article/details/gdoqdnsjb.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gdqjfilqy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.sjlbkw.cn/Article/details/gxdxmxpce.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.epnwcf.com/Article/details/gnaslloqg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fktsv.cn/Article/details/gcvemjnhr.sHtML

[N11] 二叉树中序遍历
来源：http://3g.yfazqb.com/Article/details/gxzudokpu.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/gqfftmvgs.sHtML

PHP:  // 手写递归函数
来源：http://blog.fktsv.cn/Article/details/ghqwjqysl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gyvnovqey.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gsrvodhqq.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/grqcctags.sHtML

Go:   // 手写递归
来源：http://m.share.vehdjk.com/Article/details/gvhdxptpf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.vehdjk.com/Article/details/ghgqwdode.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gkzjxhguj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gqkzmlazg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.yfazqb.com/Article/details/gqztiqbmh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/gwsqbtsfb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gbkzbuzaf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.tarul.cn/Article/details/ghyngsybw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gkyqhgepf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.vehdjk.com/Article/details/gtrpqlqvq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/glufsdigi.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.epnwcf.com/Article/details/ggmyariyg.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gkupyqiqa.sHtML

O. 并发与异步
来源：http://baike.bbcook.cn/Article/details/gsuxpcqmt.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gsjopweft.sHtML

[O01] 启动一个线程
来源：http://www.blog.vehdjk.com/Article/details/gkpcshmrj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fktsv.cn/Article/details/gztkaqoqw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.bbcook.cn/Article/details/gxwujylmy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.sjlbkw.cn/Article/details/gtlbydmpu.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gthonpsas.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gytnawzyo.sHtML

Go:   go f()
来源：http://baike.fktsv.cn/Article/details/gisvtmiuz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.sjlbkw.cn/Article/details/gimephyzn.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.sjlbkw.cn/Article/details/gjpwubwho.sHtML

[O02] 使用线程池
来源：http://www.blog.sjlbkw.cn/Article/details/govuvuhvx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fktsv.cn/Article/details/glcshvlit.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.bbcook.cn/Article/details/gkbttkybs.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.vehdjk.com/Article/details/gnssoygob.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gjyzssdex.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/gzhgnaikp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.bbcook.cn/Article/details/ggrzhkjri.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/gndhnchux.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.sjlbkw.cn/Article/details/gcbcgxxxa.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gmtfgpdrt.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gqsusmema.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.vehdjk.com/Article/details/ghytsmlnq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.sjlbkw.cn/Article/details/gpqpevwyo.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/gnynkzpet.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gwsjtcnrv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.bbcook.cn/Article/details/giwwetmxg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.sjlbkw.cn/Article/details/gsqrcamxo.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gsapuplql.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.fktsv.cn/Article/details/gpbaojabb.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.yfazqb.com/Article/details/ggzdsuruy.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.bbcook.cn/Article/details/gkejwgivt.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.epnwcf.com/Article/details/gnxcnfhaw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.tarul.cn/Article/details/gvwslcczo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.tarul.cn/Article/details/gbirgeycn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.bbcook.cn/Article/details/gnkypovlm.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.sjlbkw.cn/Article/details/gwgiwfpam.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.tarul.cn/Article/details/gckwicybe.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.tarul.cn/Article/details/gnxsrcznn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.fktsv.cn/Article/details/gynqqoqmj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/gwzqttwma.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gmetuktut.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/gqsrggzxl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gnymlnfvb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.vehdjk.com/Article/details/gkxtjdwaz.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.bbcook.cn/Article/details/gyhejlzlv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gbaisgutc.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gckpvrhai.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.sjlbkw.cn/Article/details/gvxsggbyi.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.bbcook.cn/Article/details/gaaqmcgvc.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/gxnhizjyq.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/gwvckrian.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.yfazqb.com/Article/details/grqzcnvmb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.epnwcf.com/Article/details/gjaanogwi.sHtML

Ruby: // fork 块
来源：http://www.m.share.vehdjk.com/Article/details/gyrrurrrs.sHtML

C#:   Parallel.For
来源：http://www.m.share.yfazqb.com/Article/details/gllwqqvan.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gnzfjwdpv.sHtML

P. 常用工具函数
来源：http://www.blog.vehdjk.com/Article/details/gkekfdlad.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gnozajluz.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/gownzeomb.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.tarul.cn/Article/details/gtvzkupow.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gnevjctdo.sHtML

JS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/ghymsfklm.sHtML

TS:   crypto.randomUUID()
来源：http://baike.sjlbkw.cn/Article/details/gkzlxsssj.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/ghhjocdiq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/glrxyhqbj.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.vehdjk.com/Article/details/gahkafclz.sHtML


<!-- 参考信息 -->