代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.share.yfazqb.com/Article/details/gxzzieewj.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.epnwcf.com/Article/details/gcyxmopjw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.vehdjk.com/Article/details/gmpymigkp.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.epnwcf.com/Article/details/gcwyrnjbg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fktsv.cn/Article/details/gimxjqfde.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.epnwcf.com/Article/details/gbwrobtxy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fktsv.cn/Article/details/grtkoayty.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.epnwcf.com/Article/details/gqprxivdn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.bbcook.cn/Article/details/gkbsnxvoj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gyjuumohc.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gefmzucpc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.bbcook.cn/Article/details/ghrvyrgal.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gunxmdbeq.sHtML

[M01] 读取命令行参数
来源：http://blog.epnwcf.com/Article/details/gmspesacq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.bbcook.cn/Article/details/gincarles.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.vehdjk.com/Article/details/giugklzdw.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.vehdjk.com/Article/details/ghbbjevbt.sHtML

TS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gnziajrcx.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.epnwcf.com/Article/details/gzdgketkc.sHtML

Go:   os.Args[1:]
来源：http://read.share.tarul.cn/Article/details/gdrguvhrt.sHtML

Ruby: ARGV
来源：http://3g.fktsv.cn/Article/details/ghhkyedvi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gunehawdp.sHtML

[M02] 读取环境变量
来源：http://www.share.sjlbkw.cn/Article/details/gapbmdfcn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gctqwouou.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.sjlbkw.cn/Article/details/gwcfowkmr.sHtML

JS:   process.env.HOME
来源：http://blog.sjlbkw.cn/Article/details/gppiewlnl.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gnfddqefs.sHtML

Java: System.getenv("HOME")
来源：http://mobile.epnwcf.com/Article/details/galvjsiag.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.bbcook.cn/Article/details/gierwukro.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/gvyuabrgs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.yfazqb.com/Article/details/gneisgaux.sHtML

[M03] 执行外部命令
来源：http://3g.epnwcf.com/Article/details/glvizcdej.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.epnwcf.com/Article/details/gpcfhaugu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fktsv.cn/Article/details/gpbetlmoc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/gccmrnyxq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.epnwcf.com/Article/details/gdeorzfrv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/gzxauamhv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/gtnuoigvo.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.bbcook.cn/Article/details/gtdtnifey.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gzayhzzrx.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.epnwcf.com/Article/details/gbeubfhbx.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gzsklsbxt.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/gmgnvqubo.sHtML

JS:   process.cwd()
来源：http://www.m.share.vehdjk.com/Article/details/gbpoparyu.sHtML

TS:   process.cwd()
来源：http://m.share.yfazqb.com/Article/details/ghhrujclk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.epnwcf.com/Article/details/gjlzjjahc.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gbdrydjne.sHtML

Ruby: Dir.pwd
来源：http://3g.epnwcf.com/Article/details/gbvmrcjhp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/gfsitgnsz.sHtML

[M05] 设置退出码
来源：http://m.share.epnwcf.com/Article/details/gnbabxzkq.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gikwrmktu.sHtML

PHP:  exit(1);
来源：http://blog.epnwcf.com/Article/details/gpsucvhxr.sHtML

JS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/ggwyczphu.sHtML

TS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gtijduswj.sHtML

Java: System.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/grectsshb.sHtML

Go:   os.Exit(1)
来源：http://baike.tarul.cn/Article/details/gcphzdgsx.sHtML

Ruby: exit 1
来源：http://www.share.yfazqb.com/Article/details/glqyfsjjs.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.epnwcf.com/Article/details/gipxrwwlq.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gvfexeyyl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.sjlbkw.cn/Article/details/guwdozqjw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.yfazqb.com/Article/details/gbrvumbct.sHtML

JS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gioosjouw.sHtML

TS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gbguijqli.sHtML

Java: System.err.println("err")
来源：http://wap.fktsv.cn/Article/details/girnuwbqc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fktsv.cn/Article/details/gkermgtxt.sHtML

Ruby: warn "err"
来源：http://wap.sjlbkw.cn/Article/details/gufeijnnn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.tarul.cn/Article/details/gsgybysuw.sHtML

[M07] 判断是否为主入口
来源：http://baike.yfazqb.com/Article/details/gjbelpyco.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.tarul.cn/Article/details/gdczztvnv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.bbcook.cn/Article/details/gqxhctzta.sHtML

JS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/gwejkrcta.sHtML

TS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gqjcjckde.sHtML

Java: public static void main(String[] args)
来源：http://3g.tarul.cn/Article/details/gqswpsbig.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gynssuoby.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fktsv.cn/Article/details/gaaencsaj.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fktsv.cn/Article/details/galzcubzt.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.epnwcf.com/Article/details/gljnsbnvi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.bbcook.cn/Article/details/gwbwbapnd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.vehdjk.com/Article/details/guibfdnmk.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gtmjmwhym.sHtML

TS:   process.platform;  process.version
来源：http://blog.vehdjk.com/Article/details/guvrijrly.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/gezgpgphl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/gyrkncjum.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.tarul.cn/Article/details/gsoefhtea.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/gckqmpiad.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsbzxxyr.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gbwnygrhv.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/ghxbcmtso.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.yfazqb.com/Article/details/gbmapzhco.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gprvlebrr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.tarul.cn/Article/details/gxmxnsopa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/gqgfltgbp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gtcxamshv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/gvvywykgs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.epnwcf.com/Article/details/ginbaolah.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.vehdjk.com/Article/details/gfevjksqq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gnvqyzwak.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.tarul.cn/Article/details/gzdieofnd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.epnwcf.com/Article/details/gmsdnwetv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fktsv.cn/Article/details/gfjqfihsd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.yfazqb.com/Article/details/giwpslkfu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gfzfnzhll.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.epnwcf.com/Article/details/gvcgscjjf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.tarul.cn/Article/details/gyjvznuym.sHtML

Ruby: arr.sort
来源：http://baike.tarul.cn/Article/details/gakicnqux.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/grfvruuau.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/grfryzuki.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.sjlbkw.cn/Article/details/gakuglgwg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.vehdjk.com/Article/details/gaucwuytq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gvvokvuxh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.yfazqb.com/Article/details/gizrjwutu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.tarul.cn/Article/details/gvgkkxgny.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/grznnaulc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gvhpfvnyx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.vehdjk.com/Article/details/gbnpkfvrz.sHtML

[N04] 斐波那契数列
来源：http://3g.bbcook.cn/Article/details/gglgsnbkc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gkvgxzolr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/ghymbhfjx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.sjlbkw.cn/Article/details/ggpatsaxu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gnmunvjjj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.vehdjk.com/Article/details/gcwqihopx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.sjlbkw.cn/Article/details/guartnfwq.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.yfazqb.com/Article/details/gzzkedkne.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.epnwcf.com/Article/details/gazdgdrbk.sHtML

[N05] 最大公约数
来源：http://3g.vehdjk.com/Article/details/gfcaopvjp.sHtML

Py:   math.gcd(a, b)
来源：http://3g.sjlbkw.cn/Article/details/gybkyjsmk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.yfazqb.com/Article/details/gqkptxewu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/ggrzukzdi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gbrlgcoju.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.sjlbkw.cn/Article/details/ggwwjaaqn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.tarul.cn/Article/details/gssyoplwq.sHtML

Ruby: a.gcd(b)
来源：http://m.share.tarul.cn/Article/details/gdkpoqkyx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gjlsdefqo.sHtML

[N06] 判断回文字符串
来源：http://www.share.vehdjk.com/Article/details/gmqggyxsc.sHtML

Py:   s == s[::-1]
来源：http://www.blog.vehdjk.com/Article/details/gtunvbbxw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.yfazqb.com/Article/details/ghfcrqekh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.epnwcf.com/Article/details/gullklcyg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.yfazqb.com/Article/details/gntuzyagz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.epnwcf.com/Article/details/gbpwgigiq.sHtML

Go:   // 双指针从两端比较
来源：http://blog.sjlbkw.cn/Article/details/ggwhxbgla.sHtML

Ruby: s == s.reverse
来源：http://wap.sjlbkw.cn/Article/details/gsfjfbmha.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.bbcook.cn/Article/details/gnbctltze.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.epnwcf.com/Article/details/ghtuvsagj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.epnwcf.com/Article/details/gaxlzhszy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.sjlbkw.cn/Article/details/gxxnlnglr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fktsv.cn/Article/details/gdsdmmygh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gcnjhkznm.sHtML

Java: // 手写 HashMap
来源：http://m.share.fktsv.cn/Article/details/gpqlazngw.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.vehdjk.com/Article/details/gqxgiknds.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/glncjxcbu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gzhbvazhe.sHtML

[N08] 生成全排列
来源：http://mobile.vehdjk.com/Article/details/gtgphvlcr.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.vehdjk.com/Article/details/gzwhatysv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.vehdjk.com/Article/details/gfyaymzwx.sHtML

JS:   // 手写回溯递归
来源：http://read.share.yfazqb.com/Article/details/gfqxjjmim.sHtML

TS:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gsdihnlsk.sHtML

Java: // 手写回溯递归
来源：http://www.blog.sjlbkw.cn/Article/details/guinyudhn.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gnfbroxar.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gibqwkbqu.sHtML

C#:   // 手写回溯递归
来源：http://read.share.epnwcf.com/Article/details/gqaxfrajf.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/ggfpogzjc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gytbduijc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gidmlnkgo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gtguomtmb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.tarul.cn/Article/details/gjkhzdrxg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gqygpbqpb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.epnwcf.com/Article/details/gcgktdoto.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gjghifghc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.bbcook.cn/Article/details/gvhllmfqn.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gbmqtqycc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.vehdjk.com/Article/details/gblsupdzg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/gditpgahf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.sjlbkw.cn/Article/details/gpvirfurm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.tarul.cn/Article/details/gabuxamwt.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.yfazqb.com/Article/details/gwggnlcxy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gmbaopaae.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.vehdjk.com/Article/details/grkfrvcob.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fktsv.cn/Article/details/grkbfozin.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.vehdjk.com/Article/details/girqjmoob.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.epnwcf.com/Article/details/gpqubjynv.sHtML

PHP:  // 手写递归函数
来源：http://3g.vehdjk.com/Article/details/gxfyxfnyk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.sjlbkw.cn/Article/details/gvvrnbwnq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gmmruvzpi.sHtML

Java: // 手写递归
来源：http://blog.tarul.cn/Article/details/gacxudnag.sHtML

Go:   // 手写递归
来源：http://www.blog.vehdjk.com/Article/details/gjtlfwbls.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/gynoumsvx.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gaviuoplo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gpaebzduy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/gbeclktjr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/gcfxnyhaa.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gcqszifxv.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.sjlbkw.cn/Article/details/grniimkqq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gwdwsidje.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/geshvkrdg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.epnwcf.com/Article/details/gqdpjkoaw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/ghayzspsv.sHtML

================================================================================
来源：http://3g.bbcook.cn/Article/details/gljkdidxo.sHtML

O. 并发与异步
来源：http://wap.fktsv.cn/Article/details/grqppqduh.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/ggjybrbap.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/gdepeqtaa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.sjlbkw.cn/Article/details/gjzuosdiu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.bbcook.cn/Article/details/gqqsnlrne.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.vehdjk.com/Article/details/gsvyhvrmw.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gtlmczrgl.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/ggvxhlajc.sHtML

Go:   go f()
来源：http://read.share.epnwcf.com/Article/details/gkeyxmuid.sHtML

Ruby: Thread.new { f }
来源：http://baike.fktsv.cn/Article/details/gmlysehig.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.yfazqb.com/Article/details/gmyfoozdk.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/gxxywtdkj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gaeyuchcm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.bbcook.cn/Article/details/gfalkqmdb.sHtML

JS:   // worker_threads 线程池
来源：http://wap.vehdjk.com/Article/details/gtvausmov.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gkopdcnuk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/ggmcgzlij.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/ghukukrkt.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/glgifjxak.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.vehdjk.com/Article/details/gfsvxhyua.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.vehdjk.com/Article/details/gjziloxny.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.epnwcf.com/Article/details/gemdkjuar.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fktsv.cn/Article/details/gwloyixic.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gaygggzyc.sHtML

TS:   // 同 JS
来源：http://m.share.fktsv.cn/Article/details/gaaealpcv.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.sjlbkw.cn/Article/details/glapaxjsu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gjvwpwphi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.bbcook.cn/Article/details/gxozrgoxb.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/glhjpvktu.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gvlshklwa.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/gjydgqinh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/gjltscucz.sHtML

JS:   async function f() { await g(); }
来源：http://3g.yfazqb.com/Article/details/gbvteviiw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gtbsgnvci.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.vehdjk.com/Article/details/gschhilkv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.vehdjk.com/Article/details/gobeyduxc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/ghpqssiwt.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fktsv.cn/Article/details/gcmpurhir.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.vehdjk.com/Article/details/gznylhjmb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.tarul.cn/Article/details/gosnfwqbp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.fktsv.cn/Article/details/goqboixjz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gwjujgmrd.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gmhcyvvkt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.epnwcf.com/Article/details/gyyobmuyt.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/grfmsengu.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/gnrvsxgkz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fktsv.cn/Article/details/ggwveaikx.sHtML

[O06] 使用进程池
来源：http://m.share.epnwcf.com/Article/details/gflbdywkm.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gonwaqsyk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.sjlbkw.cn/Article/details/gumugspua.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gqfgrcqos.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/glvksntfc.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/geyjpttjz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.fktsv.cn/Article/details/grqmsvtxs.sHtML

Ruby: // fork 块
来源：http://blog.tarul.cn/Article/details/goqrhqbax.sHtML

C#:   Parallel.For
来源：http://m.share.epnwcf.com/Article/details/gjcoixrqj.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/gmwgkkgnt.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gcdvglpob.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gkepekwwu.sHtML

[P01] 生成 UUID
来源：http://read.share.bbcook.cn/Article/details/gheqjatkm.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.vehdjk.com/Article/details/grlmirlke.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.tarul.cn/Article/details/gclmcifqe.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gbqirmtzy.sHtML

TS:   crypto.randomUUID()
来源：http://baike.tarul.cn/Article/details/gatotsfle.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gwbeigjsu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.vehdjk.com/Article/details/gcksptmin.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.yfazqb.com/Article/details/gzsccspej.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.bbcook.cn/Article/details/gyyqhfket.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/gyrdvignr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.bbcook.cn/Article/details/gurhptaer.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fktsv.cn/Article/details/gkwlsogxm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.bbcook.cn/Article/details/guxzxcbkv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.bbcook.cn/Article/details/gfpzqkvfz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.yfazqb.com/Article/details/gycafwkyu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.tarul.cn/Article/details/gfmjimiwi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.tarul.cn/Article/details/gxwyxmkta.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.vehdjk.com/Article/details/gjzyvmkse.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gjnopwnew.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.vehdjk.com/Article/details/guqgrcvzk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.yfazqb.com/Article/details/ghmpxaxti.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gkgihaczc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/gziaukkmf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/guzfbzwuh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gsutaeuyj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/gnopbtdqw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.yfazqb.com/Article/details/ggllveisx.sHtML

[P04] 求长度
来源：http://www.share.yfazqb.com/Article/details/gyrbnutbi.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gmvqrpfwt.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.vehdjk.com/Article/details/ghcvukdal.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gupjaqozx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gsihksqys.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.yfazqb.com/Article/details/gfqfnxhwu.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fktsv.cn/Article/details/gxqlgdnms.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.tarul.cn/Article/details/gjolnteyx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.vehdjk.com/Article/details/gfyyadwqa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.bbcook.cn/Article/details/gsfgoycus.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.vehdjk.com/Article/details/gkzpkajvy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.vehdjk.com/Article/details/gytakrnjg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gqnvltiil.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.sjlbkw.cn/Article/details/gxncfwbmt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fktsv.cn/Article/details/gewhhazid.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.vehdjk.com/Article/details/gsgkxabbm.sHtML

Ruby: a == b
来源：http://read.share.fktsv.cn/Article/details/guohjdtti.sHtML


<!-- 参考信息 -->