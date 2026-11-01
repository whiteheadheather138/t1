代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.bbcook.cn/Article/details/gbguxrrry.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/gglsmxwyr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.sjlbkw.cn/Article/details/ggndkuenq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.sjlbkw.cn/Article/details/gpyuowecv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.vehdjk.com/Article/details/gihfzsaib.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.bbcook.cn/Article/details/gnsodguds.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fktsv.cn/Article/details/gjhranpwv.sHtML

[L06] 解析响应为 JSON
来源：http://blog.yfazqb.com/Article/details/giilkfvoq.sHtML

Py:   resp.json()
来源：http://blog.yfazqb.com/Article/details/gaitjuwhv.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.vehdjk.com/Article/details/gfgphdliq.sHtML

JS:   await resp.json()
来源：http://baike.fktsv.cn/Article/details/giuxlzpoa.sHtML

TS:   await resp.json()
来源：http://www.share.epnwcf.com/Article/details/gqzgvwgky.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.yfazqb.com/Article/details/gsyacwfdn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.tarul.cn/Article/details/gkqexuzgb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.sjlbkw.cn/Article/details/grxchzafv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.tarul.cn/Article/details/garfzjqzq.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.sjlbkw.cn/Article/details/gnxspqtlh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.yfazqb.com/Article/details/gvydofklk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fktsv.cn/Article/details/ghdncxsuz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gwhcpuphe.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.sjlbkw.cn/Article/details/gvxhxfgar.sHtML

Java: resp.statusCode()
来源：http://blog.sjlbkw.cn/Article/details/gcyficlon.sHtML

Go:   resp.StatusCode
来源：http://m.share.vehdjk.com/Article/details/goykmrblx.sHtML

Ruby: resp.code.to_i
来源：http://m.share.sjlbkw.cn/Article/details/gpyeqbvws.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fktsv.cn/Article/details/grujzvvhh.sHtML

[L08] 并发请求多个地址
来源：http://3g.yfazqb.com/Article/details/gzqskklek.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.yfazqb.com/Article/details/gavldufte.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.sjlbkw.cn/Article/details/gesuiqkcq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gxycjwufe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.tarul.cn/Article/details/gwuhbfyyd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.epnwcf.com/Article/details/goymrdwoq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.sjlbkw.cn/Article/details/gggiywgjg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.tarul.cn/Article/details/gzqrjfaqi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fktsv.cn/Article/details/gzagiefev.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gfqolkhvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gxvndfgud.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gfylrrwqx.sHtML

[M01] 读取命令行参数
来源：http://baike.yfazqb.com/Article/details/ghfffbgos.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/gtxpmqvhq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fktsv.cn/Article/details/guntamtkc.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.sjlbkw.cn/Article/details/gwsqrrqpm.sHtML

TS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/gveolfvtz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/gtlrponlz.sHtML

Go:   os.Args[1:]
来源：http://m.share.epnwcf.com/Article/details/gmunmcsol.sHtML

Ruby: ARGV
来源：http://www.blog.epnwcf.com/Article/details/gytliwskm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.epnwcf.com/Article/details/ghmigolra.sHtML

[M02] 读取环境变量
来源：http://m.share.fktsv.cn/Article/details/glaftlzqt.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gcsvujcdf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.sjlbkw.cn/Article/details/ggvoikriq.sHtML

JS:   process.env.HOME
来源：http://mobile.fktsv.cn/Article/details/gaovtteyc.sHtML

TS:   process.env.HOME
来源：http://3g.fktsv.cn/Article/details/ggnjchedc.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gjljrjgvn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gflmwhabp.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gtrkizmot.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gpoyqliaz.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gnttfbvul.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.vehdjk.com/Article/details/gzhprkrcp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.epnwcf.com/Article/details/gtdyxkidw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gggmisnnj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/gptkeshyg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/glxngtibu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.sjlbkw.cn/Article/details/gwlvcchbd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.sjlbkw.cn/Article/details/ghdpagmdw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/giqsbbtvs.sHtML

[M04] 获取当前工作目录
来源：http://baike.vehdjk.com/Article/details/ggevnbaob.sHtML

Py:   os.getcwd()
来源：http://mobile.vehdjk.com/Article/details/gmxiofotp.sHtML

PHP:  getcwd();
来源：http://m.share.vehdjk.com/Article/details/gwxumvexp.sHtML

JS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gewwjoxnl.sHtML

TS:   process.cwd()
来源：http://m.share.epnwcf.com/Article/details/gphompigk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.sjlbkw.cn/Article/details/gjopboyga.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/ghbfbydpj.sHtML

Ruby: Dir.pwd
来源：http://mobile.yfazqb.com/Article/details/gaugeuvmt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gxtqvsbbo.sHtML

[M05] 设置退出码
来源：http://mobile.fktsv.cn/Article/details/gxdjkqhuf.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gdowwrblm.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gokwgmqtu.sHtML

JS:   process.exit(1)
来源：http://read.share.fktsv.cn/Article/details/gpshjvhrp.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gfxhqakwp.sHtML

Java: System.exit(1)
来源：http://read.share.tarul.cn/Article/details/gzepsrihd.sHtML

Go:   os.Exit(1)
来源：http://3g.yfazqb.com/Article/details/gfgbuhezv.sHtML

Ruby: exit 1
来源：http://www.share.vehdjk.com/Article/details/ghjhsklpu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.yfazqb.com/Article/details/gvufvvtru.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gsrohfxmy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.yfazqb.com/Article/details/gqvposupc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/gxihudtce.sHtML

JS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gavcnzmsv.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gijckitsp.sHtML

Java: System.err.println("err")
来源：http://www.blog.bbcook.cn/Article/details/gwnkxtqqz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/ggcllcdkg.sHtML

Ruby: warn "err"
来源：http://www.m.share.epnwcf.com/Article/details/glwvvqrqm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.tarul.cn/Article/details/gmmodkugw.sHtML

[M07] 判断是否为主入口
来源：http://baike.fktsv.cn/Article/details/gtfdvulpr.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.yfazqb.com/Article/details/gjjcwdrmp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fktsv.cn/Article/details/gksbxwfan.sHtML

JS:   require.main === module
来源：http://blog.yfazqb.com/Article/details/giofeewim.sHtML

TS:   require.main === module
来源：http://www.share.sjlbkw.cn/Article/details/gcngqlout.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gadrcesdp.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/guiaqcpdx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fktsv.cn/Article/details/glsazfkto.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gyxetquvt.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.bbcook.cn/Article/details/gbvlcgyhx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.vehdjk.com/Article/details/gbygjieka.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fktsv.cn/Article/details/gwmtdyvib.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gihkmxzcr.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gxqpiqreq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.tarul.cn/Article/details/gkqhckoax.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.bbcook.cn/Article/details/gzvmpakxk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gspbcegkb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.vehdjk.com/Article/details/gobuktstf.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gkyfpbtwh.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gpeolwbxy.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/gcyrhdzjb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.sjlbkw.cn/Article/details/gpjaikxsc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/glgbbejhj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fktsv.cn/Article/details/gexpztbss.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gtdjrkrfv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/ggqwnayar.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.bbcook.cn/Article/details/gfpdvfsud.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gcouuoyos.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.bbcook.cn/Article/details/gjvspzoxi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gclpfafge.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gxkdaalxo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gydxzcfgb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.fktsv.cn/Article/details/gvparnhzt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gkzctetxw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/ggghzfbrb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gxpstgvfa.sHtML

Go:   slices.Sort(arr)
来源：http://3g.vehdjk.com/Article/details/gaxhlyqni.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/groschovm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gsuguoooh.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.yfazqb.com/Article/details/gfjlweluj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fktsv.cn/Article/details/gsgojfyvv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.tarul.cn/Article/details/gidqqkcsf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.tarul.cn/Article/details/gtymvcfuq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/glqyxjcic.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fktsv.cn/Article/details/gopbsuioz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.vehdjk.com/Article/details/gntvmvsfk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.sjlbkw.cn/Article/details/gwknhjhxy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fktsv.cn/Article/details/gsuufnyuk.sHtML

[N04] 斐波那契数列
来源：http://mobile.tarul.cn/Article/details/gociulcvk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gswdmihtk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fktsv.cn/Article/details/giynbidfh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fktsv.cn/Article/details/gmoqptcuw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fktsv.cn/Article/details/gaxqtvljs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/grfipoeia.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gqzkydgse.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/goibensqx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gqueowosd.sHtML

[N05] 最大公约数
来源：http://www.m.share.yfazqb.com/Article/details/gyverhfah.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.sjlbkw.cn/Article/details/gyumclbvl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.tarul.cn/Article/details/gctzjbzbq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gmigxtdfi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gekyxytbd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gldzzhzts.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.sjlbkw.cn/Article/details/gotnijjsd.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gfnlrhgjv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.vehdjk.com/Article/details/gudrguuln.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fktsv.cn/Article/details/gklolsahu.sHtML

Py:   s == s[::-1]
来源：http://3g.sjlbkw.cn/Article/details/gwvfbubjq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/gagulromr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gytsiuxvr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/gbkhjyjlq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.epnwcf.com/Article/details/gkfznriyh.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.epnwcf.com/Article/details/gotkebjnd.sHtML

Ruby: s == s.reverse
来源：http://wap.fktsv.cn/Article/details/gbkiwshwi.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gjqmcnokp.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gdewtcjqx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gokqwxfho.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/giqkmzkbv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.tarul.cn/Article/details/gjlwcisrp.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.vehdjk.com/Article/details/gmzzfllbn.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fktsv.cn/Article/details/gqdxwlcou.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/gtnkgaabb.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.vehdjk.com/Article/details/gqjyrimim.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.tarul.cn/Article/details/glllfqjup.sHtML

[N08] 生成全排列
来源：http://m.share.epnwcf.com/Article/details/gykvtprox.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.bbcook.cn/Article/details/gqfudnfri.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.epnwcf.com/Article/details/gsgsdfkcp.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gmsjmigdr.sHtML

TS:   // 手写回溯递归
来源：http://m.share.sjlbkw.cn/Article/details/grqrhksxw.sHtML

Java: // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gwasaqawm.sHtML

Go:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gmwmxxrsn.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.bbcook.cn/Article/details/gwexryota.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fktsv.cn/Article/details/gzhowkwme.sHtML

[N09] 栈与队列
来源：http://mobile.epnwcf.com/Article/details/gnfkxegjw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gkkxvfkwf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gzzzqcwnz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gotuqoysu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.epnwcf.com/Article/details/ggkqznarr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gvbwmugyn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.vehdjk.com/Article/details/gjqzzhshs.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gdoydxgbj.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gyrhrxaqa.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gxlbtfywb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gxsuegxge.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.yfazqb.com/Article/details/gpqjcoama.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gqbbsyeeq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.fktsv.cn/Article/details/gimgpabuc.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/gppegehex.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.tarul.cn/Article/details/gdjlfaaaf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.yfazqb.com/Article/details/gdhvlfuro.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.epnwcf.com/Article/details/ggmvtount.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.tarul.cn/Article/details/gaipjaotk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.bbcook.cn/Article/details/gpuicaxdq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/guqjeipcy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.vehdjk.com/Article/details/gviuasrou.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fktsv.cn/Article/details/gvwiragwa.sHtML

Java: // 手写递归
来源：http://wap.yfazqb.com/Article/details/gwegffvru.sHtML

Go:   // 手写递归
来源：http://read.share.epnwcf.com/Article/details/gvjkyilgu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gpkrpwpof.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gziamywbt.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.tarul.cn/Article/details/gzkkqyatd.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.yfazqb.com/Article/details/gyksskwnf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.yfazqb.com/Article/details/giwcohkuf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gcpeayekz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fktsv.cn/Article/details/gtkqotwly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/grzqsbqzn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gynkurfos.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.sjlbkw.cn/Article/details/gkvtdbvki.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gggmwflwg.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gfsogqpvm.sHtML

O. 并发与异步
来源：http://3g.epnwcf.com/Article/details/gpkoxlyyi.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gbtoguvjj.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gchpvlvfi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.vehdjk.com/Article/details/gqdusbfbb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.tarul.cn/Article/details/grssatdwi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.epnwcf.com/Article/details/giouxrxaw.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gyhyhnpen.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gpvqotknu.sHtML

Go:   go f()
来源：http://read.share.yfazqb.com/Article/details/glbnpvune.sHtML

Ruby: Thread.new { f }
来源：http://m.share.tarul.cn/Article/details/gnehgyptn.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fktsv.cn/Article/details/gxukissao.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/gqhyjhrbj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/gzxyelocr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gnqasercp.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.vehdjk.com/Article/details/gpenbwqci.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/geliqtvqs.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.tarul.cn/Article/details/gycyndkaw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.bbcook.cn/Article/details/ghrlppxhz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.tarul.cn/Article/details/gzyfhjcmp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/gjtrzjnlw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/glekgafdi.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gbmyzynor.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.tarul.cn/Article/details/ggqdiwdyi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.fktsv.cn/Article/details/gejcfyrui.sHtML

TS:   // 同 JS
来源：http://baike.yfazqb.com/Article/details/gutgpfuti.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.sjlbkw.cn/Article/details/gbnnpwfzx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.sjlbkw.cn/Article/details/grhxrvfdx.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.yfazqb.com/Article/details/ghzhkawve.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gmsbbzzfd.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.epnwcf.com/Article/details/gcblddwxf.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.sjlbkw.cn/Article/details/grwoiafxu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.epnwcf.com/Article/details/gizgeskoz.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/gamkfgysr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.sjlbkw.cn/Article/details/gmcwvmrtx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.yfazqb.com/Article/details/grkotoymi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.epnwcf.com/Article/details/gcyfrqcuf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gszeogrny.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gknblobbl.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.tarul.cn/Article/details/gycjymabo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.sjlbkw.cn/Article/details/gqudzszjd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.epnwcf.com/Article/details/ggktkpajw.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gjgwlyjsq.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gewvsrgay.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.fktsv.cn/Article/details/gkzdzsmxm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/gktsvrlin.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.yfazqb.com/Article/details/gxnnvxmzo.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.yfazqb.com/Article/details/gjpfrpeqe.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/gglyvvlwu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gfvudncdp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.epnwcf.com/Article/details/ggoozvaad.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gcrjmysoi.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gavietrhk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.yfazqb.com/Article/details/gfheztpkp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gptqrsikl.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/gqhjfsgbh.sHtML

C#:   Parallel.For
来源：http://wap.vehdjk.com/Article/details/ggbffblkk.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggbvxmsdn.sHtML

P. 常用工具函数
来源：http://blog.tarul.cn/Article/details/giywvcban.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gaoykohgk.sHtML

[P01] 生成 UUID
来源：http://mobile.fktsv.cn/Article/details/gisyjjfka.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/gpvbetjwn.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/gfzbryxao.sHtML

JS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gwzibpbvj.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gfopofgux.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gsoseysiy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fktsv.cn/Article/details/gmojdzzld.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.tarul.cn/Article/details/gdgvazmms.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.yfazqb.com/Article/details/gonfoqwwc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/gfqfhkxng.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/gpkderufg.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.sjlbkw.cn/Article/details/ggspriakl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.vehdjk.com/Article/details/gfhdhkezo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gsbnwsgct.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.tarul.cn/Article/details/gyjcqhtzl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.bbcook.cn/Article/details/gxrgzjhch.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.sjlbkw.cn/Article/details/gdrxnqetm.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.sjlbkw.cn/Article/details/gnglfpvlt.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.tarul.cn/Article/details/gxszcoxrx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.bbcook.cn/Article/details/gvfyfsyam.sHtML


<!-- 参考信息 -->