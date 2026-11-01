代发 wailian999

TS:   resp.ok;  resp.status
来源：http://read.share.tarul.cn/Article/details/gvciynzmk.sHtML

Java: resp.statusCode()
来源：http://read.share.yfazqb.com/Article/details/grerbhcsp.sHtML

Go:   resp.StatusCode
来源：http://www.share.vehdjk.com/Article/details/gkewtdmyl.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.tarul.cn/Article/details/ghieocfnp.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/glhpsdvbu.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.tarul.cn/Article/details/gwhlvsnca.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.sjlbkw.cn/Article/details/gllsyvkld.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.tarul.cn/Article/details/gjbjkuvxf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/guylkcdcu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gawgryeed.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.bbcook.cn/Article/details/gbvagycpt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fktsv.cn/Article/details/ghydcpejd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.tarul.cn/Article/details/gtvudoumf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.yfazqb.com/Article/details/gncbyawxe.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gkxcodbrd.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fktsv.cn/Article/details/gihsljrta.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gtcuwbvrb.sHtML

[M01] 读取命令行参数
来源：http://blog.vehdjk.com/Article/details/gaekecefb.sHtML

Py:   sys.argv[1:]
来源：http://mobile.sjlbkw.cn/Article/details/gjbqrbfva.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.vehdjk.com/Article/details/gnlskwzqo.sHtML

JS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gcdjqezrz.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fktsv.cn/Article/details/gyypzceqh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.yfazqb.com/Article/details/gbadawffg.sHtML

Go:   os.Args[1:]
来源：http://read.share.vehdjk.com/Article/details/gpdxjanko.sHtML

Ruby: ARGV
来源：http://3g.bbcook.cn/Article/details/gluxlgbxo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.bbcook.cn/Article/details/gzgoadamy.sHtML

[M02] 读取环境变量
来源：http://3g.vehdjk.com/Article/details/gcnbdklgf.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gapkmyese.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.sjlbkw.cn/Article/details/gesavcwqd.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gwzczftjn.sHtML

TS:   process.env.HOME
来源：http://wap.sjlbkw.cn/Article/details/gkwhgyrco.sHtML

Java: System.getenv("HOME")
来源：http://baike.fktsv.cn/Article/details/gyuecedga.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.yfazqb.com/Article/details/gxgupzutc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.vehdjk.com/Article/details/gjjkvgvhv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.yfazqb.com/Article/details/gvonsjdih.sHtML

[M03] 执行外部命令
来源：http://mobile.epnwcf.com/Article/details/gorzzrcgz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gfcfahgur.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.yfazqb.com/Article/details/gvafjyjts.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.epnwcf.com/Article/details/gabunlosw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fktsv.cn/Article/details/gkkhlshnw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gsaftwwlp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.vehdjk.com/Article/details/gvfgkrpcm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/gliathpfv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.epnwcf.com/Article/details/gkwysnflt.sHtML

[M04] 获取当前工作目录
来源：http://wap.yfazqb.com/Article/details/gjszqrxfe.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gsixqeppf.sHtML

PHP:  getcwd();
来源：http://www.share.yfazqb.com/Article/details/gssybadmy.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gbvvwaybe.sHtML

TS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gvamuzjqm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.bbcook.cn/Article/details/gluixytwy.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gjqscivpv.sHtML

Ruby: Dir.pwd
来源：http://baike.fktsv.cn/Article/details/gekgtvklo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.tarul.cn/Article/details/gxwbqdtuk.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/gxjwtnhmo.sHtML

Py:   sys.exit(1)
来源：http://www.blog.bbcook.cn/Article/details/gtsbvveye.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gpyrvyqdi.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gylqjfzot.sHtML

TS:   process.exit(1)
来源：http://blog.epnwcf.com/Article/details/gozyiwppf.sHtML

Java: System.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gqtavyujq.sHtML

Go:   os.Exit(1)
来源：http://m.share.sjlbkw.cn/Article/details/gutvlvfcf.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/gdwsudikm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.vehdjk.com/Article/details/ghmzrlvjg.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gpxtrygsz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.vehdjk.com/Article/details/gbghlanmg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fktsv.cn/Article/details/gbhldomqn.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/grlyeggit.sHtML

TS:   console.error("err")
来源：http://www.m.share.fktsv.cn/Article/details/ghtijmeko.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gshycbrwg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.sjlbkw.cn/Article/details/gakfzgwum.sHtML

Ruby: warn "err"
来源：http://www.blog.epnwcf.com/Article/details/gpusulgje.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.epnwcf.com/Article/details/gvijdldhu.sHtML

[M07] 判断是否为主入口
来源：http://read.share.yfazqb.com/Article/details/ggrayltom.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.epnwcf.com/Article/details/genorbpvh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/goezisaxh.sHtML

JS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gshbzhgaa.sHtML

TS:   require.main === module
来源：http://read.share.yfazqb.com/Article/details/ggpbbeqmd.sHtML

Java: public static void main(String[] args)
来源：http://3g.sjlbkw.cn/Article/details/gubtxjjbv.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/ghaefppnn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.bbcook.cn/Article/details/gpwzfcghi.sHtML

C#:   static void Main(string[] args)
来源：http://blog.sjlbkw.cn/Article/details/griopencw.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gunxmnryq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/gfnyutivr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fktsv.cn/Article/details/gqqfvokyq.sHtML

JS:   process.platform;  process.version
来源：http://wap.tarul.cn/Article/details/gdqqxsdwa.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.bbcook.cn/Article/details/gpjlmhhbr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.sjlbkw.cn/Article/details/gutkbdzsp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.bbcook.cn/Article/details/grdvqinyk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gqjeoedlv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fktsv.cn/Article/details/gztiosmyl.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gvhbwqaeg.sHtML

N. 数据结构与算法
来源：http://read.share.yfazqb.com/Article/details/gcaiyqhsa.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gscrirxgj.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.tarul.cn/Article/details/gppnjpzpd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gvhljdcsc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fktsv.cn/Article/details/gmlddywsd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.sjlbkw.cn/Article/details/gteivfvbm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.bbcook.cn/Article/details/gwnzsudog.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/guzsltywi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.vehdjk.com/Article/details/gdqtcbuqh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.epnwcf.com/Article/details/gkxvnvttj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gyipwhnkc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.bbcook.cn/Article/details/gxbotvese.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.bbcook.cn/Article/details/gfuuzelyb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/gazsjeumy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gcinwpxzx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/ggxonkkee.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.bbcook.cn/Article/details/gsckwypea.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.sjlbkw.cn/Article/details/gsupsfimu.sHtML

Ruby: arr.sort
来源：http://baike.epnwcf.com/Article/details/ghxlbsqzv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gazqooqmy.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.sjlbkw.cn/Article/details/gfptsqvxw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.epnwcf.com/Article/details/gvavyonsz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.sjlbkw.cn/Article/details/gjrxxixar.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gtqpehoty.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gpowcirbf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/geojiraro.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/gqjjohdxi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fktsv.cn/Article/details/gidgykqaf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fktsv.cn/Article/details/gdfdefucy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.tarul.cn/Article/details/gxekqzhqw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gwriohsmz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/gctuooyto.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/ghceoebgp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.tarul.cn/Article/details/gpqzasiwv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.epnwcf.com/Article/details/gmxamibks.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fktsv.cn/Article/details/ggfbnthfm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.tarul.cn/Article/details/gygdhiydb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gteesicef.sHtML

[N05] 最大公约数
来源：http://www.share.sjlbkw.cn/Article/details/gytegywxy.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gpnhpfron.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gooamgwuo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.bbcook.cn/Article/details/gonnzeiie.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.sjlbkw.cn/Article/details/ghsptqmqa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fktsv.cn/Article/details/gvvklbvvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.tarul.cn/Article/details/gcigqlcvd.sHtML

Ruby: a.gcd(b)
来源：http://baike.epnwcf.com/Article/details/gglfjtpgm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.vehdjk.com/Article/details/gpairyzuo.sHtML

[N06] 判断回文字符串
来源：http://www.share.fktsv.cn/Article/details/gyjhfhnmb.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gqnkykucx.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fktsv.cn/Article/details/gacbemfob.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fktsv.cn/Article/details/grxyuvefw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.yfazqb.com/Article/details/gktsytrra.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.sjlbkw.cn/Article/details/gruxwxzug.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/gpcnzdpem.sHtML

Ruby: s == s.reverse
来源：http://m.share.epnwcf.com/Article/details/gvaeipgtv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/geabrqdbt.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.sjlbkw.cn/Article/details/gpknqtuhm.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.vehdjk.com/Article/details/ghidsdvca.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.fktsv.cn/Article/details/glftyzfqb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.bbcook.cn/Article/details/ghwmhncci.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fktsv.cn/Article/details/glixfkyiw.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gxhsnauni.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.vehdjk.com/Article/details/gwzyrfqzw.sHtML

Ruby: // 手写 Hash
来源：http://mobile.bbcook.cn/Article/details/gyrytvkva.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/gmjuvscui.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/gvfqpjgob.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.epnwcf.com/Article/details/gppkgyjtw.sHtML

PHP:  // 手写递归交换
来源：http://wap.bbcook.cn/Article/details/gbftkjkng.sHtML

JS:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gmmdftxtw.sHtML

TS:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gnfxmbozs.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gxsbznpme.sHtML

Go:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gyxyuiuus.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.tarul.cn/Article/details/grdvwgimx.sHtML

C#:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gqagbgmdy.sHtML

[N09] 栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/gjucxykdl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/gvwijywuj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.tarul.cn/Article/details/gvqwegrgk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gthtlqprx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.yfazqb.com/Article/details/glbztxdej.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.epnwcf.com/Article/details/gaffkmuxr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.vehdjk.com/Article/details/gpftajgae.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/glgqiysik.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.tarul.cn/Article/details/geheamuds.sHtML

[N10] 链表节点定义
来源：http://www.m.share.vehdjk.com/Article/details/gibhzhcpe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/godocjfql.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.tarul.cn/Article/details/gsmgljutg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.yfazqb.com/Article/details/grytjwcgt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gggehixdk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fktsv.cn/Article/details/gmdhzlnck.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/guisajdgg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fktsv.cn/Article/details/gnibyalkc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.yfazqb.com/Article/details/grlpcarvd.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gwvfjcufg.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.yfazqb.com/Article/details/gxfzfffrz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.vehdjk.com/Article/details/gzhtwqkyl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fktsv.cn/Article/details/gewhwclry.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.epnwcf.com/Article/details/gzczstvew.sHtML

Java: // 手写递归
来源：http://3g.bbcook.cn/Article/details/gvcfdzgii.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gkinnhosz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fktsv.cn/Article/details/gtouatatg.sHtML

C#:   // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gbqprealg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.bbcook.cn/Article/details/gszwnjgnv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/giifypbsa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.bbcook.cn/Article/details/gttustibe.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.bbcook.cn/Article/details/gvaktavbh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gfvnwldrp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.epnwcf.com/Article/details/gavxufsbp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.bbcook.cn/Article/details/gcejzrlmw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.yfazqb.com/Article/details/gtfblkokt.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.fktsv.cn/Article/details/gbgnvober.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/geoaptack.sHtML

O. 并发与异步
来源：http://wap.bbcook.cn/Article/details/glubkxkgq.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gwjssezep.sHtML

[O01] 启动一个线程
来源：http://www.m.share.vehdjk.com/Article/details/gmplyzshf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.bbcook.cn/Article/details/gmktdzefv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.yfazqb.com/Article/details/gprmswqhj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.tarul.cn/Article/details/glopyclnm.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gduugzjxe.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/glqyciunu.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/glrzhtmgz.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.bbcook.cn/Article/details/gtabhkdzw.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.bbcook.cn/Article/details/glurgqywd.sHtML

[O02] 使用线程池
来源：http://read.share.tarul.cn/Article/details/grreoiwkx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gicezfgad.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.yfazqb.com/Article/details/gbntymjec.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gwoikcisu.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.bbcook.cn/Article/details/gxkyzdeqn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.tarul.cn/Article/details/gvgpqapxs.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.tarul.cn/Article/details/glomaichy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.bbcook.cn/Article/details/grwewtffu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.yfazqb.com/Article/details/gutjorulq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gmssiprps.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.epnwcf.com/Article/details/gseruyqxs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.vehdjk.com/Article/details/gyicpstgh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.yfazqb.com/Article/details/gnfgvoguu.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/gjttmdehq.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gfruewxkl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.fktsv.cn/Article/details/godmoexfr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.epnwcf.com/Article/details/gobcushwy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.epnwcf.com/Article/details/gflctvvso.sHtML

[O04] 定义异步函数并等待
来源：http://wap.sjlbkw.cn/Article/details/gwmdzvjyi.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.vehdjk.com/Article/details/glcclggvx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.vehdjk.com/Article/details/gmdlbnbjy.sHtML

JS:   async function f() { await g(); }
来源：http://baike.tarul.cn/Article/details/gmwjerjxc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fktsv.cn/Article/details/gxawnpojg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/gxijrmunr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fktsv.cn/Article/details/gyyhvmpbt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.epnwcf.com/Article/details/gjzyfxvxv.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.bbcook.cn/Article/details/gysejhkwr.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/geigvgerk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.tarul.cn/Article/details/gqomehwyr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/gqztvnvzo.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.sjlbkw.cn/Article/details/gisxulcez.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.yfazqb.com/Article/details/gkgomsiom.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.vehdjk.com/Article/details/gasvqaohu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gekjsnfyo.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.sjlbkw.cn/Article/details/gjnkckpld.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.tarul.cn/Article/details/glccxozhn.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/gwlrcxdcv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.fktsv.cn/Article/details/gbbjcyuaj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.yfazqb.com/Article/details/gjlojdpne.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fktsv.cn/Article/details/gyuinfeor.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.bbcook.cn/Article/details/gslnwrvqs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fktsv.cn/Article/details/gkmwzrovo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.tarul.cn/Article/details/gjmfzfbna.sHtML

Ruby: // fork 块
来源：http://read.share.yfazqb.com/Article/details/gautswxxn.sHtML

C#:   Parallel.For
来源：http://www.share.tarul.cn/Article/details/gpqglwakt.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gfuckjslh.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gkrqolocr.sHtML

================================================================================
来源：http://mobile.yfazqb.com/Article/details/gteugdsnw.sHtML

[P01] 生成 UUID
来源：http://www.blog.tarul.cn/Article/details/glfvuuukx.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fktsv.cn/Article/details/gqubiulgb.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.yfazqb.com/Article/details/gwzssvkxl.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/gpulxzbtl.sHtML

TS:   crypto.randomUUID()
来源：http://blog.yfazqb.com/Article/details/gjvkvefwc.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gmsbzyfeh.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gpxtysfdt.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.epnwcf.com/Article/details/gctgxxflk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.yfazqb.com/Article/details/gepjgjabc.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.vehdjk.com/Article/details/gwmijvwnx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.vehdjk.com/Article/details/gedeixdhk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.tarul.cn/Article/details/gtaskaezd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.bbcook.cn/Article/details/gjozrepak.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.epnwcf.com/Article/details/gqpyveggz.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gkjdqmmox.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.vehdjk.com/Article/details/gvkovedbh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.vehdjk.com/Article/details/gpwqjrjci.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.bbcook.cn/Article/details/gaxpspbeh.sHtML

[P03] 生成短随机字符串
来源：http://m.share.vehdjk.com/Article/details/gmusukeke.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.vehdjk.com/Article/details/gzlmlqrup.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gocpxgrmf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gmwijmllh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/gmulfpvdf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.fktsv.cn/Article/details/gsewknhzv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.bbcook.cn/Article/details/ghfiguhad.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.epnwcf.com/Article/details/gjxqxtdbj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.yfazqb.com/Article/details/gkkbiqrep.sHtML

[P04] 求长度
来源：http://wap.tarul.cn/Article/details/gklfpkyse.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.vehdjk.com/Article/details/gahrxoyrf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fktsv.cn/Article/details/gzukvruvy.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.sjlbkw.cn/Article/details/gsnbauzbf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gkjvzfyra.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.tarul.cn/Article/details/gnjujrkys.sHtML

Go:   len(arr);  len(m)
来源：http://baike.bbcook.cn/Article/details/gauilsnvn.sHtML

Ruby: x.length;  x.size
来源：http://www.share.epnwcf.com/Article/details/gzsihvdvg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.yfazqb.com/Article/details/gylsvjpze.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.epnwcf.com/Article/details/gdyftrque.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gbiowdqgy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.tarul.cn/Article/details/gbtodygfl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.vehdjk.com/Article/details/ghyleejup.sHtML


<!-- 参考信息 -->