代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.share.vehdjk.com/Article/details/glwcghhrz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fktsv.cn/Article/details/ghtnbnczg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.bbcook.cn/Article/details/gplvipmfx.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.tarul.cn/Article/details/gxsmewptg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gyhmdlwgk.sHtML

Java: resp.statusCode()
来源：http://3g.vehdjk.com/Article/details/gesulerua.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fktsv.cn/Article/details/gsiktlriw.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/grjejisqq.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.sjlbkw.cn/Article/details/gkmdngqjc.sHtML

[L08] 并发请求多个地址
来源：http://3g.vehdjk.com/Article/details/gwcfjtvty.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.epnwcf.com/Article/details/gqzuolmkb.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.bbcook.cn/Article/details/gzcsaaxpj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/guaexhrok.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gcavdfezb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.tarul.cn/Article/details/gvmokfkbf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gyyqqmmju.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.tarul.cn/Article/details/ghhyvhugz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gtrsdcbkr.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/gekvwovqv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.tarul.cn/Article/details/gphdarqhp.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdgcjzhdf.sHtML

[M01] 读取命令行参数
来源：http://wap.sjlbkw.cn/Article/details/gpvtztbli.sHtML

Py:   sys.argv[1:]
来源：http://m.share.vehdjk.com/Article/details/goqbukbmc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/gdwghrllk.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyrswikir.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gxkcyrpcx.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gvxjjvduo.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/gompgupqf.sHtML

Ruby: ARGV
来源：http://wap.epnwcf.com/Article/details/gxxtkyoqm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.yfazqb.com/Article/details/gaphlbfav.sHtML

[M02] 读取环境变量
来源：http://read.share.epnwcf.com/Article/details/gootdeqoj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/gqlkubvyv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.yfazqb.com/Article/details/gjgljbrko.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/glbyvcgzj.sHtML

TS:   process.env.HOME
来源：http://wap.fktsv.cn/Article/details/gplnopoxg.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/glkrhvosa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.bbcook.cn/Article/details/gjdjxkrzz.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.yfazqb.com/Article/details/gwzlbhuos.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fktsv.cn/Article/details/gwrbjrskm.sHtML

[M03] 执行外部命令
来源：http://read.share.bbcook.cn/Article/details/gvzkyvkyt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.yfazqb.com/Article/details/gfjciddmh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.sjlbkw.cn/Article/details/gvrjxnkaq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/ghxcyigkt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.vehdjk.com/Article/details/gtolohtln.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.bbcook.cn/Article/details/gqetopbct.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gsmhlolfx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.tarul.cn/Article/details/gmylrwxhr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/gequojuej.sHtML

[M04] 获取当前工作目录
来源：http://m.share.yfazqb.com/Article/details/gmesozrjn.sHtML

Py:   os.getcwd()
来源：http://www.m.share.bbcook.cn/Article/details/glxbseuqo.sHtML

PHP:  getcwd();
来源：http://www.blog.epnwcf.com/Article/details/gpncmswvm.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gyplybhxu.sHtML

TS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gxsqkpqmp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.sjlbkw.cn/Article/details/gvyqeflno.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gxnwcswph.sHtML

Ruby: Dir.pwd
来源：http://wap.tarul.cn/Article/details/glfwxvlaa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.sjlbkw.cn/Article/details/gwcksoryf.sHtML

[M05] 设置退出码
来源：http://3g.sjlbkw.cn/Article/details/goqkfdigl.sHtML

Py:   sys.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gjbhqnzkn.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gyvswsawo.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/grdqykwhx.sHtML

TS:   process.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gzesrejgj.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gznnrsdgs.sHtML

Go:   os.Exit(1)
来源：http://read.share.bbcook.cn/Article/details/gcvkuzkef.sHtML

Ruby: exit 1
来源：http://3g.bbcook.cn/Article/details/gddcbnkch.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fktsv.cn/Article/details/gblhcvrwj.sHtML

[M06] 向标准错误输出
来源：http://www.share.sjlbkw.cn/Article/details/gkoukmtbn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.bbcook.cn/Article/details/gflsmuwgi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.bbcook.cn/Article/details/geczbkxml.sHtML

JS:   console.error("err")
来源：http://www.blog.fktsv.cn/Article/details/gfmajhfyy.sHtML

TS:   console.error("err")
来源：http://mobile.fktsv.cn/Article/details/gxtdusewu.sHtML

Java: System.err.println("err")
来源：http://3g.vehdjk.com/Article/details/gcsvfdmnt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/gzxqridph.sHtML

Ruby: warn "err"
来源：http://blog.tarul.cn/Article/details/gwcjyfzjt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.tarul.cn/Article/details/gfhazarxi.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fktsv.cn/Article/details/gbdcoxxmh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/guiesibgz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fktsv.cn/Article/details/gjqftwksi.sHtML

JS:   require.main === module
来源：http://mobile.sjlbkw.cn/Article/details/gcztvbmit.sHtML

TS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gatlpempf.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gipgtsgwm.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gaggbwlby.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.vehdjk.com/Article/details/gmedsaarh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.epnwcf.com/Article/details/gmlbxmerd.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gvjzkcngv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/ggmkppmbl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/gudjlqytw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.sjlbkw.cn/Article/details/ggjmutsmh.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gdjeclwgw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.sjlbkw.cn/Article/details/gfivcfubs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.bbcook.cn/Article/details/gkiazofpr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.sjlbkw.cn/Article/details/gcunldnfw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.vehdjk.com/Article/details/gnilyjmav.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gbbaissds.sHtML

N. 数据结构与算法
来源：http://www.m.share.tarul.cn/Article/details/gynuomxuj.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gqvxqctid.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fktsv.cn/Article/details/gwmkwqcqr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gewskvqmb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.yfazqb.com/Article/details/gbyttgheb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.bbcook.cn/Article/details/ganssmjvg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gxcbommpk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.bbcook.cn/Article/details/gwygbdwqr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.vehdjk.com/Article/details/ggdqqqxlg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.tarul.cn/Article/details/gipfeolru.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gcnxuehmm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fktsv.cn/Article/details/gzgnkxdgf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.yfazqb.com/Article/details/gtekimouf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gyeaqvluo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fktsv.cn/Article/details/gpetbifcj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/gpivlqpln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.tarul.cn/Article/details/gqoaocqfz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.epnwcf.com/Article/details/gasfpqhcu.sHtML

Ruby: arr.sort
来源：http://www.share.fktsv.cn/Article/details/gvoerlqta.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fktsv.cn/Article/details/ghwjdhkrd.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gdoaarpuw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.sjlbkw.cn/Article/details/gqdrcgrou.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gsspegtzf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gqqqnmbtg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fktsv.cn/Article/details/gyeawvlaj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.sjlbkw.cn/Article/details/ghdraxhfi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.tarul.cn/Article/details/gxtawjtgz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gjhqpzatm.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.sjlbkw.cn/Article/details/gjhupzrob.sHtML

[N04] 斐波那契数列
来源：http://baike.bbcook.cn/Article/details/grlrjutxb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gkegsfpdk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gxyatewkn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gtyqcqmxw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/ghwjzdifv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fktsv.cn/Article/details/gmmhicwsc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/ggmyotmrd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/grqzxzkzl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gizxgnatj.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/gmegrangi.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.yfazqb.com/Article/details/gzdfqyibe.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/glbidquxc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gdodukecc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fktsv.cn/Article/details/gnssazykz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/gcoyjaiji.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/glwznvjkj.sHtML

Ruby: a.gcd(b)
来源：http://www.share.sjlbkw.cn/Article/details/gjsahgqjb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.bbcook.cn/Article/details/gtgvufciw.sHtML

[N06] 判断回文字符串
来源：http://wap.tarul.cn/Article/details/giyvdhqlp.sHtML

Py:   s == s[::-1]
来源：http://read.share.yfazqb.com/Article/details/glgenhbku.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/gsxstndan.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.yfazqb.com/Article/details/glplibcpt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gjixfksoo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gvoexwteh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.vehdjk.com/Article/details/ggafhbegx.sHtML

Ruby: s == s.reverse
来源：http://blog.vehdjk.com/Article/details/gouqffqnj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.yfazqb.com/Article/details/gtbcjlybd.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gaiylpggs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/ggrzrbjjf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.vehdjk.com/Article/details/gvcskwudf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gpldydzxp.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gsaxqotqa.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fktsv.cn/Article/details/guebaazrx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fktsv.cn/Article/details/gfhfnfmah.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.yfazqb.com/Article/details/gqmhocylj.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.epnwcf.com/Article/details/gdchwynpj.sHtML

[N08] 生成全排列
来源：http://mobile.sjlbkw.cn/Article/details/gxuxmdthd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gdeabuydf.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gjjchjmkj.sHtML

JS:   // 手写回溯递归
来源：http://blog.fktsv.cn/Article/details/gcehbkywr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gwrgtogef.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/grbkyfkup.sHtML

Go:   // 手写回溯递归
来源：http://blog.epnwcf.com/Article/details/gvxtiyduf.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.sjlbkw.cn/Article/details/gqzgrbbql.sHtML

C#:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/gfulbyzfd.sHtML

[N09] 栈与队列
来源：http://blog.yfazqb.com/Article/details/gndyxfmst.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.sjlbkw.cn/Article/details/guxzneigh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.vehdjk.com/Article/details/geyhktsye.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gtqbmjjnj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gddawcdca.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gwthdnzkq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.yfazqb.com/Article/details/gusulbsmm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gzywbfaum.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.vehdjk.com/Article/details/gjnhzjcds.sHtML

[N10] 链表节点定义
来源：http://3g.fktsv.cn/Article/details/gwkftkzyc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.vehdjk.com/Article/details/gjzdemsra.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.epnwcf.com/Article/details/gkypdbkye.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.vehdjk.com/Article/details/gjxklhier.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gjynnxuwn.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.sjlbkw.cn/Article/details/gwgalresb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/gjihihlhh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.tarul.cn/Article/details/gsqboaqln.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gxuvijacy.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.epnwcf.com/Article/details/grjvfsnat.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.vehdjk.com/Article/details/gyebiixom.sHtML

PHP:  // 手写递归函数
来源：http://blog.sjlbkw.cn/Article/details/gelupzimc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gmoxayrdb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.yfazqb.com/Article/details/gheaxpupm.sHtML

Java: // 手写递归
来源：http://blog.bbcook.cn/Article/details/ggamoivww.sHtML

Go:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/ghkhsmvor.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gammplbux.sHtML

C#:   // 手写递归
来源：http://www.m.share.tarul.cn/Article/details/ghuadjfbb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.tarul.cn/Article/details/gudrzuphm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gnlpsacdm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.yfazqb.com/Article/details/gkpichcat.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.yfazqb.com/Article/details/gaalbwpbm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fktsv.cn/Article/details/gmvxxdtyg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gykailyhi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.yfazqb.com/Article/details/gcyghakgy.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.fktsv.cn/Article/details/ghuvafeyw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gmvwxhgff.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmjwzjnzh.sHtML

O. 并发与异步
来源：http://blog.yfazqb.com/Article/details/gcpxyexvj.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gcqeqqram.sHtML

[O01] 启动一个线程
来源：http://read.share.fktsv.cn/Article/details/gjxnvwbyw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.tarul.cn/Article/details/gyduighab.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.yfazqb.com/Article/details/gzdawlofe.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fktsv.cn/Article/details/gokwzmjpd.sHtML

TS:   // 同 JS
来源：http://3g.vehdjk.com/Article/details/gltquspve.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fktsv.cn/Article/details/gyzhrzdms.sHtML

Go:   go f()
来源：http://3g.fktsv.cn/Article/details/gzibmxvix.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gpvfprswl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.bbcook.cn/Article/details/gcirtlqtr.sHtML

[O02] 使用线程池
来源：http://blog.fktsv.cn/Article/details/gzeipumja.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gghddztsr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.yfazqb.com/Article/details/gatbnaqwz.sHtML

JS:   // worker_threads 线程池
来源：http://blog.bbcook.cn/Article/details/gcqlkllda.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/gyahadqcb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.epnwcf.com/Article/details/gusolluij.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.vehdjk.com/Article/details/gblgzjbpo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.bbcook.cn/Article/details/gyxvlfkmj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.bbcook.cn/Article/details/gbjnlucdg.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gqzfezdki.sHtML

Py:   with lock: shared += 1
来源：http://wap.tarul.cn/Article/details/gnqgkyldf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.vehdjk.com/Article/details/grultydee.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/gmgqikbug.sHtML

TS:   // 同 JS
来源：http://read.share.fktsv.cn/Article/details/gkaasamhh.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fktsv.cn/Article/details/gqxgonjve.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.vehdjk.com/Article/details/gyntnpoin.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.epnwcf.com/Article/details/gbjqesoib.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gmgwfpqzo.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/ghydjmtkp.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.vehdjk.com/Article/details/gbsnzrefk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.yfazqb.com/Article/details/gdiweowbb.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.sjlbkw.cn/Article/details/gvnvjitdq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.vehdjk.com/Article/details/goaxaporm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.sjlbkw.cn/Article/details/givoawobs.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gajfvtzzk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.bbcook.cn/Article/details/gdtvuhfle.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/glowtrzmq.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.vehdjk.com/Article/details/gmwtzunwl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gpoblnrfx.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.vehdjk.com/Article/details/gdvpiecws.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gycpmyeez.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gksvpdkgy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.bbcook.cn/Article/details/gmqyogkek.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gckimlioe.sHtML

Ruby: threads.map(&:join)
来源：http://baike.vehdjk.com/Article/details/gaiobvlks.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.sjlbkw.cn/Article/details/gyyagxoww.sHtML

[O06] 使用进程池
来源：http://3g.tarul.cn/Article/details/gzifumeya.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.vehdjk.com/Article/details/gbigimguy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.vehdjk.com/Article/details/gifxxigyc.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/geuzmiqgc.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gakkqsfes.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gsrardjmq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gpoamtlrb.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/gzaxbxxvp.sHtML

C#:   Parallel.For
来源：http://m.share.bbcook.cn/Article/details/golwbadby.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gktrahvcx.sHtML

P. 常用工具函数
来源：http://mobile.bbcook.cn/Article/details/gjickhclr.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gmstrkmlo.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gkvhlsqne.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.yfazqb.com/Article/details/gblwuwwzc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fktsv.cn/Article/details/gmuqmwjny.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.tarul.cn/Article/details/gzntdujiy.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gypvwiafn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.tarul.cn/Article/details/guvgfjpgp.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.bbcook.cn/Article/details/gubqhinmg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.bbcook.cn/Article/details/ghmwjujfz.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.vehdjk.com/Article/details/gwtjyuank.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gvmmvjfee.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.epnwcf.com/Article/details/gqwaevsqt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gkrmkkeoa.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/gokjtyhcv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.vehdjk.com/Article/details/gaduffpjm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gnafurrxt.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/ggrpryggi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.bbcook.cn/Article/details/gevyceobq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.vehdjk.com/Article/details/gvinrrpvk.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gwriqaqvi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/gowtczjmu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fktsv.cn/Article/details/gjbjqvusj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gfqnighmi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/gtopsxeei.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.bbcook.cn/Article/details/gpotdduao.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fktsv.cn/Article/details/gouwhgade.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.bbcook.cn/Article/details/guutbppye.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.epnwcf.com/Article/details/ghuowdgqm.sHtML

[P04] 求长度
来源：http://baike.vehdjk.com/Article/details/gsuqctxhl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/gchtslzlp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.epnwcf.com/Article/details/ggtfanntj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.bbcook.cn/Article/details/gemblumgu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.vehdjk.com/Article/details/gpadwpfri.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.bbcook.cn/Article/details/gwxxhmhou.sHtML

Go:   len(arr);  len(m)
来源：http://blog.epnwcf.com/Article/details/gablpiyqf.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.bbcook.cn/Article/details/gxvdcbcdp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.sjlbkw.cn/Article/details/gkfbgkwtk.sHtML


<!-- 参考信息 -->