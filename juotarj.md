代发 wailian999

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.epnwcf.com/Article/details/gtavbygka.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.vehdjk.com/Article/details/gffxkjrqn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.epnwcf.com/Article/details/gjlmjxuke.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.yfazqb.com/Article/details/ggnbmfjvq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.tarul.cn/Article/details/gwlhpqeur.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.yfazqb.com/Article/details/gteczkazv.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.epnwcf.com/Article/details/gxdqjxfll.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fktsv.cn/Article/details/glolxncea.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.yfazqb.com/Article/details/giegvxrdg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.vehdjk.com/Article/details/gfyyetxyd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fktsv.cn/Article/details/gzltbflkv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.sjlbkw.cn/Article/details/gkxmxnwgy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.sjlbkw.cn/Article/details/ghnagjjaa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.tarul.cn/Article/details/gbzeokqdk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.bbcook.cn/Article/details/gfkafgsaz.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.bbcook.cn/Article/details/gglrhthud.sHtML

Py:   resp.json()
来源：http://wap.fktsv.cn/Article/details/gvhpvpffb.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.tarul.cn/Article/details/gjwzlwxvt.sHtML

JS:   await resp.json()
来源：http://m.share.vehdjk.com/Article/details/gpzsfsiwi.sHtML

TS:   await resp.json()
来源：http://baike.sjlbkw.cn/Article/details/glccwqhvq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.vehdjk.com/Article/details/gmodznejt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.epnwcf.com/Article/details/gfjrgmzxw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.vehdjk.com/Article/details/guldgaeqe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.yfazqb.com/Article/details/giepxfhxp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.bbcook.cn/Article/details/gkpfigjbu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.sjlbkw.cn/Article/details/gxdohcrnd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gsljzaepp.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.epnwcf.com/Article/details/gkiaieveg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.yfazqb.com/Article/details/gtulsvwku.sHtML

Java: resp.statusCode()
来源：http://3g.sjlbkw.cn/Article/details/gzwjmamoq.sHtML

Go:   resp.StatusCode
来源：http://baike.sjlbkw.cn/Article/details/gvsotsgvx.sHtML

Ruby: resp.code.to_i
来源：http://3g.bbcook.cn/Article/details/ggbbhnkpu.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fktsv.cn/Article/details/gbubdsqmh.sHtML

[L08] 并发请求多个地址
来源：http://read.share.yfazqb.com/Article/details/gdjbhgrdy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.vehdjk.com/Article/details/gvtxuqtzu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/ghaewhcjb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/gjgskwpnv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.bbcook.cn/Article/details/geqhuwmfh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/glcttesog.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/ghcoddgrj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.bbcook.cn/Article/details/gzoaksntm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.epnwcf.com/Article/details/gzszjxoix.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gwivectfv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gnptknydo.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glckzouoi.sHtML

[M01] 读取命令行参数
来源：http://read.share.sjlbkw.cn/Article/details/gvetauimc.sHtML

Py:   sys.argv[1:]
来源：http://blog.vehdjk.com/Article/details/gjgxfcper.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.yfazqb.com/Article/details/gjtdpqjjo.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gqbnweqip.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.epnwcf.com/Article/details/gulzjswjm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.tarul.cn/Article/details/gbwljhxrp.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/gjjwtdmsp.sHtML

Ruby: ARGV
来源：http://3g.epnwcf.com/Article/details/gtnjeqfyi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.bbcook.cn/Article/details/gizpcxrfc.sHtML

[M02] 读取环境变量
来源：http://www.share.bbcook.cn/Article/details/gpmxtqiui.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gytynvlct.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gwxmiriro.sHtML

JS:   process.env.HOME
来源：http://baike.tarul.cn/Article/details/gefwkdovg.sHtML

TS:   process.env.HOME
来源：http://blog.vehdjk.com/Article/details/ggolyaddy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gthgenvts.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gvqvxvtuo.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fktsv.cn/Article/details/gijrqgchi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/gwfpaciji.sHtML

[M03] 执行外部命令
来源：http://www.share.vehdjk.com/Article/details/gthagiftn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gdhdxlyjd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.vehdjk.com/Article/details/gcgwdmdrs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gebmclnbg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.bbcook.cn/Article/details/gcfkwzoir.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.epnwcf.com/Article/details/gugvizolf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.vehdjk.com/Article/details/gxlukmimh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gqnftnwqf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.bbcook.cn/Article/details/gmltbhqrm.sHtML

[M04] 获取当前工作目录
来源：http://3g.tarul.cn/Article/details/goptbuezd.sHtML

Py:   os.getcwd()
来源：http://read.share.sjlbkw.cn/Article/details/gpdhuoqcd.sHtML

PHP:  getcwd();
来源：http://read.share.vehdjk.com/Article/details/gdxbtbygc.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/glyfcraks.sHtML

TS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/goztxoycl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/goabiwqbw.sHtML

Go:   os.Getwd()
来源：http://www.share.vehdjk.com/Article/details/gwcxuuifg.sHtML

Ruby: Dir.pwd
来源：http://www.share.epnwcf.com/Article/details/gfwoyzqwb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.sjlbkw.cn/Article/details/gcppqwnhn.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gutdoopkk.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gjgihcrid.sHtML

PHP:  exit(1);
来源：http://baike.vehdjk.com/Article/details/gakecpunn.sHtML

JS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/ggakoyxum.sHtML

TS:   process.exit(1)
来源：http://m.share.vehdjk.com/Article/details/gajoeryel.sHtML

Java: System.exit(1)
来源：http://baike.tarul.cn/Article/details/gnhqlqzvq.sHtML

Go:   os.Exit(1)
来源：http://wap.epnwcf.com/Article/details/gneugnlts.sHtML

Ruby: exit 1
来源：http://www.blog.fktsv.cn/Article/details/gajdipege.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.yfazqb.com/Article/details/gimeawbjm.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gtppqmysd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fktsv.cn/Article/details/gfkgkvksc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/ghjnsnyva.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gtdlxmerf.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gqoythrij.sHtML

Java: System.err.println("err")
来源：http://wap.epnwcf.com/Article/details/gdakolwjs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.tarul.cn/Article/details/guitiiwax.sHtML

Ruby: warn "err"
来源：http://m.share.epnwcf.com/Article/details/gwbnxycuo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.sjlbkw.cn/Article/details/gywfdhzee.sHtML

[M07] 判断是否为主入口
来源：http://www.share.epnwcf.com/Article/details/grieluklp.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gohulrawl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.vehdjk.com/Article/details/gvqhbbhec.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gxythglfx.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gmoqgiuid.sHtML

Java: public static void main(String[] args)
来源：http://baike.sjlbkw.cn/Article/details/gmdsflpml.sHtML

Go:   func main()
来源：http://mobile.yfazqb.com/Article/details/gdgbdiqio.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.yfazqb.com/Article/details/godisxvip.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gryniyucm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gxqkcmuzv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.tarul.cn/Article/details/gdplcawkx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/ghxsjfxwy.sHtML

JS:   process.platform;  process.version
来源：http://wap.fktsv.cn/Article/details/goevrdpkt.sHtML

TS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gafnylnha.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gbxiryepr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.sjlbkw.cn/Article/details/gqeikbecj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.epnwcf.com/Article/details/giqvedlox.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/gyuiifdnd.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gzsorazwq.sHtML

N. 数据结构与算法
来源：http://baike.epnwcf.com/Article/details/gyrwmrslt.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gogydichy.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.sjlbkw.cn/Article/details/gqvwbcerm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gnnrrxthf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gnumwfrml.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.sjlbkw.cn/Article/details/gwtgjaxyu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/glyrfdvpe.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/gmtbilmhp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gvjjhewfu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fktsv.cn/Article/details/gujltvgoo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.vehdjk.com/Article/details/gcvjlbgiy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.vehdjk.com/Article/details/gjsvjnlju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.tarul.cn/Article/details/gkohuotyr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gqlmtsknm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gsdlssorm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gfblpzksf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/gxvzmccma.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gcnmpcmyu.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/geupjytsm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gqmxelwxe.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.vehdjk.com/Article/details/gjtlkaskp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gilzmmduy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gxoonggwz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.tarul.cn/Article/details/gtbmmztaq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.vehdjk.com/Article/details/gndacqvev.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/gptgyiclh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.yfazqb.com/Article/details/gbivhnerc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.sjlbkw.cn/Article/details/gujnbpqwy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/ggxryyfra.sHtML

[N04] 斐波那契数列
来源：http://read.share.sjlbkw.cn/Article/details/gurnzygno.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/ghuiujnut.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gmdwivzay.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gstiblkdy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/glpwvdxxe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gxpunevws.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.vehdjk.com/Article/details/gtclpfjfs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.sjlbkw.cn/Article/details/giwxjwykz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.tarul.cn/Article/details/gqvezvtfa.sHtML

[N05] 最大公约数
来源：http://www.blog.yfazqb.com/Article/details/gogtxhpts.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gpnzrbcje.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gtxgndjtv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.sjlbkw.cn/Article/details/gnwktaznf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.vehdjk.com/Article/details/gbaawuyta.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.epnwcf.com/Article/details/gjkhjwsds.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.bbcook.cn/Article/details/ggvewgjeh.sHtML

Ruby: a.gcd(b)
来源：http://3g.tarul.cn/Article/details/gtokhjewi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.yfazqb.com/Article/details/gieqtfilq.sHtML

[N06] 判断回文字符串
来源：http://read.share.tarul.cn/Article/details/gbjcixxgd.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gdsndkriq.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fktsv.cn/Article/details/gixzxybuk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gxaeuruxm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gximkkmpr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.tarul.cn/Article/details/ggfcbxllr.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/gdylkwkzo.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/ghddmqejj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.yfazqb.com/Article/details/gdullblwd.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.sjlbkw.cn/Article/details/gpvxyszqg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gwvfuzzfz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.tarul.cn/Article/details/gvfnjlnqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gyrblrzkl.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.bbcook.cn/Article/details/gjyjffbgh.sHtML

Java: // 手写 HashMap
来源：http://mobile.bbcook.cn/Article/details/gnddizfqe.sHtML

Go:   // 手写 map[int]int
来源：http://wap.tarul.cn/Article/details/gvkdevrci.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/guzfwolgk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fktsv.cn/Article/details/gvblwcuhv.sHtML

[N08] 生成全排列
来源：http://blog.tarul.cn/Article/details/gorkbujxr.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gevjjzykk.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/ggfzxtwsr.sHtML

JS:   // 手写回溯递归
来源：http://3g.tarul.cn/Article/details/ggytnjilk.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/giugwhssk.sHtML

Java: // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gfkpbwvqy.sHtML

Go:   // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/gyxxpoupc.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.tarul.cn/Article/details/gpemvngym.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gkkrfdbnl.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gejmtjvjv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.epnwcf.com/Article/details/gfprbitac.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.bbcook.cn/Article/details/gbrvbkext.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gctxcikor.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.tarul.cn/Article/details/gyfaoftcp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/gdsljyehl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/ghhcxhkrn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.sjlbkw.cn/Article/details/goodyivdp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.yfazqb.com/Article/details/geoupelkc.sHtML

[N10] 链表节点定义
来源：http://www.blog.epnwcf.com/Article/details/gvjippvia.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gzquhkbgj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.epnwcf.com/Article/details/gzzuzodfl.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.sjlbkw.cn/Article/details/ghqipsyrz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.vehdjk.com/Article/details/gowvofjga.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gjyvqxvhi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.fktsv.cn/Article/details/gcdzbjofg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fktsv.cn/Article/details/gmxadggkn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.epnwcf.com/Article/details/gtddvgwpx.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.vehdjk.com/Article/details/golbtcvzg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.epnwcf.com/Article/details/grqvxzhcb.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/goycgrsom.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.yfazqb.com/Article/details/gariygcai.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.vehdjk.com/Article/details/gjgiuponc.sHtML

Java: // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gvsrbadwu.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/glwpxpida.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fktsv.cn/Article/details/gyfdyeexv.sHtML

C#:   // 手写递归
来源：http://mobile.epnwcf.com/Article/details/gvpkcuels.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.vehdjk.com/Article/details/ghhsmrtpq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.vehdjk.com/Article/details/gwjeznpqx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.epnwcf.com/Article/details/gyizeeuhu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gcrntisqg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gctfvfmoz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/ghoiphqle.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.sjlbkw.cn/Article/details/guxdnaaaq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.epnwcf.com/Article/details/ggdbfmlqt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.sjlbkw.cn/Article/details/gldhcmcuh.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gmjvuwplr.sHtML

O. 并发与异步
来源：http://blog.yfazqb.com/Article/details/gkbloafyv.sHtML

================================================================================
来源：http://m.share.tarul.cn/Article/details/guslqzopi.sHtML

[O01] 启动一个线程
来源：http://m.share.sjlbkw.cn/Article/details/grjdfjopy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gdwtfteqm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.sjlbkw.cn/Article/details/gggassdyb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/ggsgbfnly.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/ggrdzqacn.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.epnwcf.com/Article/details/gmqljlwno.sHtML

Go:   go f()
来源：http://baike.yfazqb.com/Article/details/gotjqsgox.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fktsv.cn/Article/details/gklabnxen.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.vehdjk.com/Article/details/gxgjybiqy.sHtML

[O02] 使用线程池
来源：http://blog.epnwcf.com/Article/details/geblaxspv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/ghnmwkxho.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/gxyentdlg.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.bbcook.cn/Article/details/gejkcuqdt.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gcolbwwnz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/gmfbfpvnw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gcahkfrrx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gjigbgjqv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gfexullvu.sHtML

[O03] 加锁保护共享数据
来源：http://baike.tarul.cn/Article/details/glgekcwpt.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/ghfhakwui.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.vehdjk.com/Article/details/ghdukloch.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/guyqmkzeu.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gcxluremt.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gfdxfowtc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.fktsv.cn/Article/details/gnvyryoct.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.epnwcf.com/Article/details/gziketeaf.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gcavwfjwi.sHtML

[O04] 定义异步函数并等待
来源：http://wap.yfazqb.com/Article/details/gfhyezjeo.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.tarul.cn/Article/details/glatfdxvp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.vehdjk.com/Article/details/gyrmmjixl.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.tarul.cn/Article/details/ggmbmiepo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.yfazqb.com/Article/details/grjasahce.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gvmwlrymn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gecaovihs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.tarul.cn/Article/details/gjtkpggtu.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.epnwcf.com/Article/details/gywclwtpq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.bbcook.cn/Article/details/ghjnqjioj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fktsv.cn/Article/details/giosmanlj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fktsv.cn/Article/details/gbwfazpqm.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.vehdjk.com/Article/details/ghdawksyi.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/gjmntqymb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.tarul.cn/Article/details/glazwdmyj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gajgqxygb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/gandvvvnq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gaqoxufzy.sHtML

[O06] 使用进程池
来源：http://read.share.vehdjk.com/Article/details/grlhyrjtm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.tarul.cn/Article/details/gyneqhsab.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.yfazqb.com/Article/details/ghaawftga.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.vehdjk.com/Article/details/grewwgdqy.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gjdqomdoi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.vehdjk.com/Article/details/gkunjcnaz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.sjlbkw.cn/Article/details/ghtozsecu.sHtML

Ruby: // fork 块
来源：http://3g.sjlbkw.cn/Article/details/grmpadaon.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gfmbartwy.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gwxorbfcm.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgnfczke.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gswwmptxj.sHtML

[P01] 生成 UUID
来源：http://mobile.bbcook.cn/Article/details/gvbcooako.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.tarul.cn/Article/details/glnwvcibe.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gtplekevh.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/gdhemksls.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gftqxqztt.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gstjlagko.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gketpaehf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.tarul.cn/Article/details/gajpzngpz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/glvornfhv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gdcnoxvze.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gvmloeyzp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/grbpnribq.sHtML


<!-- 参考信息 -->