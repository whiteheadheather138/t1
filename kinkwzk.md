代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.vehdjk.com/Article/details/ginjjhbco.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.yfazqb.com/Article/details/gdbbexcxs.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.bbcook.cn/Article/details/gyghatkau.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fktsv.cn/Article/details/gokwbchxl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.sjlbkw.cn/Article/details/gdbyccqld.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.bbcook.cn/Article/details/gpubcygdv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.epnwcf.com/Article/details/giuavzjyu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fktsv.cn/Article/details/gbuatdhap.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fktsv.cn/Article/details/glvxgvsab.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fktsv.cn/Article/details/gckcuzcsq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.yfazqb.com/Article/details/govlnzkuw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fktsv.cn/Article/details/grxaxoegh.sHtML

Py:   resp.json()
来源：http://www.blog.tarul.cn/Article/details/gygznpbcl.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.vehdjk.com/Article/details/gbyhtrszz.sHtML

JS:   await resp.json()
来源：http://www.blog.yfazqb.com/Article/details/ggrspwxfb.sHtML

TS:   await resp.json()
来源：http://read.share.sjlbkw.cn/Article/details/gkogtiajg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.sjlbkw.cn/Article/details/gnsihwjye.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.yfazqb.com/Article/details/gwocfrdrs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fktsv.cn/Article/details/gclkmdijh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.tarul.cn/Article/details/gnjzraanb.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.vehdjk.com/Article/details/gpteooqzl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fktsv.cn/Article/details/gypyaciqy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.sjlbkw.cn/Article/details/gswzkymlt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.vehdjk.com/Article/details/gissbqjed.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/gwmnhrluj.sHtML

Java: resp.statusCode()
来源：http://www.share.sjlbkw.cn/Article/details/gnmcynpqx.sHtML

Go:   resp.StatusCode
来源：http://blog.sjlbkw.cn/Article/details/gabptflbj.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gaopftetc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gvnxesqfm.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gedaunelq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.bbcook.cn/Article/details/gllxejyhg.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.tarul.cn/Article/details/gzlssuquz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fktsv.cn/Article/details/gtjzzuxlk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.bbcook.cn/Article/details/guxixympw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.tarul.cn/Article/details/grjjwmybf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.tarul.cn/Article/details/gkiuxhjsn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fktsv.cn/Article/details/gzimbmgqv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.bbcook.cn/Article/details/gnizlnjub.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gedvkuvuz.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.epnwcf.com/Article/details/gjyspyvre.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/ggkqranap.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gidgyujxf.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gtnzqdbsh.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.yfazqb.com/Article/details/gqqfhofbq.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gcoipvmxf.sHtML

TS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gavwnjaca.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.tarul.cn/Article/details/gvecmwqju.sHtML

Go:   os.Args[1:]
来源：http://read.share.fktsv.cn/Article/details/gmpnddxub.sHtML

Ruby: ARGV
来源：http://read.share.vehdjk.com/Article/details/ghjjwpeks.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fktsv.cn/Article/details/gaolsjodn.sHtML

[M02] 读取环境变量
来源：http://www.m.share.bbcook.cn/Article/details/gixfczkfi.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gsvfittkv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.yfazqb.com/Article/details/giuvtwejh.sHtML

JS:   process.env.HOME
来源：http://mobile.yfazqb.com/Article/details/gxhdilvkr.sHtML

TS:   process.env.HOME
来源：http://www.m.share.tarul.cn/Article/details/gtwghzorz.sHtML

Java: System.getenv("HOME")
来源：http://blog.sjlbkw.cn/Article/details/ghwqnsrum.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gknkllvhy.sHtML

Ruby: ENV["HOME"]
来源：http://blog.sjlbkw.cn/Article/details/grwlgdidb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/gmdudxaep.sHtML

[M03] 执行外部命令
来源：http://blog.bbcook.cn/Article/details/gpozcfwcj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.sjlbkw.cn/Article/details/goxthsfud.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gklkzkhko.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gwywthtfe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fktsv.cn/Article/details/gaakcjhfy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.tarul.cn/Article/details/gsoelwtni.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/gjfjskmul.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/gsrjfvfui.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.vehdjk.com/Article/details/gthgppjjo.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/gkapmdlry.sHtML

Py:   os.getcwd()
来源：http://www.blog.bbcook.cn/Article/details/gmpgbnujj.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gjueabowm.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gqxvqyodk.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/ghsugkyht.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.sjlbkw.cn/Article/details/glhreprwm.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gditzszha.sHtML

Ruby: Dir.pwd
来源：http://www.blog.vehdjk.com/Article/details/gnqljoaqq.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.vehdjk.com/Article/details/gwvrcoibh.sHtML

[M05] 设置退出码
来源：http://baike.epnwcf.com/Article/details/gxohsfzzn.sHtML

Py:   sys.exit(1)
来源：http://read.share.bbcook.cn/Article/details/gkgjglosl.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gtzgmtygw.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gguqlyadt.sHtML

TS:   process.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gdjdqbqpp.sHtML

Java: System.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gyggkuzou.sHtML

Go:   os.Exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gelruklgx.sHtML

Ruby: exit 1
来源：http://3g.sjlbkw.cn/Article/details/gaawmupux.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.epnwcf.com/Article/details/gkzytlieh.sHtML

[M06] 向标准错误输出
来源：http://m.share.sjlbkw.cn/Article/details/gopiouojf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gqyjjnrdx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gaqoxfueb.sHtML

JS:   console.error("err")
来源：http://blog.epnwcf.com/Article/details/ggseorakz.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/gqhyysijo.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/gkzhzfvlm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.tarul.cn/Article/details/gnxzsewlk.sHtML

Ruby: warn "err"
来源：http://m.share.vehdjk.com/Article/details/gjiklpjxq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gpiylinxa.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gpizljgjs.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.sjlbkw.cn/Article/details/gvpclvkng.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.vehdjk.com/Article/details/gcukxghku.sHtML

JS:   require.main === module
来源：http://m.share.tarul.cn/Article/details/gyaocoopp.sHtML

TS:   require.main === module
来源：http://www.blog.yfazqb.com/Article/details/glnprdycy.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.epnwcf.com/Article/details/gmwawjduy.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/gxtnyxgxw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gmmslmxys.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gcyfolxfy.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.epnwcf.com/Article/details/gaziazipn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fktsv.cn/Article/details/gapevehdk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.bbcook.cn/Article/details/genbalqjj.sHtML

JS:   process.platform;  process.version
来源：http://3g.tarul.cn/Article/details/gzftkgwqg.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.vehdjk.com/Article/details/gnvircjrc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.sjlbkw.cn/Article/details/gidfwsfwp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fktsv.cn/Article/details/grbrwkiew.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gzwwwkrtk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/gpbvupdaw.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gwofhxwph.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gaohfkdjo.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gvbbvvabc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.bbcook.cn/Article/details/glextcfec.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gpfujtrmm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gpmqyxbue.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.epnwcf.com/Article/details/gunjbqrbj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gkamdlgyc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fktsv.cn/Article/details/gweciklph.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.epnwcf.com/Article/details/granpvuwo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/glvhjgbno.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fktsv.cn/Article/details/goisftwrk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.tarul.cn/Article/details/gcgewpivo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/glnjuqtul.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gnuuuhupn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.vehdjk.com/Article/details/gttkhaaiu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/glrkakgqy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gqonjqxgq.sHtML

Go:   slices.Sort(arr)
来源：http://wap.sjlbkw.cn/Article/details/gmiprycsh.sHtML

Ruby: arr.sort
来源：http://m.share.yfazqb.com/Article/details/gcpcgebel.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.vehdjk.com/Article/details/gvhamnsjy.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/gkuckdrht.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/ghodljuya.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.epnwcf.com/Article/details/gqbenhzic.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gmjrgfiia.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gxxmqbfaw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.vehdjk.com/Article/details/gqhrrmdud.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.tarul.cn/Article/details/gyrjrkscm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.vehdjk.com/Article/details/gpupubrqw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/gyncltdtz.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/gxkkquwjn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.yfazqb.com/Article/details/gqxcoykyv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gfsszuhlb.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gadggcfle.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/grqamexjq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/gpmsdesip.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/glabymtdh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gmwcqicsa.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/ggperetuk.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gessezdod.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gsgzxnxqn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.yfazqb.com/Article/details/gxmsobjon.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gvtlzorfx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gtgunsmak.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fktsv.cn/Article/details/gdxiqrqef.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.tarul.cn/Article/details/gkzygpoxl.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.tarul.cn/Article/details/ghhcaibuj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.tarul.cn/Article/details/gtywvnlqj.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.sjlbkw.cn/Article/details/gpgyjvmpa.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gxjftdtdj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.vehdjk.com/Article/details/goznshohu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gmmhlmhrk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/gbpyrgxyw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.epnwcf.com/Article/details/gejijdqny.sHtML

Go:   // 双指针从两端比较
来源：http://wap.bbcook.cn/Article/details/gxlcrqdyt.sHtML

Ruby: s == s.reverse
来源：http://3g.fktsv.cn/Article/details/gkxzrjufa.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.sjlbkw.cn/Article/details/gcdbdinrh.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.epnwcf.com/Article/details/gyizdhoac.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fktsv.cn/Article/details/gvfriwrrc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.yfazqb.com/Article/details/gcpdvlbfh.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.vehdjk.com/Article/details/gyllewlos.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fktsv.cn/Article/details/gfozrqbiw.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gsnwprvri.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.epnwcf.com/Article/details/gdicmumtq.sHtML

Ruby: // 手写 Hash
来源：http://www.share.yfazqb.com/Article/details/glzsszqdq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.bbcook.cn/Article/details/gyakifrdv.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gguqboifa.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.vehdjk.com/Article/details/gajkvnkel.sHtML

PHP:  // 手写递归交换
来源：http://baike.epnwcf.com/Article/details/glejuyzds.sHtML

JS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/guajymdmv.sHtML

TS:   // 手写回溯递归
来源：http://www.share.sjlbkw.cn/Article/details/gcyvjpbii.sHtML

Java: // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gixajwagp.sHtML

Go:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/gqgfsctko.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.yfazqb.com/Article/details/gzmfiuvbh.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gbovwhfbf.sHtML

[N09] 栈与队列
来源：http://baike.tarul.cn/Article/details/gwbhiexsf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.tarul.cn/Article/details/gawqhddie.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.epnwcf.com/Article/details/geuwmuemw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/groovaxsw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.sjlbkw.cn/Article/details/gmtbmpcey.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.vehdjk.com/Article/details/gmfueyvdo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/glxaekwva.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/ghlwsjuwn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gaksuvviz.sHtML

[N10] 链表节点定义
来源：http://wap.yfazqb.com/Article/details/gepvdimij.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fktsv.cn/Article/details/gylwguxsm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.vehdjk.com/Article/details/gcacvkggo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.sjlbkw.cn/Article/details/gqehmjxmk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gvrapbiqw.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/gqcebiein.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.sjlbkw.cn/Article/details/gaydndfer.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.epnwcf.com/Article/details/gmvjvrzfa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.yfazqb.com/Article/details/gruozwvlk.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.bbcook.cn/Article/details/gajlxytvt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.bbcook.cn/Article/details/gelkrzpmf.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/giupqpjvo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/ghacaoiey.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/gkgjvzfeg.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gnnlaeaoc.sHtML

Go:   // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/givdhezgi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.epnwcf.com/Article/details/gsffeqbky.sHtML

C#:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gdgmxganw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.epnwcf.com/Article/details/gvfqlyuhc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.yfazqb.com/Article/details/gdbildbeq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.epnwcf.com/Article/details/gnlqlwqwt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/ginpyvofo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gbhgmpdtj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/gaftgkdhq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gpfipxmik.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.sjlbkw.cn/Article/details/gjjoqlbwc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gtxtahpgj.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gglrtluss.sHtML

O. 并发与异步
来源：http://mobile.bbcook.cn/Article/details/gqubaooex.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/grbuczbtp.sHtML

[O01] 启动一个线程
来源：http://mobile.tarul.cn/Article/details/gxsmersyk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.bbcook.cn/Article/details/gxzwagclp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gbahtaeeo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gjgakvhzx.sHtML

TS:   // 同 JS
来源：http://mobile.tarul.cn/Article/details/gdpkiycxr.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.epnwcf.com/Article/details/gplovldfj.sHtML

Go:   go f()
来源：http://www.share.tarul.cn/Article/details/gdnqmdsjr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fktsv.cn/Article/details/gyjifywmn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.epnwcf.com/Article/details/gdnqjibtg.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gimiapdsk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.sjlbkw.cn/Article/details/glpeqrmln.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/govooipco.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gtncgbonb.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gvwmzrfzc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/glguhngop.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gaowibcaz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gziypmtkf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fktsv.cn/Article/details/gldsylcgu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.epnwcf.com/Article/details/gekbjukwv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.bbcook.cn/Article/details/gmayxrzrw.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gpppjttli.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/ggpinwzta.sHtML

TS:   // 同 JS
来源：http://m.share.bbcook.cn/Article/details/gkdburkkk.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gfdqglhri.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.yfazqb.com/Article/details/gqefxptvv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.sjlbkw.cn/Article/details/guiqxnfaz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.tarul.cn/Article/details/glrfotcwi.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.epnwcf.com/Article/details/gprofwkyd.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.yfazqb.com/Article/details/gtgbhcqmi.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.epnwcf.com/Article/details/ggxpzbnoc.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.tarul.cn/Article/details/grgsqetpi.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gzavupbhw.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/ggxufhigi.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fktsv.cn/Article/details/gzmvpyjzc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.yfazqb.com/Article/details/gjahxyhou.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.yfazqb.com/Article/details/gijnwkvqh.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.fktsv.cn/Article/details/ggrkadbrq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.epnwcf.com/Article/details/gjkmzpedb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gruzrwbpd.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.bbcook.cn/Article/details/gegidprhg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.vehdjk.com/Article/details/glrzeyadc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.yfazqb.com/Article/details/gssvbuxmt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.sjlbkw.cn/Article/details/giuknjjyn.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/gyctxcuxn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.vehdjk.com/Article/details/gziukxppb.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/gkglykqrz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.tarul.cn/Article/details/gtfauphpn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fktsv.cn/Article/details/geuviloyw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gkorsttlv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gzbhtszcc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.tarul.cn/Article/details/gvftxkzzh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.yfazqb.com/Article/details/gjwxktzpe.sHtML

Ruby: // fork 块
来源：http://blog.epnwcf.com/Article/details/gzsddshbm.sHtML

C#:   Parallel.For
来源：http://baike.epnwcf.com/Article/details/goeaykwdt.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gjgbcjcid.sHtML

P. 常用工具函数
来源：http://3g.epnwcf.com/Article/details/glaiagiyp.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/grvkfzzeb.sHtML

[P01] 生成 UUID
来源：http://baike.bbcook.cn/Article/details/goagrwdwx.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fktsv.cn/Article/details/gmmxadtys.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/grwooqfky.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gfuelavdx.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.yfazqb.com/Article/details/ggfmcwblh.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.fktsv.cn/Article/details/gvlyuhfal.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gankshmip.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.epnwcf.com/Article/details/grmtcgjow.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.yfazqb.com/Article/details/goiogyrfq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.epnwcf.com/Article/details/gfvsjvudt.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.yfazqb.com/Article/details/gdejqhmvl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.sjlbkw.cn/Article/details/gyxgcpbxj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/gzzvegjnn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fktsv.cn/Article/details/glbghnyez.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://3g.yfazqb.com/Article/details/gmelmtuof.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.bbcook.cn/Article/details/gryrjqkkj.sHtML


<!-- 参考信息 -->