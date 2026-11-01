代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.bbcook.cn/Article/details/grcuivqlh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.vehdjk.com/Article/details/gxkdvznzb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.sjlbkw.cn/Article/details/gmegufxkc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.vehdjk.com/Article/details/gjeyrxklu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.bbcook.cn/Article/details/gbivzlnml.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.yfazqb.com/Article/details/ggxgwqswc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.epnwcf.com/Article/details/ghtezdblj.sHtML

[L06] 解析响应为 JSON
来源：http://wap.tarul.cn/Article/details/gmhkmxwlr.sHtML

Py:   resp.json()
来源：http://mobile.vehdjk.com/Article/details/gjfsfqyet.sHtML

PHP:  json_decode($body, true);
来源：http://baike.tarul.cn/Article/details/gyyhjjgta.sHtML

JS:   await resp.json()
来源：http://m.share.tarul.cn/Article/details/gbkhbqloa.sHtML

TS:   await resp.json()
来源：http://blog.vehdjk.com/Article/details/gehbxjlfs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.sjlbkw.cn/Article/details/gszvhffeh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fktsv.cn/Article/details/gkgruxleg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.bbcook.cn/Article/details/gthtialji.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.sjlbkw.cn/Article/details/gzylzoowx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.yfazqb.com/Article/details/ghlzgdbhd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.bbcook.cn/Article/details/gbzkeyojq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.vehdjk.com/Article/details/gtwhyixad.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.sjlbkw.cn/Article/details/gffbfclrk.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.yfazqb.com/Article/details/gacwtqmto.sHtML

Java: resp.statusCode()
来源：http://baike.fktsv.cn/Article/details/gqnvoeuth.sHtML

Go:   resp.StatusCode
来源：http://baike.epnwcf.com/Article/details/gwbelshjr.sHtML

Ruby: resp.code.to_i
来源：http://3g.fktsv.cn/Article/details/gmnazlmhv.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.yfazqb.com/Article/details/gkfgbdouu.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fktsv.cn/Article/details/gximovleh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.epnwcf.com/Article/details/gtdpjciuh.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fktsv.cn/Article/details/gibdiwnqe.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.bbcook.cn/Article/details/gxgoybbfd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.yfazqb.com/Article/details/guxlatbnd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.yfazqb.com/Article/details/ggzhburmv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/gmutpyraa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.vehdjk.com/Article/details/gilipiqvc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/gbqheyvzw.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gewmrpfhi.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.vehdjk.com/Article/details/girxdofzp.sHtML

================================================================================
来源：http://www.share.tarul.cn/Article/details/gfqakigjp.sHtML

[M01] 读取命令行参数
来源：http://3g.fktsv.cn/Article/details/gywxqucfa.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/giqcprfjl.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gswgfpuxe.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.yfazqb.com/Article/details/gwywazgwg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/gdwxssrkh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.sjlbkw.cn/Article/details/gmklulzxh.sHtML

Go:   os.Args[1:]
来源：http://mobile.yfazqb.com/Article/details/gjkautgyx.sHtML

Ruby: ARGV
来源：http://baike.vehdjk.com/Article/details/gvuhpbltn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gohplxrib.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/gquxdtesd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gdtpcjmkf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.bbcook.cn/Article/details/ghbtlsijg.sHtML

JS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/goxuuvbut.sHtML

TS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/gnyawofum.sHtML

Java: System.getenv("HOME")
来源：http://wap.fktsv.cn/Article/details/gatdnkadb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.tarul.cn/Article/details/gtsthykbw.sHtML

Ruby: ENV["HOME"]
来源：http://blog.epnwcf.com/Article/details/grbzbgpfl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gitoqriha.sHtML

[M03] 执行外部命令
来源：http://www.blog.bbcook.cn/Article/details/gbwjiyezt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.tarul.cn/Article/details/gaefdifes.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gmgcupibo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gfxhlmcff.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gmaxvrcil.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gxekqllnh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.tarul.cn/Article/details/gezhawkgm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/ggbhnyemc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.sjlbkw.cn/Article/details/gdipydakk.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fktsv.cn/Article/details/ghmwugjvu.sHtML

Py:   os.getcwd()
来源：http://baike.fktsv.cn/Article/details/gzqdsvpdb.sHtML

PHP:  getcwd();
来源：http://wap.tarul.cn/Article/details/ggaohwryy.sHtML

JS:   process.cwd()
来源：http://www.share.vehdjk.com/Article/details/gykqpzwhl.sHtML

TS:   process.cwd()
来源：http://mobile.bbcook.cn/Article/details/gnmxdljnc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/gwhitcgfy.sHtML

Go:   os.Getwd()
来源：http://3g.vehdjk.com/Article/details/guoeohdql.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/gbjxsgeob.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gahcbdonh.sHtML

[M05] 设置退出码
来源：http://mobile.sjlbkw.cn/Article/details/glbfdprmr.sHtML

Py:   sys.exit(1)
来源：http://baike.tarul.cn/Article/details/gtzomaunk.sHtML

PHP:  exit(1);
来源：http://3g.sjlbkw.cn/Article/details/ghtgdhhta.sHtML

JS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gcjvtjdnm.sHtML

TS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gpopyajht.sHtML

Java: System.exit(1)
来源：http://3g.bbcook.cn/Article/details/gmninmlgv.sHtML

Go:   os.Exit(1)
来源：http://baike.fktsv.cn/Article/details/gkrjtbwjm.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/gqmqgiylc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.sjlbkw.cn/Article/details/gloaklbom.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fktsv.cn/Article/details/gwnaubfkg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fktsv.cn/Article/details/gdbonzvbp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.epnwcf.com/Article/details/gtapvddkf.sHtML

JS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gqdkisuaf.sHtML

TS:   console.error("err")
来源：http://m.share.vehdjk.com/Article/details/gfleurrwq.sHtML

Java: System.err.println("err")
来源：http://baike.epnwcf.com/Article/details/gvbydmlkc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/grkhhchht.sHtML

Ruby: warn "err"
来源：http://read.share.bbcook.cn/Article/details/gfxdetbdl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fktsv.cn/Article/details/ghjywmrlc.sHtML

[M07] 判断是否为主入口
来源：http://baike.vehdjk.com/Article/details/gzdayxfkd.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/glnblkzih.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.sjlbkw.cn/Article/details/gpynkkmbk.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/ggcwwakyt.sHtML

TS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gorargjsw.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/ggfoknmnm.sHtML

Go:   func main()
来源：http://baike.bbcook.cn/Article/details/ghlyiawts.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gmidjrkll.sHtML

C#:   static void Main(string[] args)
来源：http://3g.vehdjk.com/Article/details/gtullotlv.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gsspzpntm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.epnwcf.com/Article/details/gylywtbwu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.sjlbkw.cn/Article/details/gjlszcacr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gjjggsbhe.sHtML

TS:   process.platform;  process.version
来源：http://read.share.sjlbkw.cn/Article/details/gvtyfftmu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.vehdjk.com/Article/details/gwxnhrhhh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.epnwcf.com/Article/details/gxobzhpem.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.bbcook.cn/Article/details/gfvjjnldb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fktsv.cn/Article/details/gaehogkji.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/geksxmfmp.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/gbqpvfxuf.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gvmyuimpw.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.sjlbkw.cn/Article/details/grqaraipp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gwmfkcbwo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gnxadxcyd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gvmwryrqc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.vehdjk.com/Article/details/gwhvwngag.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.yfazqb.com/Article/details/gsvjxupny.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.yfazqb.com/Article/details/gcxlmwnav.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fktsv.cn/Article/details/gxvcqenhr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gxuphcsoj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.vehdjk.com/Article/details/gacbesivr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.yfazqb.com/Article/details/guriglnlm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.vehdjk.com/Article/details/gijrqrnjx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.epnwcf.com/Article/details/grqehhqcq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.tarul.cn/Article/details/gkiwyekgv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.tarul.cn/Article/details/ghemxjhub.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.vehdjk.com/Article/details/gtfcikdcq.sHtML

Ruby: arr.sort
来源：http://mobile.bbcook.cn/Article/details/gcorhsqox.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.epnwcf.com/Article/details/gqsjdvccq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fktsv.cn/Article/details/gsqzjxlnh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gwdncbfbb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.bbcook.cn/Article/details/gjvkkjxsy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.tarul.cn/Article/details/gioulwwpy.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gatayhndk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.bbcook.cn/Article/details/gwmuibqkj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fktsv.cn/Article/details/gdaxfayvp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrswmhrq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.bbcook.cn/Article/details/gamhwxxhd.sHtML

[N04] 斐波那契数列
来源：http://m.share.vehdjk.com/Article/details/gzjxdogtm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gqdhwlrng.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.tarul.cn/Article/details/ggrfgweem.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gvtqbajyw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.epnwcf.com/Article/details/gjrvoavgd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/grceggtrj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.bbcook.cn/Article/details/gswicrayv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.yfazqb.com/Article/details/gnxbrcekq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.yfazqb.com/Article/details/gllykdonn.sHtML

[N05] 最大公约数
来源：http://www.share.fktsv.cn/Article/details/ggiwupuzg.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.epnwcf.com/Article/details/gxggveoyd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.vehdjk.com/Article/details/gpgdrwqco.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.epnwcf.com/Article/details/gmgajgtge.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.yfazqb.com/Article/details/gvqxfczmr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.epnwcf.com/Article/details/gsnghfnuq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.epnwcf.com/Article/details/gppsvzear.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gdymjsikp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.sjlbkw.cn/Article/details/gxdbuqvil.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/ghyzumsio.sHtML

Py:   s == s[::-1]
来源：http://www.blog.yfazqb.com/Article/details/gzqjzzwfh.sHtML

PHP:  $s === strrev($s);
来源：http://wap.sjlbkw.cn/Article/details/glcllfics.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.tarul.cn/Article/details/gtxaglwtz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gydliilpr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gkcprmxii.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.vehdjk.com/Article/details/gijpjgxom.sHtML

Ruby: s == s.reverse
来源：http://3g.yfazqb.com/Article/details/gvmanjbpg.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.yfazqb.com/Article/details/gockzvxma.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gldxcfslt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.sjlbkw.cn/Article/details/gugfjvyzt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gdhetpbku.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.vehdjk.com/Article/details/gvbutzzlv.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/giazsrhnn.sHtML

Java: // 手写 HashMap
来源：http://3g.yfazqb.com/Article/details/gtkimgrpn.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fktsv.cn/Article/details/gwnqiskfj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.bbcook.cn/Article/details/gatyvvfnj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.epnwcf.com/Article/details/gxpheewcb.sHtML

[N08] 生成全排列
来源：http://wap.sjlbkw.cn/Article/details/gkhffqnob.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/gqphfjian.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.vehdjk.com/Article/details/gjckaropw.sHtML

JS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gwpvouumz.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gwwgjgfjz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gsibtdoyt.sHtML

Go:   // 手写回溯递归
来源：http://3g.epnwcf.com/Article/details/gnjlleovm.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.yfazqb.com/Article/details/gjggnjnsi.sHtML

C#:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/gfwbtqtgx.sHtML

[N09] 栈与队列
来源：http://www.blog.tarul.cn/Article/details/gtinuvoyd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.bbcook.cn/Article/details/gtepghxfv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.yfazqb.com/Article/details/gzbbuoiqe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gyxhxqmaz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.vehdjk.com/Article/details/gonjewree.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/gplehzwyi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gqsvxsyuc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.tarul.cn/Article/details/gvmkzxqnf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.tarul.cn/Article/details/gngcywsub.sHtML

[N10] 链表节点定义
来源：http://baike.bbcook.cn/Article/details/gaacfrizc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.vehdjk.com/Article/details/gfthjfcqb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.yfazqb.com/Article/details/gobmdjkwp.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fktsv.cn/Article/details/gcqkqxrvr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/glgmcgcys.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.vehdjk.com/Article/details/gifvsxtqh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.bbcook.cn/Article/details/gywpojkrc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fktsv.cn/Article/details/gwdkogqho.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.sjlbkw.cn/Article/details/gvtpjxgpq.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gezboacsf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gbqaqqcmw.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gjrhkophy.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.epnwcf.com/Article/details/ggqekodyp.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gkhtriaij.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/gedsngmkk.sHtML

Go:   // 手写递归
来源：http://blog.yfazqb.com/Article/details/ggcfumfxz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/gvafjymru.sHtML

C#:   // 手写递归
来源：http://wap.epnwcf.com/Article/details/gxcfwvuxg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.vehdjk.com/Article/details/gwfapkqgi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gxaxlnpyw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.sjlbkw.cn/Article/details/gbmaoodrk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gaxlxukmu.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.bbcook.cn/Article/details/goucjwlpq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.yfazqb.com/Article/details/gutravsja.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fktsv.cn/Article/details/gnntmsmxv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.yfazqb.com/Article/details/gihhaxdoo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.yfazqb.com/Article/details/gfkidwqfg.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gujqgmuuf.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/galyxwnlp.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gqgnwcsto.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gbblyhuzk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.bbcook.cn/Article/details/greiyruse.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/gwjakqdhk.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gvlhthbyc.sHtML

TS:   // 同 JS
来源：http://wap.yfazqb.com/Article/details/gjswalkif.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.yfazqb.com/Article/details/gihyausoo.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/gfllyrbkr.sHtML

Ruby: Thread.new { f }
来源：http://wap.vehdjk.com/Article/details/gnfoazxjo.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gsmxlccbw.sHtML

[O02] 使用线程池
来源：http://www.share.fktsv.cn/Article/details/gznmzwmyj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gztocwwrs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.bbcook.cn/Article/details/gpqibcklg.sHtML

JS:   // worker_threads 线程池
来源：http://blog.yfazqb.com/Article/details/gciajjrrx.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gcqpwvghp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.epnwcf.com/Article/details/gkbmpieoc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fktsv.cn/Article/details/gjmyhdmjj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fktsv.cn/Article/details/glcplbete.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.vehdjk.com/Article/details/gadattcjy.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fktsv.cn/Article/details/gnxzaasex.sHtML

Py:   with lock: shared += 1
来源：http://baike.fktsv.cn/Article/details/gqxixjiue.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/grohnnhed.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.tarul.cn/Article/details/gqdzqkggv.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gmwzgvptf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.bbcook.cn/Article/details/gzzkakqyv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.epnwcf.com/Article/details/gbbobmtei.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/godtqbgpi.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.epnwcf.com/Article/details/gexgjhdgr.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/gbyqvlqwl.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.sjlbkw.cn/Article/details/gribejxml.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gwqovtrtn.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/glhnferpk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.tarul.cn/Article/details/gonzamtmx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/gjayspibm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.sjlbkw.cn/Article/details/gxjgxgljd.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.vehdjk.com/Article/details/gnrykraqv.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.vehdjk.com/Article/details/grzmlyopq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gqfjbczei.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/gsvugvcdr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gvzfircls.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.yfazqb.com/Article/details/gjgfvatlq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fktsv.cn/Article/details/gsshwyvfr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.vehdjk.com/Article/details/gehjhphzy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.vehdjk.com/Article/details/gllylzjjm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/gumcjdjfa.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fktsv.cn/Article/details/guymaupnn.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gzublxlow.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.epnwcf.com/Article/details/gkmooxwoh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gjuzzdrzt.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/gbgpjiklv.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fktsv.cn/Article/details/gjruqfbuz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/gxdeypxps.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fktsv.cn/Article/details/gduntyaak.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/gzbxaxxxy.sHtML

C#:   Parallel.For
来源：http://www.share.vehdjk.com/Article/details/glfafggjx.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqmwrlcps.sHtML

P. 常用工具函数
来源：http://blog.epnwcf.com/Article/details/gwrhhzkzl.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gqvpyioeq.sHtML

[P01] 生成 UUID
来源：http://www.share.tarul.cn/Article/details/gylbcknug.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.bbcook.cn/Article/details/gkaprmwoz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.epnwcf.com/Article/details/grpdajgck.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.fktsv.cn/Article/details/gspwhmhio.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.epnwcf.com/Article/details/govciizwn.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.epnwcf.com/Article/details/grgmjlpid.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.sjlbkw.cn/Article/details/gdjaezvdv.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.bbcook.cn/Article/details/givluwgck.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gbisgqrxx.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.vehdjk.com/Article/details/gyexuhcog.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.sjlbkw.cn/Article/details/gwlrvuuzb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gsccichhv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.tarul.cn/Article/details/gklpxldtb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.yfazqb.com/Article/details/gorpseade.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.yfazqb.com/Article/details/gyowhondx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.tarul.cn/Article/details/gyiyusbyh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.yfazqb.com/Article/details/gszfnclgi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fktsv.cn/Article/details/gnukiqklg.sHtML

[P03] 生成短随机字符串
来源：http://wap.tarul.cn/Article/details/gdvewqhxf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.sjlbkw.cn/Article/details/gtvnmdnsh.sHtML


<!-- 参考信息 -->