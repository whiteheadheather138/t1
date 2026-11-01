代发 wailian999

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.vehdjk.com/Article/details/gmgyerzdb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.bbcook.cn/Article/details/gyapvnxhk.sHtML

[L05] 上传文件（multipart）
来源：http://blog.sjlbkw.cn/Article/details/gsscupsvu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.epnwcf.com/Article/details/ggdgdbynn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.vehdjk.com/Article/details/ghflynnxe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.tarul.cn/Article/details/gnskdafly.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.sjlbkw.cn/Article/details/gsvaazpaw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.vehdjk.com/Article/details/gtofdiwqt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.bbcook.cn/Article/details/gquhsjfge.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.vehdjk.com/Article/details/gxeqfmemm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.yfazqb.com/Article/details/gmfspsuym.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.yfazqb.com/Article/details/gymqxyqyu.sHtML

Py:   resp.json()
来源：http://blog.tarul.cn/Article/details/glzqshyfy.sHtML

PHP:  json_decode($body, true);
来源：http://wap.yfazqb.com/Article/details/gsmhilffd.sHtML

JS:   await resp.json()
来源：http://baike.bbcook.cn/Article/details/gdacudhgb.sHtML

TS:   await resp.json()
来源：http://3g.tarul.cn/Article/details/gqnzcfmjn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.bbcook.cn/Article/details/ghhsanrpq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.yfazqb.com/Article/details/gtadyhrmo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.vehdjk.com/Article/details/gkiqmtjoy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.epnwcf.com/Article/details/gschnckwp.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gbtopclyz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.yfazqb.com/Article/details/gfsbmfgxh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.yfazqb.com/Article/details/gvvlxnpgt.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gopzytslf.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.bbcook.cn/Article/details/glrdrmcsi.sHtML

Java: resp.statusCode()
来源：http://blog.fktsv.cn/Article/details/gmufjcdtz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.epnwcf.com/Article/details/ghmnfiufl.sHtML

Ruby: resp.code.to_i
来源：http://blog.sjlbkw.cn/Article/details/gckueuwcq.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.bbcook.cn/Article/details/gpjjovhwy.sHtML

[L08] 并发请求多个地址
来源：http://3g.epnwcf.com/Article/details/ghapnchfd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gdpgvewba.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/gslapsdbl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.sjlbkw.cn/Article/details/gucxzxsdo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gpuzrrcya.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.sjlbkw.cn/Article/details/gqhfwjuif.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.vehdjk.com/Article/details/gkyoqosdv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.bbcook.cn/Article/details/gsiadjfhk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.yfazqb.com/Article/details/gymwdbyzz.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gboxmayuw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.bbcook.cn/Article/details/gxtqsbhai.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gdgalujnw.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gwbkqrxuv.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gpdstdjmf.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fktsv.cn/Article/details/ghpbfqrnf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.bbcook.cn/Article/details/gajdtxyah.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.bbcook.cn/Article/details/gsopppwuw.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gseoydlgu.sHtML

Go:   os.Args[1:]
来源：http://wap.sjlbkw.cn/Article/details/ggxywboyh.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gobuihqft.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gddsaodrn.sHtML

[M02] 读取环境变量
来源：http://m.share.vehdjk.com/Article/details/gkitsuqbk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.tarul.cn/Article/details/gmsuhvrcu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.tarul.cn/Article/details/gvgsbwzox.sHtML

JS:   process.env.HOME
来源：http://www.blog.vehdjk.com/Article/details/gxssgvhtk.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/ghnvihdsr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gjpodzpfz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gxqmdjhgc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fktsv.cn/Article/details/gibanmitl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.epnwcf.com/Article/details/gmnmewaou.sHtML

[M03] 执行外部命令
来源：http://wap.sjlbkw.cn/Article/details/gjobbaghc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/gmfwqqrxo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.sjlbkw.cn/Article/details/gocnljimj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.tarul.cn/Article/details/gtuwwrlsz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gtrvvkcup.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/glssndiyn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/gwavlqxpw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.vehdjk.com/Article/details/goaqyxunm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.yfazqb.com/Article/details/gggxnwpiw.sHtML

[M04] 获取当前工作目录
来源：http://wap.tarul.cn/Article/details/gajuxxjei.sHtML

Py:   os.getcwd()
来源：http://wap.epnwcf.com/Article/details/gsqgraurn.sHtML

PHP:  getcwd();
来源：http://mobile.fktsv.cn/Article/details/gskgnhkox.sHtML

JS:   process.cwd()
来源：http://www.share.sjlbkw.cn/Article/details/gihviwawn.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/gmmkavsbx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gemrabauk.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/gcvigxfri.sHtML

Ruby: Dir.pwd
来源：http://blog.epnwcf.com/Article/details/gxwovvtfy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.epnwcf.com/Article/details/glhrcvsyw.sHtML

[M05] 设置退出码
来源：http://mobile.yfazqb.com/Article/details/gdamgnvps.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gtarttpaq.sHtML

PHP:  exit(1);
来源：http://www.share.fktsv.cn/Article/details/gufjvxqtz.sHtML

JS:   process.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gmeitjins.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/ghwwuazov.sHtML

Java: System.exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gfmzpgjmp.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/gywwdqvoa.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gfsdazjse.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.bbcook.cn/Article/details/glgeobkwd.sHtML

[M06] 向标准错误输出
来源：http://3g.vehdjk.com/Article/details/gwxqcveqo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.vehdjk.com/Article/details/gosbjzvdv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.sjlbkw.cn/Article/details/gkuogdldn.sHtML

JS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/geygwjmza.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gtkbljmki.sHtML

Java: System.err.println("err")
来源：http://www.blog.vehdjk.com/Article/details/gddnpqgzf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.epnwcf.com/Article/details/grcqraois.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gtqqejksk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.yfazqb.com/Article/details/greoeswyx.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.vehdjk.com/Article/details/gmsjdqpfp.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.sjlbkw.cn/Article/details/ggxrymnni.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.epnwcf.com/Article/details/gvlkxfsks.sHtML

JS:   require.main === module
来源：http://www.share.vehdjk.com/Article/details/glpqaqqel.sHtML

TS:   require.main === module
来源：http://mobile.epnwcf.com/Article/details/gjrktcebq.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gnzoruboj.sHtML

Go:   func main()
来源：http://baike.fktsv.cn/Article/details/glnewfexw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gfxwizbqv.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.vehdjk.com/Article/details/gefuuaurm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.sjlbkw.cn/Article/details/gbkxdnrig.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.vehdjk.com/Article/details/ggvumiyoc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gnkciuhvt.sHtML

JS:   process.platform;  process.version
来源：http://m.share.vehdjk.com/Article/details/gicsjdotz.sHtML

TS:   process.platform;  process.version
来源：http://m.share.yfazqb.com/Article/details/gwtrkbcri.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gictmxayk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/ggiqettod.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.bbcook.cn/Article/details/gxbxphojr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.tarul.cn/Article/details/gampndytv.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gvhmskwni.sHtML

N. 数据结构与算法
来源：http://blog.sjlbkw.cn/Article/details/gbzktokgs.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gdviilzqz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.vehdjk.com/Article/details/gvkxfdzgs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gnvikuaow.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.yfazqb.com/Article/details/gzhivhwxj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gxilmofnf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gtawfktus.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.bbcook.cn/Article/details/gbzekglsg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/ghnabdgox.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gknxiolzw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/grtsflkxy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/gssgccctu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fktsv.cn/Article/details/gimzcivld.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/gnjuuvosy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.bbcook.cn/Article/details/gvblpjbdz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gpmenykkb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.vehdjk.com/Article/details/glhgnrrda.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/gbrhnosqp.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/ghdmiufcl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.epnwcf.com/Article/details/gxrgkqilk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.tarul.cn/Article/details/ggaaofgun.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gipotgmph.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.vehdjk.com/Article/details/gslbhpdrd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.bbcook.cn/Article/details/gclkynloc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.bbcook.cn/Article/details/grrzgrufv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.vehdjk.com/Article/details/gnkhtsayc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.epnwcf.com/Article/details/gjcsrdncm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.epnwcf.com/Article/details/gsixwhplv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.vehdjk.com/Article/details/gvminxjvo.sHtML

[N04] 斐波那契数列
来源：http://m.share.sjlbkw.cn/Article/details/gsrvmggyo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.bbcook.cn/Article/details/gmqqkzzeb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.epnwcf.com/Article/details/gbwcdpbbk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gwkniunad.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gpcjotqbo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.yfazqb.com/Article/details/gkntmrcig.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.epnwcf.com/Article/details/gcjeucxls.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.sjlbkw.cn/Article/details/gdzuoqqep.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gjdhfuhfi.sHtML

[N05] 最大公约数
来源：http://www.blog.sjlbkw.cn/Article/details/ggfwgyzpl.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gpzascqll.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gwexzhsdr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gufqspgip.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.yfazqb.com/Article/details/gvfxffegm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.bbcook.cn/Article/details/gxmidotlo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fktsv.cn/Article/details/gtoljaanl.sHtML

Ruby: a.gcd(b)
来源：http://m.share.vehdjk.com/Article/details/gbsjtfjlv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.bbcook.cn/Article/details/gfsbbopuo.sHtML

[N06] 判断回文字符串
来源：http://3g.epnwcf.com/Article/details/gzkelakeb.sHtML

Py:   s == s[::-1]
来源：http://baike.vehdjk.com/Article/details/ghdujgmtf.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/gzrcbyuno.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.epnwcf.com/Article/details/gznjdlghi.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gvvvpcjgj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.bbcook.cn/Article/details/gureyqcmu.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.sjlbkw.cn/Article/details/gocqhdekc.sHtML

Ruby: s == s.reverse
来源：http://blog.yfazqb.com/Article/details/gbmerzfax.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.yfazqb.com/Article/details/gerjohars.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fktsv.cn/Article/details/gahvngmas.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.tarul.cn/Article/details/gxbdehoiw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.epnwcf.com/Article/details/gcufuvenb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gvpdbikdf.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/gcimyfvsb.sHtML

Java: // 手写 HashMap
来源：http://mobile.vehdjk.com/Article/details/gaucwvysh.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.bbcook.cn/Article/details/goxejvggz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gicfyllmb.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fktsv.cn/Article/details/gjaoakqno.sHtML

[N08] 生成全排列
来源：http://read.share.epnwcf.com/Article/details/gycmolzem.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gxkjinbrx.sHtML

PHP:  // 手写递归交换
来源：http://blog.fktsv.cn/Article/details/gqrigjrdp.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gamvaaabf.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fktsv.cn/Article/details/gjrpajxcz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gxowpahdt.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/ggeeksazu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/ghnnngqtj.sHtML

C#:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/glqbgolwl.sHtML

[N09] 栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/ggzqthqnr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.tarul.cn/Article/details/grbifluan.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.yfazqb.com/Article/details/gtipsmhua.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gtisauhzg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.epnwcf.com/Article/details/gbgoekubt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.epnwcf.com/Article/details/gbueelgzp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/gtjrhhnjz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fktsv.cn/Article/details/gkxoyupkg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/gtcqljwwa.sHtML

[N10] 链表节点定义
来源：http://baike.fktsv.cn/Article/details/gildbhjfb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fktsv.cn/Article/details/ggzzdxrag.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.vehdjk.com/Article/details/gmicnukrb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/guztabzbh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.yfazqb.com/Article/details/gjrezpnrj.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.yfazqb.com/Article/details/guhebjsfk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gmcnlwnvn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/gipozcuvv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.bbcook.cn/Article/details/gvxysidkl.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.epnwcf.com/Article/details/grpagmgxd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/getyuygeo.sHtML

PHP:  // 手写递归函数
来源：http://m.share.yfazqb.com/Article/details/gpabgpstj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gfzqdcqec.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gwaxaupsn.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gxomomewm.sHtML

Go:   // 手写递归
来源：http://3g.fktsv.cn/Article/details/gucnqwrmf.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.vehdjk.com/Article/details/girhdukyn.sHtML

C#:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/gfuwdwnfz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fktsv.cn/Article/details/gygytxokh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.fktsv.cn/Article/details/guerarykr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fktsv.cn/Article/details/gwoxswigz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gwmqmdsyy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.yfazqb.com/Article/details/gzdagxluu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gjrmqrrtm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.tarul.cn/Article/details/gttgyzbno.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.epnwcf.com/Article/details/gnjuiyrgq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gzatkeeuq.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gilxjbwrg.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gksokfrgn.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gsiferdjm.sHtML

[O01] 启动一个线程
来源：http://mobile.vehdjk.com/Article/details/ghrbmwxgn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.yfazqb.com/Article/details/gyyskwwvv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.vehdjk.com/Article/details/ggkncbvvc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.epnwcf.com/Article/details/gbzpavyjr.sHtML

TS:   // 同 JS
来源：http://www.blog.bbcook.cn/Article/details/gcjemmpuh.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.yfazqb.com/Article/details/gnqxmwynq.sHtML

Go:   go f()
来源：http://baike.vehdjk.com/Article/details/gzymmauop.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gulrpzlkd.sHtML

C#:   Task.Run(() => F());
来源：http://wap.tarul.cn/Article/details/gdvabgsxv.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gtfhocipl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.bbcook.cn/Article/details/gdklbkldz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/ghiqsrewj.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gungolmtw.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.bbcook.cn/Article/details/gntgthoqc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.vehdjk.com/Article/details/gakutllpr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gkcgfoiqt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fktsv.cn/Article/details/glznzkubx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gvteuieqi.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/gfdryrbcr.sHtML

Py:   with lock: shared += 1
来源：http://wap.fktsv.cn/Article/details/gpvgfwocg.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.fktsv.cn/Article/details/gtxijjpfl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gwvsozfja.sHtML

TS:   // 同 JS
来源：http://3g.tarul.cn/Article/details/gmjjkzsdc.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/gjltgtjcj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.tarul.cn/Article/details/gtdbmmdyt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.yfazqb.com/Article/details/gxgdsrcnt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gntfbplwz.sHtML

[O04] 定义异步函数并等待
来源：http://wap.tarul.cn/Article/details/grwlsgusx.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/guwooapvr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.sjlbkw.cn/Article/details/gknahttry.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gqfgwwyyl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gmnbmjhvh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/gmrdgugnj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.bbcook.cn/Article/details/gzyyaysqp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gbopggzlm.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.epnwcf.com/Article/details/gxzlallhz.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fktsv.cn/Article/details/gphucgtlp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fktsv.cn/Article/details/ghstaxemb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.bbcook.cn/Article/details/gbtwzskko.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.epnwcf.com/Article/details/guxfveqns.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.vehdjk.com/Article/details/getehfune.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/grmafjsak.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.bbcook.cn/Article/details/gglijbbhy.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/geljqdkxh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/gwqihceud.sHtML

[O06] 使用进程池
来源：http://www.m.share.epnwcf.com/Article/details/gkiqfoqeu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.tarul.cn/Article/details/gvxqdrloz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fktsv.cn/Article/details/gahzkuyrx.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/ggipbjuul.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/ggiluecvc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.epnwcf.com/Article/details/grxvpjhcm.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.bbcook.cn/Article/details/glgyzlipp.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/gcwnoyjcc.sHtML

C#:   Parallel.For
来源：http://www.m.share.fktsv.cn/Article/details/gydfdrizh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkmkocywq.sHtML

P. 常用工具函数
来源：http://www.m.share.fktsv.cn/Article/details/gtdeglbgf.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/ghncyqcjn.sHtML

[P01] 生成 UUID
来源：http://mobile.vehdjk.com/Article/details/gmbettisd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.tarul.cn/Article/details/ghqxernka.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.bbcook.cn/Article/details/gjnklickc.sHtML

JS:   crypto.randomUUID()
来源：http://3g.bbcook.cn/Article/details/gedfqvlwf.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/gfuzzxrwt.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.yfazqb.com/Article/details/gomgujxck.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fktsv.cn/Article/details/gjllyfwoo.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fktsv.cn/Article/details/glhxxdwxg.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.yfazqb.com/Article/details/glwwieytt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.tarul.cn/Article/details/gdcejyxez.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.fktsv.cn/Article/details/goqzgxwgk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gwjlzvnav.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.sjlbkw.cn/Article/details/gfvldakwe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.bbcook.cn/Article/details/gnezecldu.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gqhvfzxpm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.epnwcf.com/Article/details/gyyvrcehp.sHtML


<!-- 参考信息 -->