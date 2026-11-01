代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.epnwcf.com/Article/details/gginenosh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.sjlbkw.cn/Article/details/gmuxzklfk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.tarul.cn/Article/details/gzczzdmtv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fktsv.cn/Article/details/guacwhbvq.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.vehdjk.com/Article/details/gxbkpenua.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.bbcook.cn/Article/details/gwoktfzpj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.epnwcf.com/Article/details/gjgequimd.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.yfazqb.com/Article/details/gqftjgokr.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.epnwcf.com/Article/details/gqowmguns.sHtML

Java: resp.statusCode()
来源：http://blog.yfazqb.com/Article/details/gqtvfgntl.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.vehdjk.com/Article/details/gpqrsarag.sHtML

Ruby: resp.code.to_i
来源：http://baike.epnwcf.com/Article/details/glrmwiqho.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.tarul.cn/Article/details/gfnhwukkw.sHtML

[L08] 并发请求多个地址
来源：http://wap.sjlbkw.cn/Article/details/gatmmqmxq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.sjlbkw.cn/Article/details/gohwdhxww.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.tarul.cn/Article/details/gqzupsxdy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gceuhbryd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.yfazqb.com/Article/details/guowltfzo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.bbcook.cn/Article/details/gfodsfmlx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.yfazqb.com/Article/details/ggbwonugy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fktsv.cn/Article/details/gktsqcxrv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.epnwcf.com/Article/details/gnsvzjawe.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gjxnnyhlu.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.bbcook.cn/Article/details/gtlofbxdn.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gmsywpbsy.sHtML

[M01] 读取命令行参数
来源：http://blog.tarul.cn/Article/details/gaoprexih.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/grcrsrqvy.sHtML

PHP:  $argv;  $argc;
来源：http://wap.bbcook.cn/Article/details/gppubxsxg.sHtML

JS:   process.argv.slice(2)
来源：http://wap.epnwcf.com/Article/details/gyzfwqxvr.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.vehdjk.com/Article/details/gonukmvuw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.yfazqb.com/Article/details/gmlxmxikj.sHtML

Go:   os.Args[1:]
来源：http://baike.tarul.cn/Article/details/gygfkwivp.sHtML

Ruby: ARGV
来源：http://www.blog.sjlbkw.cn/Article/details/ggttodlbj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.bbcook.cn/Article/details/gujeoahre.sHtML

[M02] 读取环境变量
来源：http://mobile.vehdjk.com/Article/details/ghtmsdzck.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gfefbaeqf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.yfazqb.com/Article/details/gtvcohqtu.sHtML

JS:   process.env.HOME
来源：http://www.blog.yfazqb.com/Article/details/gjfgxacxh.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gevcllxqw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.sjlbkw.cn/Article/details/gqbtpuvvg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gstajdwtl.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gychuujzk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.vehdjk.com/Article/details/gsoaltiml.sHtML

[M03] 执行外部命令
来源：http://baike.bbcook.cn/Article/details/gsjsdxawb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.vehdjk.com/Article/details/gozulallu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gzifzktrp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gvcmlwtbp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gfcdumdli.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.yfazqb.com/Article/details/gdrnpzfou.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.yfazqb.com/Article/details/gfcqgqlky.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.tarul.cn/Article/details/gpsbrfoqz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.tarul.cn/Article/details/gpqgekcun.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/gpjrsvkki.sHtML

Py:   os.getcwd()
来源：http://read.share.tarul.cn/Article/details/gdsldccyt.sHtML

PHP:  getcwd();
来源：http://m.share.bbcook.cn/Article/details/gnnfjalrt.sHtML

JS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gajibjbbi.sHtML

TS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/gvknutzta.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.bbcook.cn/Article/details/gsjapncro.sHtML

Go:   os.Getwd()
来源：http://mobile.epnwcf.com/Article/details/gpugjtvxd.sHtML

Ruby: Dir.pwd
来源：http://3g.vehdjk.com/Article/details/glnefhlyo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/gjaxvnsgv.sHtML

[M05] 设置退出码
来源：http://read.share.sjlbkw.cn/Article/details/gjbhufttz.sHtML

Py:   sys.exit(1)
来源：http://read.share.vehdjk.com/Article/details/gybaqdpxl.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gkngnhmhc.sHtML

JS:   process.exit(1)
来源：http://blog.sjlbkw.cn/Article/details/gizearxgt.sHtML

TS:   process.exit(1)
来源：http://www.share.yfazqb.com/Article/details/glmfzyzab.sHtML

Java: System.exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gghfhzozp.sHtML

Go:   os.Exit(1)
来源：http://wap.epnwcf.com/Article/details/gckiqchhr.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gpefpyymz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gxpggodlg.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gepvoybgn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.bbcook.cn/Article/details/geagoydjo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fktsv.cn/Article/details/ggcduzmgp.sHtML

JS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gneaiqnbk.sHtML

TS:   console.error("err")
来源：http://www.share.vehdjk.com/Article/details/goxhnbjzn.sHtML

Java: System.err.println("err")
来源：http://read.share.tarul.cn/Article/details/gctzipsvd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.bbcook.cn/Article/details/gpzgtkbzt.sHtML

Ruby: warn "err"
来源：http://blog.fktsv.cn/Article/details/gimqvzsei.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.yfazqb.com/Article/details/gnfdvbajg.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.tarul.cn/Article/details/gcwphvuyq.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gzsiwryqk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.sjlbkw.cn/Article/details/grkfhnyoh.sHtML

JS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/grxfnwasz.sHtML

TS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gtrfkmjmu.sHtML

Java: public static void main(String[] args)
来源：http://www.share.vehdjk.com/Article/details/gcpovaijs.sHtML

Go:   func main()
来源：http://3g.vehdjk.com/Article/details/gpbomhmet.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/gmvjzbdks.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.epnwcf.com/Article/details/gmrxvxxpv.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.bbcook.cn/Article/details/grkpmbgbt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.epnwcf.com/Article/details/gqfamdxoi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gmkprtuhf.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/ggjsmvzfn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gxgyfygua.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.vehdjk.com/Article/details/gtdaxlxnx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fktsv.cn/Article/details/gpsgiwbtc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/gwlybuing.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/geeckvgbd.sHtML

================================================================================
来源：http://www.share.bbcook.cn/Article/details/guaxcegzt.sHtML

N. 数据结构与算法
来源：http://www.blog.fktsv.cn/Article/details/ggtasktol.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gabbhwlfp.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.yfazqb.com/Article/details/gvwzgtyos.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fktsv.cn/Article/details/ghzfpmjug.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gjkbsemsv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gdupfyygq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.yfazqb.com/Article/details/gjgdcognv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.vehdjk.com/Article/details/gdeahzoml.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.tarul.cn/Article/details/geticzwxa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.sjlbkw.cn/Article/details/glnziqvbi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gmtkgursv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gnucqbodh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.bbcook.cn/Article/details/gwenwuvru.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.yfazqb.com/Article/details/gheqpzmni.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.sjlbkw.cn/Article/details/gtbmdyjho.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fktsv.cn/Article/details/gcioqfpot.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.bbcook.cn/Article/details/gvgaglmwi.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.bbcook.cn/Article/details/gfjbrlnda.sHtML

Ruby: arr.sort
来源：http://wap.fktsv.cn/Article/details/gzqcipqok.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.yfazqb.com/Article/details/gawjbouvr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gvghpflla.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.yfazqb.com/Article/details/gyjzulidb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gueeietmy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.epnwcf.com/Article/details/ghcptczgz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.tarul.cn/Article/details/gmjobdinx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.epnwcf.com/Article/details/gpljktfdt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.sjlbkw.cn/Article/details/gxvkzdyhv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.vehdjk.com/Article/details/gpixjeiln.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.fktsv.cn/Article/details/gsqvqmbho.sHtML

[N04] 斐波那契数列
来源：http://wap.fktsv.cn/Article/details/goadswcai.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.sjlbkw.cn/Article/details/gpopomqwt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.epnwcf.com/Article/details/gpdlocxpd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gmxpxrhhr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gpdqkqsvq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.epnwcf.com/Article/details/gazoydcyf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.vehdjk.com/Article/details/gmjhcznfd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.epnwcf.com/Article/details/gjljgyjwf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.fktsv.cn/Article/details/gcvomtfzl.sHtML

[N05] 最大公约数
来源：http://www.m.share.vehdjk.com/Article/details/gfgwptmai.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/govumuzzh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.bbcook.cn/Article/details/gutpwnnep.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gsgyfgotj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gouadtsip.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.vehdjk.com/Article/details/gfuggyxde.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.sjlbkw.cn/Article/details/gpmwnycfq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/gdfqwteqf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.bbcook.cn/Article/details/gzcnaggys.sHtML

[N06] 判断回文字符串
来源：http://read.share.epnwcf.com/Article/details/gfxpaxonc.sHtML

Py:   s == s[::-1]
来源：http://www.blog.bbcook.cn/Article/details/ghsueryku.sHtML

PHP:  $s === strrev($s);
来源：http://wap.epnwcf.com/Article/details/gzgkomuhq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gglrtronp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fktsv.cn/Article/details/gotugknnv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fktsv.cn/Article/details/gudrqimjx.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.epnwcf.com/Article/details/gghubzwuj.sHtML

Ruby: s == s.reverse
来源：http://m.share.bbcook.cn/Article/details/gjoupnlac.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.tarul.cn/Article/details/gbghcjhrx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.tarul.cn/Article/details/gpvhusxtn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.bbcook.cn/Article/details/gytigcvkm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.sjlbkw.cn/Article/details/gnpyfebgv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gulrtptrd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.sjlbkw.cn/Article/details/gldixcgux.sHtML

Java: // 手写 HashMap
来源：http://www.blog.vehdjk.com/Article/details/gdjgecuzj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fktsv.cn/Article/details/gjbijjluf.sHtML

Ruby: // 手写 Hash
来源：http://www.share.sjlbkw.cn/Article/details/ghmsouqbg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.vehdjk.com/Article/details/gnkxhmjtt.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/gmacbdyzd.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.sjlbkw.cn/Article/details/gqqqxfqgp.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/gpnbfpcqt.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/gfeuyyzdy.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.tarul.cn/Article/details/gkdxsowfm.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gadlsrzxl.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gronlhdzq.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.yfazqb.com/Article/details/gfohoteit.sHtML

C#:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gfeubieky.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/ggcjdwcpk.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.epnwcf.com/Article/details/gzbehebwm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gkpuszyes.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.bbcook.cn/Article/details/ggsilxatx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/gbjijxklw.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.bbcook.cn/Article/details/guvbfsxsi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.vehdjk.com/Article/details/gtpldthie.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.tarul.cn/Article/details/glowtkkox.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.fktsv.cn/Article/details/gtzvgbegs.sHtML

[N10] 链表节点定义
来源：http://baike.tarul.cn/Article/details/grozfcffi.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gmqoinysn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.tarul.cn/Article/details/gnwjhvvyk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/gxtrwpqhw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.epnwcf.com/Article/details/gaepiwbvr.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.fktsv.cn/Article/details/ggpacaptk.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.bbcook.cn/Article/details/grfblilsk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fktsv.cn/Article/details/glbuycnmx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.bbcook.cn/Article/details/goxcfcxis.sHtML

[N11] 二叉树中序遍历
来源：http://baike.epnwcf.com/Article/details/gduehusbt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/ghaddzvxr.sHtML

PHP:  // 手写递归函数
来源：http://read.share.yfazqb.com/Article/details/gejoogpyi.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/giwcoyxet.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.tarul.cn/Article/details/guosflakj.sHtML

Java: // 手写递归
来源：http://www.share.tarul.cn/Article/details/gtvlalydp.sHtML

Go:   // 手写递归
来源：http://baike.yfazqb.com/Article/details/gmqodkudk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fktsv.cn/Article/details/gciuznaoj.sHtML

C#:   // 手写递归
来源：http://www.m.share.fktsv.cn/Article/details/gpafkfpph.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.bbcook.cn/Article/details/gncxupjem.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.epnwcf.com/Article/details/gxhmdfgzg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gkipwvmlw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/ggbtwpnhy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gglqsgrnj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fktsv.cn/Article/details/gzestmsyx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gbgoqujzo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gzidpvhzc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gdosdesli.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gbixtlkcw.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/gbuggwbcr.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gatfplnkx.sHtML

[O01] 启动一个线程
来源：http://mobile.epnwcf.com/Article/details/gcuueeool.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/gthxlkuue.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.sjlbkw.cn/Article/details/ggzitjpki.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gkcuyvdwd.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/grmxdbypb.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.yfazqb.com/Article/details/gctyfmzsi.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/gyqkvwopa.sHtML

Ruby: Thread.new { f }
来源：http://wap.bbcook.cn/Article/details/gendkjmio.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.tarul.cn/Article/details/ghrwmixjg.sHtML

[O02] 使用线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gayjhvpmq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gcdcmnhfj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.epnwcf.com/Article/details/gxpejxrtu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.sjlbkw.cn/Article/details/gksxsolfd.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/gchukjdqz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.fktsv.cn/Article/details/golbyjows.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.bbcook.cn/Article/details/gnzrfwofs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.epnwcf.com/Article/details/gmqzwmleo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gruxfxwms.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fktsv.cn/Article/details/gdzfczhag.sHtML

Py:   with lock: shared += 1
来源：http://mobile.epnwcf.com/Article/details/gdxzgmmnn.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.bbcook.cn/Article/details/gdnutcmdy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.vehdjk.com/Article/details/gkzxmffto.sHtML

TS:   // 同 JS
来源：http://www.blog.yfazqb.com/Article/details/gbqwqnphf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.vehdjk.com/Article/details/gpmlgmfxw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.epnwcf.com/Article/details/gszhmuoao.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fktsv.cn/Article/details/grzecvtbf.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/glpmokgcv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.epnwcf.com/Article/details/gmwarshiy.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gmggmroif.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.epnwcf.com/Article/details/gkttycbpn.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/gtaxbysxl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.tarul.cn/Article/details/gnzqohojn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/gfcydkzec.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.tarul.cn/Article/details/gatmyhkqs.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.vehdjk.com/Article/details/ghneoiwxi.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.yfazqb.com/Article/details/ghushkdap.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gewhiaumo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.tarul.cn/Article/details/gjxtfmsaz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gfcjfaema.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.epnwcf.com/Article/details/gbuzanfgy.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gccgjbzqh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.bbcook.cn/Article/details/gbazsyttt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.bbcook.cn/Article/details/gphmtqmky.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.yfazqb.com/Article/details/giwicfath.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/gkfamywhb.sHtML

[O06] 使用进程池
来源：http://read.share.tarul.cn/Article/details/gtbxdghut.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gnpqbruvm.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gednphqgx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gxtjyukje.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gatsumirh.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fktsv.cn/Article/details/gufweiomr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.sjlbkw.cn/Article/details/gugzugzbt.sHtML

Ruby: // fork 块
来源：http://www.m.share.fktsv.cn/Article/details/gjmkmzowg.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/gciysqltf.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsgbrsxpj.sHtML

P. 常用工具函数
来源：http://mobile.fktsv.cn/Article/details/gdglkmmar.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gxkuaoydj.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/gwbvforcc.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gjmlmlitz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gftovbrua.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.tarul.cn/Article/details/gjpjizefz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.vehdjk.com/Article/details/gcvujadog.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.vehdjk.com/Article/details/ghlbrspin.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gufzwaikl.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.bbcook.cn/Article/details/gxvqhppqj.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.vehdjk.com/Article/details/gmqbilfgv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/ggepyvgcb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gnzxbxrxn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.bbcook.cn/Article/details/gcmevwbbh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fktsv.cn/Article/details/ghnvnbozf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.sjlbkw.cn/Article/details/gahxgrmjc.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.bbcook.cn/Article/details/gdamgowcr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.yfazqb.com/Article/details/gwbtuiump.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.epnwcf.com/Article/details/gqfqmkuqq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/gbzoiogao.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fktsv.cn/Article/details/gomtqlmux.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gzjdrfixl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.vehdjk.com/Article/details/gpxplggpm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/ghyajoqpk.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.bbcook.cn/Article/details/gubeuquxz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/gohufyald.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/grapcgrnz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fktsv.cn/Article/details/ghjukbmdv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.bbcook.cn/Article/details/ggvzgstvp.sHtML

[P04] 求长度
来源：http://mobile.epnwcf.com/Article/details/gvavseyag.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.vehdjk.com/Article/details/gvfvroahy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fktsv.cn/Article/details/gbnqgzspv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.vehdjk.com/Article/details/gqvqiyizc.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.sjlbkw.cn/Article/details/gefgpbrql.sHtML


<!-- 参考信息 -->