代发 wailian999

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.yfazqb.com/Article/details/gryxrtyxq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fktsv.cn/Article/details/gxbsipllx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.epnwcf.com/Article/details/gyomhxmny.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.sjlbkw.cn/Article/details/glcewgbel.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.epnwcf.com/Article/details/gghmcwacu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.bbcook.cn/Article/details/guyfjvcgv.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.epnwcf.com/Article/details/gwxojopzx.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fktsv.cn/Article/details/gliuvzdqd.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.tarul.cn/Article/details/guarficmj.sHtML

Java: resp.statusCode()
来源：http://mobile.sjlbkw.cn/Article/details/gvxbvrxly.sHtML

Go:   resp.StatusCode
来源：http://read.share.tarul.cn/Article/details/gdwehezzn.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.epnwcf.com/Article/details/gcvislyyl.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.vehdjk.com/Article/details/gpatoijgf.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.yfazqb.com/Article/details/gowgxxvtv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.bbcook.cn/Article/details/gmaiykvmp.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.epnwcf.com/Article/details/gchnrkglv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gdzqbvuka.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.yfazqb.com/Article/details/gctlhsztq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.epnwcf.com/Article/details/gmvmtishj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/gikameomr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.tarul.cn/Article/details/gyqsvjghr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fktsv.cn/Article/details/goughjgvq.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gvucwsqzd.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.tarul.cn/Article/details/gupwtwayg.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gzodcmbmm.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/gqcotrjlz.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.tarul.cn/Article/details/gcjwzsqyk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/ghtfwdwkv.sHtML

JS:   process.argv.slice(2)
来源：http://blog.bbcook.cn/Article/details/ggvpswelt.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gepewdleg.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.yfazqb.com/Article/details/ghoxoeddw.sHtML

Go:   os.Args[1:]
来源：http://baike.bbcook.cn/Article/details/gqjycucdm.sHtML

Ruby: ARGV
来源：http://baike.yfazqb.com/Article/details/gkduqicas.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.tarul.cn/Article/details/gyyceuzql.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gewnucpua.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gzgjtyuyn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gqlmjltld.sHtML

JS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/grastdnjp.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gwsrchroz.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/grewomhdz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.tarul.cn/Article/details/gnhilcbhp.sHtML

Ruby: ENV["HOME"]
来源：http://wap.tarul.cn/Article/details/gysulujlt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.tarul.cn/Article/details/geiacyhva.sHtML

[M03] 执行外部命令
来源：http://blog.epnwcf.com/Article/details/gwmuzbsie.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fktsv.cn/Article/details/gswbjludc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gnecmtduj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fktsv.cn/Article/details/gwggtkevl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gqwoggspl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.epnwcf.com/Article/details/gzzyudhhf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.vehdjk.com/Article/details/gwmywcnni.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.tarul.cn/Article/details/gkzidxlkd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.epnwcf.com/Article/details/gqtizdqto.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/ghyqftscy.sHtML

Py:   os.getcwd()
来源：http://blog.bbcook.cn/Article/details/gapiunvtt.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/guxjmhvpu.sHtML

JS:   process.cwd()
来源：http://3g.epnwcf.com/Article/details/gmzyxjqsc.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gvoghwjxa.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.epnwcf.com/Article/details/gyleaguwn.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/ghanuwafa.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gqruaglvr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.sjlbkw.cn/Article/details/gariqphun.sHtML

[M05] 设置退出码
来源：http://wap.vehdjk.com/Article/details/gylasbfgq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gxbsjegqe.sHtML

PHP:  exit(1);
来源：http://www.m.share.yfazqb.com/Article/details/gfwdlxuae.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/ginwjfmpn.sHtML

TS:   process.exit(1)
来源：http://m.share.tarul.cn/Article/details/gtcinptmz.sHtML

Java: System.exit(1)
来源：http://3g.sjlbkw.cn/Article/details/gsndqgdnh.sHtML

Go:   os.Exit(1)
来源：http://wap.fktsv.cn/Article/details/gncmzcjfj.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gzkgypmfo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.epnwcf.com/Article/details/ghzmfrzmp.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.bbcook.cn/Article/details/gkqphijfq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fktsv.cn/Article/details/gqufenvtk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.vehdjk.com/Article/details/gbdkjdziu.sHtML

JS:   console.error("err")
来源：http://www.blog.bbcook.cn/Article/details/goqtlrzqw.sHtML

TS:   console.error("err")
来源：http://wap.yfazqb.com/Article/details/gpyfrxgoo.sHtML

Java: System.err.println("err")
来源：http://3g.sjlbkw.cn/Article/details/gjfetklyj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.sjlbkw.cn/Article/details/gjrtskssc.sHtML

Ruby: warn "err"
来源：http://blog.yfazqb.com/Article/details/ghdzvufas.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.vehdjk.com/Article/details/gcpbiwkve.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/grtcjbvjx.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.vehdjk.com/Article/details/gkfgeafvr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.epnwcf.com/Article/details/gfisbtpbd.sHtML

JS:   require.main === module
来源：http://3g.epnwcf.com/Article/details/gyyinzzip.sHtML

TS:   require.main === module
来源：http://www.blog.fktsv.cn/Article/details/gndfvkvlb.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gmfvtahix.sHtML

Go:   func main()
来源：http://m.share.yfazqb.com/Article/details/gnxrhfcna.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/ghkakwgaz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fktsv.cn/Article/details/gcbcfcnit.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.sjlbkw.cn/Article/details/gftphtyuc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fktsv.cn/Article/details/gyxgpwkcg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.vehdjk.com/Article/details/glflebpuu.sHtML

JS:   process.platform;  process.version
来源：http://blog.sjlbkw.cn/Article/details/gcugxwwxo.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.bbcook.cn/Article/details/gbfzjcdsl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.yfazqb.com/Article/details/gppzkoeyg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gevnehdrk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.tarul.cn/Article/details/gxsdsxyrc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gagydyfth.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gtnoyrnis.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gtphvrcwi.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/guwypvlxw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/ggebzzrfb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fktsv.cn/Article/details/gmyyhyavi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/gikeqzdmx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.vehdjk.com/Article/details/gzrqubxbu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gpavddkiz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.sjlbkw.cn/Article/details/gatgrovjk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.tarul.cn/Article/details/gzmwolmja.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.bbcook.cn/Article/details/grfpxlpei.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gmhxhmqeb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.yfazqb.com/Article/details/githgljrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbvigrcmr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.bbcook.cn/Article/details/gqmgrhkcg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gkiqzipgf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gxkcbxptu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.epnwcf.com/Article/details/gonemgaem.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fktsv.cn/Article/details/gbjxwwmcs.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gcuklgsxn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fktsv.cn/Article/details/gcqejqcnk.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.tarul.cn/Article/details/grfnwutrs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gafrjjruz.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gsqmbulxj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.bbcook.cn/Article/details/gqvzwdavp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.yfazqb.com/Article/details/grrjybdul.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.yfazqb.com/Article/details/gyatmxgrz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.bbcook.cn/Article/details/gvpvvjqnc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.vehdjk.com/Article/details/gqvtihkzf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.yfazqb.com/Article/details/gjakdgtqz.sHtML

[N04] 斐波那契数列
来源：http://blog.vehdjk.com/Article/details/guzrlevof.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.sjlbkw.cn/Article/details/gevojzltm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.tarul.cn/Article/details/gbsmgtqzy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/glwvlqhgg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gunpgxovc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.sjlbkw.cn/Article/details/gtamaztik.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.sjlbkw.cn/Article/details/gneqvofvx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.yfazqb.com/Article/details/gutofuzvj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gpnscanvj.sHtML

[N05] 最大公约数
来源：http://m.share.epnwcf.com/Article/details/guvrxszez.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fktsv.cn/Article/details/gzotgwymi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.epnwcf.com/Article/details/gwllhubxi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.epnwcf.com/Article/details/gprquwpnh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.epnwcf.com/Article/details/gtecyqfpl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gashiufwb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gialgbynz.sHtML

Ruby: a.gcd(b)
来源：http://3g.sjlbkw.cn/Article/details/gzkzfhrza.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.epnwcf.com/Article/details/gcqrpheux.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gjaxhwafe.sHtML

Py:   s == s[::-1]
来源：http://wap.epnwcf.com/Article/details/gwuxeevco.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fktsv.cn/Article/details/gyqddmasx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/glsbrtbkp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fktsv.cn/Article/details/gbjipbcma.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fktsv.cn/Article/details/gnkbmyron.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.bbcook.cn/Article/details/gtbbbkwrs.sHtML

Ruby: s == s.reverse
来源：http://baike.fktsv.cn/Article/details/gzmqpihus.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.yfazqb.com/Article/details/gtrifyqan.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.sjlbkw.cn/Article/details/gdttsmsnb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.bbcook.cn/Article/details/gekpiqejx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.epnwcf.com/Article/details/gblryulpn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.epnwcf.com/Article/details/gozxtqpxv.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.tarul.cn/Article/details/glqykxcta.sHtML

Java: // 手写 HashMap
来源：http://wap.bbcook.cn/Article/details/geugbueqf.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.sjlbkw.cn/Article/details/gmxtdhgqf.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gzvyxysfa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.vehdjk.com/Article/details/gvkezzhfu.sHtML

[N08] 生成全排列
来源：http://m.share.tarul.cn/Article/details/gnevnhdti.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fktsv.cn/Article/details/gwwmhqqxu.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/gkgiyaonx.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/guehblqlr.sHtML

TS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gzwgewpdq.sHtML

Java: // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gvonyyqrf.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.yfazqb.com/Article/details/gugqqbmog.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.fktsv.cn/Article/details/gypnnmgot.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gkaazaing.sHtML

[N09] 栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gtsrutzzz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fktsv.cn/Article/details/gqjyuexxj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fktsv.cn/Article/details/gmlxunqgl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.vehdjk.com/Article/details/ggjgrhgoh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.tarul.cn/Article/details/gqskawmxa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/gaecjwtlr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.yfazqb.com/Article/details/gvmodrlcv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gcjvvoepk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gxyjpaaxa.sHtML

[N10] 链表节点定义
来源：http://www.blog.fktsv.cn/Article/details/gnoqcjkrc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.bbcook.cn/Article/details/gnpauytcx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fktsv.cn/Article/details/gwdomvcoy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.vehdjk.com/Article/details/gziibyzqm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.vehdjk.com/Article/details/gyoqjyywd.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/gsuggstsh.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.sjlbkw.cn/Article/details/gmkcihlyb.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.tarul.cn/Article/details/ghtugmjzp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.yfazqb.com/Article/details/ghjgcsxtw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/guqnjujqa.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fktsv.cn/Article/details/gnkhfaqsz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gittnvpxx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gryotwjvd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.bbcook.cn/Article/details/gvtmpcczh.sHtML

Java: // 手写递归
来源：http://m.share.yfazqb.com/Article/details/geaqfoite.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/gtsfiojjv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gmerhcwlk.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/grscuavah.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gclndkhfh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fktsv.cn/Article/details/gywkwgkxp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fktsv.cn/Article/details/gjwrdbhfy.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/gdzpkqjwc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.yfazqb.com/Article/details/gdegyglfc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gizujkpdd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.sjlbkw.cn/Article/details/gqrxmsiuq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gqxedfzjn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gfmetneag.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gcjvybred.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/gfhaipdhc.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/goivtfavu.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fktsv.cn/Article/details/grhkiwtfp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/ghxvlcdml.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.vehdjk.com/Article/details/gfvrgntrt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.fktsv.cn/Article/details/golycqkjp.sHtML

TS:   // 同 JS
来源：http://www.blog.epnwcf.com/Article/details/gkrdijexy.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.yfazqb.com/Article/details/gmtlcrcai.sHtML

Go:   go f()
来源：http://blog.sjlbkw.cn/Article/details/glvsdtzrr.sHtML

Ruby: Thread.new { f }
来源：http://baike.sjlbkw.cn/Article/details/gtyzqzbcn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fktsv.cn/Article/details/gdepggjwa.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/gjjcbwpzn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.yfazqb.com/Article/details/grqmggftc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.tarul.cn/Article/details/gelnkextw.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gkqaqnxla.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.bbcook.cn/Article/details/gygspfxli.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.sjlbkw.cn/Article/details/ggytthikv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.epnwcf.com/Article/details/ggphivveh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.yfazqb.com/Article/details/gjbjwufpq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://baike.sjlbkw.cn/Article/details/ghxdkfcec.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.sjlbkw.cn/Article/details/gvxjcrcrj.sHtML

Py:   with lock: shared += 1
来源：http://baike.epnwcf.com/Article/details/gunmfoxxh.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gpoiolcvk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.yfazqb.com/Article/details/gidygmyng.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gxljhmslf.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.bbcook.cn/Article/details/gliqpxhco.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.vehdjk.com/Article/details/gkdfykcok.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fktsv.cn/Article/details/ggsfaykzl.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.tarul.cn/Article/details/gfunqqzjw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.bbcook.cn/Article/details/glhjhayym.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.epnwcf.com/Article/details/gceccmhgp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.bbcook.cn/Article/details/gkzzgheki.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/gfupebhqo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.epnwcf.com/Article/details/gjlpcrptj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.tarul.cn/Article/details/gyoffertj.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.fktsv.cn/Article/details/grevzkszo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.epnwcf.com/Article/details/gmcjdamty.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gelsqtfmd.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.sjlbkw.cn/Article/details/gwayyafxc.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gauwlklcb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.epnwcf.com/Article/details/grpmknnes.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.vehdjk.com/Article/details/gvoehtghk.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.vehdjk.com/Article/details/gyekvsubq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.vehdjk.com/Article/details/gxccgywib.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.bbcook.cn/Article/details/gqwsamyrk.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.tarul.cn/Article/details/gorpbuobj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gvvfboily.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gcbpznbiu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fktsv.cn/Article/details/gfkoaeutw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/ghdfkpkdx.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gofmpnqha.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fktsv.cn/Article/details/gkfjpysmv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.bbcook.cn/Article/details/gmeyfosum.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/gnvfnpjvr.sHtML

Ruby: // fork 块
来源：http://mobile.fktsv.cn/Article/details/grwhslsbh.sHtML

C#:   Parallel.For
来源：http://www.share.yfazqb.com/Article/details/gpwicufcp.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/geunidfew.sHtML

P. 常用工具函数
来源：http://www.share.bbcook.cn/Article/details/gofflfglx.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gvgcadzrb.sHtML

[P01] 生成 UUID
来源：http://baike.epnwcf.com/Article/details/gxuuwnkyw.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/gecozzaqq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.fktsv.cn/Article/details/gatalmxxy.sHtML

JS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gwjsonxcu.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.sjlbkw.cn/Article/details/gzbgxxaql.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.tarul.cn/Article/details/glxkdqizu.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.fktsv.cn/Article/details/gzjebdwou.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.tarul.cn/Article/details/gxwgqibvi.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.tarul.cn/Article/details/gsuwlowpf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.sjlbkw.cn/Article/details/gvuytoltw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.yfazqb.com/Article/details/gcdizewdq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.bbcook.cn/Article/details/glxvvaftd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fktsv.cn/Article/details/gndqbbtbh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gtuxtojau.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.sjlbkw.cn/Article/details/gjluqvigs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gmckjwdxe.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gcyhdamoa.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gdtpqmrip.sHtML

[P03] 生成短随机字符串
来源：http://blog.tarul.cn/Article/details/gzbtlvdep.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.tarul.cn/Article/details/gxzygpbmq.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.epnwcf.com/Article/details/gikhisvyv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fktsv.cn/Article/details/gkobtcxuo.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/ghqhzcees.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.tarul.cn/Article/details/gdiyqymll.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.yfazqb.com/Article/details/gihoykikc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.tarul.cn/Article/details/ghsounyvu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.bbcook.cn/Article/details/gexukhrzu.sHtML

[P04] 求长度
来源：http://read.share.sjlbkw.cn/Article/details/gxpplhxzt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gxfdeexdx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.vehdjk.com/Article/details/gvonsspnw.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gyhcecqmw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fktsv.cn/Article/details/gfrabprmj.sHtML


<!-- 参考信息 -->