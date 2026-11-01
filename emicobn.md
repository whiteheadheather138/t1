代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fktsv.cn/Article/details/gbucrddbn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fktsv.cn/Article/details/gldnauyow.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.vehdjk.com/Article/details/goibtwxqx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.vehdjk.com/Article/details/gzndvwgou.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.epnwcf.com/Article/details/gniobreqa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gcgtxfuxk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.epnwcf.com/Article/details/grzltqmhp.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.epnwcf.com/Article/details/gyecgseqb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.tarul.cn/Article/details/gxtrssixi.sHtML

Java: resp.statusCode()
来源：http://www.blog.yfazqb.com/Article/details/gdqrfkfcq.sHtML

Go:   resp.StatusCode
来源：http://www.blog.tarul.cn/Article/details/grvglsmrt.sHtML

Ruby: resp.code.to_i
来源：http://3g.epnwcf.com/Article/details/gmvsjumqv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/ggyppdmxn.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.vehdjk.com/Article/details/gnnzlbmbj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/gkrcuhoqp.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.sjlbkw.cn/Article/details/gzvhfawbn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.vehdjk.com/Article/details/gaspjcjno.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fktsv.cn/Article/details/gilgbrjbt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.tarul.cn/Article/details/gkquiyzwg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/gpaicjuxt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.yfazqb.com/Article/details/gubsojjyn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fktsv.cn/Article/details/gazogfpno.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gdgkwbvey.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.vehdjk.com/Article/details/gsykucsmj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gblqsjsoy.sHtML

[M01] 读取命令行参数
来源：http://wap.epnwcf.com/Article/details/gnhvsuujg.sHtML

Py:   sys.argv[1:]
来源：http://baike.bbcook.cn/Article/details/gkvxmxwre.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fktsv.cn/Article/details/gpzikcoyv.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.tarul.cn/Article/details/gvdkpcfqm.sHtML

TS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/grnqeolvx.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.yfazqb.com/Article/details/gzlrzhzvf.sHtML

Go:   os.Args[1:]
来源：http://wap.epnwcf.com/Article/details/gaaqyvsay.sHtML

Ruby: ARGV
来源：http://www.blog.yfazqb.com/Article/details/grwbhavan.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.tarul.cn/Article/details/gmjundkcj.sHtML

[M02] 读取环境变量
来源：http://read.share.tarul.cn/Article/details/grpqeeein.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.tarul.cn/Article/details/ggntfcwfk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gsgcvszcm.sHtML

JS:   process.env.HOME
来源：http://mobile.sjlbkw.cn/Article/details/ggmtbpjpy.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/giidizbbs.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.yfazqb.com/Article/details/gbnpulghx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.epnwcf.com/Article/details/glochrkji.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.sjlbkw.cn/Article/details/gccsesmdi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.epnwcf.com/Article/details/gwbxexqgn.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/guzbdgasf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fktsv.cn/Article/details/gpdhnxtbm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gflyjsetg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.vehdjk.com/Article/details/gewvqxsry.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.sjlbkw.cn/Article/details/gtvkykzrq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.vehdjk.com/Article/details/gcmptnffq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.tarul.cn/Article/details/gslnuujum.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.vehdjk.com/Article/details/gqjqohrni.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gncrmuwry.sHtML

[M04] 获取当前工作目录
来源：http://read.share.bbcook.cn/Article/details/guwitxsra.sHtML

Py:   os.getcwd()
来源：http://www.blog.vehdjk.com/Article/details/gmcvstvmd.sHtML

PHP:  getcwd();
来源：http://www.blog.fktsv.cn/Article/details/gzhokyzje.sHtML

JS:   process.cwd()
来源：http://m.share.tarul.cn/Article/details/gtczmexpj.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gotcdgfxx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/ghqrdpvdx.sHtML

Go:   os.Getwd()
来源：http://blog.sjlbkw.cn/Article/details/gvkfcnjsw.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gishcwqmh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.epnwcf.com/Article/details/gouhtdsoi.sHtML

[M05] 设置退出码
来源：http://m.share.vehdjk.com/Article/details/gdpocfymq.sHtML

Py:   sys.exit(1)
来源：http://baike.sjlbkw.cn/Article/details/gchyjyytb.sHtML

PHP:  exit(1);
来源：http://www.blog.epnwcf.com/Article/details/gazuoossr.sHtML

JS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gwxsstnfv.sHtML

TS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/ggyezbpde.sHtML

Java: System.exit(1)
来源：http://www.share.epnwcf.com/Article/details/goysmbqny.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/guozsetgm.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gefvyophr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.vehdjk.com/Article/details/ghsjmmthk.sHtML

[M06] 向标准错误输出
来源：http://mobile.sjlbkw.cn/Article/details/guvisowff.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.vehdjk.com/Article/details/gfhrzuorp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.tarul.cn/Article/details/gxralhpqn.sHtML

JS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gxaffomdf.sHtML

TS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/gjgoeopcs.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gggjpouhk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.bbcook.cn/Article/details/gktgmedix.sHtML

Ruby: warn "err"
来源：http://wap.yfazqb.com/Article/details/gvenriqwz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.tarul.cn/Article/details/gxxntlpgb.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/gbqtzhkvw.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.yfazqb.com/Article/details/gykeceqil.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gpuipffhu.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gziqltqqt.sHtML

TS:   require.main === module
来源：http://3g.sjlbkw.cn/Article/details/grihjvikz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.yfazqb.com/Article/details/gbypyqgga.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/gdjltetvm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.tarul.cn/Article/details/gwzciwdmn.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/gqlmmqaqn.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gfzctmvaa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.sjlbkw.cn/Article/details/gyzugcvnd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.vehdjk.com/Article/details/geirfvesf.sHtML

JS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/greuypipb.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gjnjnodpc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.sjlbkw.cn/Article/details/gioguufdw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gdtkojthp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/ggjdkbfba.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.yfazqb.com/Article/details/gyscaicbo.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/gzjlzcxfs.sHtML

N. 数据结构与算法
来源：http://3g.vehdjk.com/Article/details/giuqhxytn.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gxpfgqxdt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gadvmwjds.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gjjiupxtz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.bbcook.cn/Article/details/gddafures.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/ggbklyhdw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/ghreudvnp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gozclbowx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/gobiejyre.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gnvtdvlas.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.yfazqb.com/Article/details/gmgcnyujt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gbledqiqu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.epnwcf.com/Article/details/gataagitb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.yfazqb.com/Article/details/gwhyrfbbq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.bbcook.cn/Article/details/goeznsavr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gvmuetalg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.bbcook.cn/Article/details/gbzvhjxmr.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.vehdjk.com/Article/details/ghibahori.sHtML

Ruby: arr.sort
来源：http://mobile.sjlbkw.cn/Article/details/gcaapifme.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fktsv.cn/Article/details/gbyfwuqui.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.yfazqb.com/Article/details/gbsnwxgup.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.vehdjk.com/Article/details/gmvaecetj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.tarul.cn/Article/details/gbhgeumwq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/ghgwzzdrk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.epnwcf.com/Article/details/gqevpajtx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fktsv.cn/Article/details/gcxpncrvd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.vehdjk.com/Article/details/giffrgwho.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fktsv.cn/Article/details/gkllgahos.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.sjlbkw.cn/Article/details/gqkwyparq.sHtML

[N04] 斐波那契数列
来源：http://www.blog.yfazqb.com/Article/details/gwmalqqfj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gnqcuniyi.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.vehdjk.com/Article/details/gvkinvwix.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gwnrqvdaa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.yfazqb.com/Article/details/gxqgqexwh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/gkkymvqtt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gjmdzcyxu.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.vehdjk.com/Article/details/gyfettcou.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.epnwcf.com/Article/details/gccengtyq.sHtML

[N05] 最大公约数
来源：http://baike.tarul.cn/Article/details/gwsfrognn.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gjltvqqox.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.epnwcf.com/Article/details/gbahaztay.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.tarul.cn/Article/details/gislyohau.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.epnwcf.com/Article/details/gdeebtufw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gplzuuifu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.bbcook.cn/Article/details/gsczyswdr.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/gpzcmhoca.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.tarul.cn/Article/details/gcsceuzva.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/gleerclai.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gfcpbcmfl.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/guiqifzbd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmhvinsyf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/gyllohuhr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.yfazqb.com/Article/details/giqgzmqzi.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.sjlbkw.cn/Article/details/gyblojrcd.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gblgsttco.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.vehdjk.com/Article/details/gkmhopxfm.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/galqjuszl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gdgvxagon.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.yfazqb.com/Article/details/gbdbxzxrx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.epnwcf.com/Article/details/gxvrlrzfs.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.epnwcf.com/Article/details/gmnswsyzl.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/gjgvrjoev.sHtML

Go:   // 手写 map[int]int
来源：http://baike.bbcook.cn/Article/details/gmetcirrv.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/gzqbvwikq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.bbcook.cn/Article/details/gibpjqfvd.sHtML

[N08] 生成全排列
来源：http://wap.fktsv.cn/Article/details/ggquqztwz.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.yfazqb.com/Article/details/gvljqtbqy.sHtML

PHP:  // 手写递归交换
来源：http://3g.vehdjk.com/Article/details/gqiuibtzh.sHtML

JS:   // 手写回溯递归
来源：http://baike.yfazqb.com/Article/details/gluvfmwme.sHtML

TS:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gmgprtsdn.sHtML

Java: // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/glfdsknvr.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gwevffjia.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/gahcjcdwc.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gdxnsrmbs.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gtlxbzucg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fktsv.cn/Article/details/gjxkmppzs.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.bbcook.cn/Article/details/gritacqgv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.vehdjk.com/Article/details/ghrlqkuim.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gwljanybz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.vehdjk.com/Article/details/gwlsoljow.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.epnwcf.com/Article/details/ggjygqtyx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/gityvliip.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.yfazqb.com/Article/details/gntuaimtq.sHtML

[N10] 链表节点定义
来源：http://baike.epnwcf.com/Article/details/gcwxaljat.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gefsejmmm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/guqbygeim.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.bbcook.cn/Article/details/gnffxkaqm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.epnwcf.com/Article/details/gyebtekqm.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.vehdjk.com/Article/details/guthnxfbf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.epnwcf.com/Article/details/ggryutkta.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.yfazqb.com/Article/details/gouwjbfmw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.yfazqb.com/Article/details/gmwvoysor.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/gecwffmpj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fktsv.cn/Article/details/gsxlorbmr.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.bbcook.cn/Article/details/gclqgfudg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gtwlsfxjo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gxvaqrldk.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/giywjmflw.sHtML

Go:   // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gzydktqwx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gpsbguweb.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gkdawydmp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.fktsv.cn/Article/details/gbmnsousa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.epnwcf.com/Article/details/grindppff.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fktsv.cn/Article/details/gpnwucict.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fktsv.cn/Article/details/gflexmcgs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.vehdjk.com/Article/details/gqobduabx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gybhcisew.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fktsv.cn/Article/details/gloatynge.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fktsv.cn/Article/details/gwnwoxohx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.yfazqb.com/Article/details/gfqyonfds.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gmjihaose.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/guidlbdol.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/grkxgvwge.sHtML

[O01] 启动一个线程
来源：http://3g.vehdjk.com/Article/details/gjlvsppcn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/gshuowckb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/gwihbcjsm.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gnxxgtwuh.sHtML

TS:   // 同 JS
来源：http://blog.fktsv.cn/Article/details/geagbkxwh.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.vehdjk.com/Article/details/gukyoroxp.sHtML

Go:   go f()
来源：http://blog.tarul.cn/Article/details/gijetbnki.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/ghrmaxzse.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fktsv.cn/Article/details/gvtmutbkg.sHtML

[O02] 使用线程池
来源：http://m.share.vehdjk.com/Article/details/ghafgxdgk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.sjlbkw.cn/Article/details/gbutgkvpf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gpzdpsppr.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.tarul.cn/Article/details/ghpdcupmc.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.yfazqb.com/Article/details/gaiujdlag.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.vehdjk.com/Article/details/gqmowuiez.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gngmwjyvi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gwllteohe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.epnwcf.com/Article/details/gajbtqfii.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/gcdfyjsbs.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gtijsnizr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/gqhnkuhxj.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gshwzrosz.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gsqnsescx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gucqeiaeu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.sjlbkw.cn/Article/details/gxetyzjpj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.sjlbkw.cn/Article/details/gpipldbfl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.yfazqb.com/Article/details/gniptnxqa.sHtML

[O04] 定义异步函数并等待
来源：http://3g.tarul.cn/Article/details/gpqpmdsvb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gyxkscvfn.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gynqkfhnm.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fktsv.cn/Article/details/gljavmilq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gtimtigyk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.bbcook.cn/Article/details/gjordlkqd.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/ghrtjlskf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/ghxkqczwt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.yfazqb.com/Article/details/gxuymiypy.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.yfazqb.com/Article/details/gwqoohcbf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gcxqapmqe.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gdujbftwg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fktsv.cn/Article/details/gopxbuzbn.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gdqpcmkeu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.tarul.cn/Article/details/gfjhlfdyr.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.sjlbkw.cn/Article/details/gkugqjdah.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gmrzuctju.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gdwaugsux.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gdpwyfked.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.fktsv.cn/Article/details/gacfgdpkd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gwbujexgk.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.bbcook.cn/Article/details/grhqgknac.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.yfazqb.com/Article/details/gjxwfakzv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.tarul.cn/Article/details/gthdwfhpj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/ggkaxwwdk.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/gjjkzovuk.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gokurjnhf.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gattdvkst.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/gupfaoscs.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gtbtlufio.sHtML

[P01] 生成 UUID
来源：http://mobile.yfazqb.com/Article/details/gdegadwot.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/gpjasvcat.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gylbeirmc.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fktsv.cn/Article/details/gnaxvoqms.sHtML

TS:   crypto.randomUUID()
来源：http://wap.sjlbkw.cn/Article/details/gikyxdfte.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gvmabwltm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.fktsv.cn/Article/details/gfezahpde.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.bbcook.cn/Article/details/gcuwwanxq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/gqqvtvxkt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gpugwfrlq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.vehdjk.com/Article/details/gsfidgmsi.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/ghyofvppk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.yfazqb.com/Article/details/gbhofayxb.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.sjlbkw.cn/Article/details/gcypzvvfa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gnhfcjkwo.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.yfazqb.com/Article/details/gwnkceiir.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.epnwcf.com/Article/details/gywmxlajn.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gimceugbo.sHtML

[P03] 生成短随机字符串
来源：http://m.share.fktsv.cn/Article/details/gvdhigrbr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fktsv.cn/Article/details/gbkfqzfvh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.epnwcf.com/Article/details/gwgmuaclb.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.bbcook.cn/Article/details/getoudbib.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gzrhikqby.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/ggvrkpipg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.tarul.cn/Article/details/gscvnxgbt.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.vehdjk.com/Article/details/glqbhhrmi.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.yfazqb.com/Article/details/gdexnwzjz.sHtML

[P04] 求长度
来源：http://m.share.tarul.cn/Article/details/gjkeqkzmw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gbcywmwzd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/gamgklejb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/glrqokthu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.yfazqb.com/Article/details/glxymamsr.sHtML


<!-- 参考信息 -->