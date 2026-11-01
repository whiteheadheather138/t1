代发 wailian999

TS:   resp.ok;  resp.status
来源：http://baike.sjlbkw.cn/Article/details/ggsfhkcdk.sHtML

Java: resp.statusCode()
来源：http://baike.sjlbkw.cn/Article/details/glbxdotyk.sHtML

Go:   resp.StatusCode
来源：http://3g.bbcook.cn/Article/details/gtbglulzv.sHtML

Ruby: resp.code.to_i
来源：http://mobile.yfazqb.com/Article/details/gthacnstg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.tarul.cn/Article/details/gkoaaifpu.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/gtmohtgdq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.bbcook.cn/Article/details/ghnynpozx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.epnwcf.com/Article/details/gradecspn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.tarul.cn/Article/details/gvscrmsji.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.vehdjk.com/Article/details/gamlwxwll.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.yfazqb.com/Article/details/gizfciqli.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/girshomhk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fktsv.cn/Article/details/gikmlidjj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.yfazqb.com/Article/details/gjnbjigyr.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gjhvuckgr.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gvcoyjevb.sHtML

================================================================================
来源：http://mobile.sjlbkw.cn/Article/details/gfbgrdaey.sHtML

[M01] 读取命令行参数
来源：http://baike.tarul.cn/Article/details/gnaosxdop.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/gjltibpxa.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.yfazqb.com/Article/details/gpskgmowz.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fktsv.cn/Article/details/ghvxbelkq.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gylytgmag.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.epnwcf.com/Article/details/gmzvnnfac.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gefhtussq.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/grbladhhc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.epnwcf.com/Article/details/gjfsiwqxx.sHtML

[M02] 读取环境变量
来源：http://baike.fktsv.cn/Article/details/gowdcitdb.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.yfazqb.com/Article/details/gcqvltuys.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.vehdjk.com/Article/details/gefyayrdw.sHtML

JS:   process.env.HOME
来源：http://www.m.share.sjlbkw.cn/Article/details/glulkhrlg.sHtML

TS:   process.env.HOME
来源：http://read.share.yfazqb.com/Article/details/gvgbafxuv.sHtML

Java: System.getenv("HOME")
来源：http://wap.vehdjk.com/Article/details/gjbxgcrkj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.vehdjk.com/Article/details/gvlembxwq.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fktsv.cn/Article/details/gumrhzhyu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.yfazqb.com/Article/details/grvclaxli.sHtML

[M03] 执行外部命令
来源：http://read.share.vehdjk.com/Article/details/gwhridctl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gjpwbeycd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.sjlbkw.cn/Article/details/gtuihiqxa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gcebvtbuu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.bbcook.cn/Article/details/gqddxtkuj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.epnwcf.com/Article/details/ggjwtsefy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fktsv.cn/Article/details/ghyskmxym.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.bbcook.cn/Article/details/gtwvxkgkz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.epnwcf.com/Article/details/gzbbhwbve.sHtML

[M04] 获取当前工作目录
来源：http://3g.fktsv.cn/Article/details/ghfvapphm.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/gkgytbabw.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/gwthqialc.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gcnbsdhbg.sHtML

TS:   process.cwd()
来源：http://m.share.fktsv.cn/Article/details/gbzbrrazb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gamysqkiw.sHtML

Go:   os.Getwd()
来源：http://read.share.tarul.cn/Article/details/giingisnz.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/gmlqafluy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gxemynags.sHtML

[M05] 设置退出码
来源：http://3g.bbcook.cn/Article/details/gwarltjnx.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gjfdnolab.sHtML

PHP:  exit(1);
来源：http://blog.yfazqb.com/Article/details/gvampsodo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/ggrophwwt.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gkerklpth.sHtML

Java: System.exit(1)
来源：http://3g.tarul.cn/Article/details/gwiiptcvp.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gfbnovnep.sHtML

Ruby: exit 1
来源：http://read.share.bbcook.cn/Article/details/gtjypqaxw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.epnwcf.com/Article/details/gtozjltti.sHtML

[M06] 向标准错误输出
来源：http://read.share.tarul.cn/Article/details/ghtoleobu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.tarul.cn/Article/details/gpycymhqc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.sjlbkw.cn/Article/details/gtxbtomdr.sHtML

JS:   console.error("err")
来源：http://blog.bbcook.cn/Article/details/gnxftacyu.sHtML

TS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gkvhjwqgr.sHtML

Java: System.err.println("err")
来源：http://www.share.fktsv.cn/Article/details/gtkkfolnw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.yfazqb.com/Article/details/gtzfrpfzl.sHtML

Ruby: warn "err"
来源：http://wap.tarul.cn/Article/details/goupcbjtj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gvmgcqxvd.sHtML

[M07] 判断是否为主入口
来源：http://blog.bbcook.cn/Article/details/gvagyyqot.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.yfazqb.com/Article/details/gbcazgozn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fktsv.cn/Article/details/gfgeibejr.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/grnwfzyfh.sHtML

TS:   require.main === module
来源：http://m.share.fktsv.cn/Article/details/gulbsokhn.sHtML

Java: public static void main(String[] args)
来源：http://3g.fktsv.cn/Article/details/gdhhwnpdd.sHtML

Go:   func main()
来源：http://wap.yfazqb.com/Article/details/getwmnszc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.vehdjk.com/Article/details/grkqbypoj.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.vehdjk.com/Article/details/gfrtpfyul.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/gxmoxxalq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.yfazqb.com/Article/details/gqxlvxthn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.tarul.cn/Article/details/glzuoyuev.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.yfazqb.com/Article/details/giyrhnarj.sHtML

TS:   process.platform;  process.version
来源：http://baike.sjlbkw.cn/Article/details/guekbffee.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.yfazqb.com/Article/details/gfdagacno.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.bbcook.cn/Article/details/gnizpowyv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fktsv.cn/Article/details/gdlkufoyc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.vehdjk.com/Article/details/guzzkgvgs.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/gktjglkmw.sHtML

N. 数据结构与算法
来源：http://baike.yfazqb.com/Article/details/gnbtmfmei.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/geilwrdzl.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fktsv.cn/Article/details/goyhraxrw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gcywynwnk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.epnwcf.com/Article/details/geeisilgv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.epnwcf.com/Article/details/gxqsgwbxk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.yfazqb.com/Article/details/gbooanjfw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gfmqvbbhu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gnfzxrhel.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/ggplneeqo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.tarul.cn/Article/details/gxiiyxgqe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/ghmxitwyb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.tarul.cn/Article/details/gjdwdtqbg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.epnwcf.com/Article/details/gepkaoydw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.epnwcf.com/Article/details/gawiylcgq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.sjlbkw.cn/Article/details/ggvockeql.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.bbcook.cn/Article/details/gypsieegm.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.yfazqb.com/Article/details/gsduinthf.sHtML

Ruby: arr.sort
来源：http://read.share.yfazqb.com/Article/details/gwwudvknn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.bbcook.cn/Article/details/ggmmzfuhs.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gbuiepzhb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/ggfstggyi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.tarul.cn/Article/details/gltrdrdzk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.sjlbkw.cn/Article/details/gjaeeaquo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gnyodogyq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.bbcook.cn/Article/details/ghwbhscgh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gnhcgtucv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gixhkvxtv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.sjlbkw.cn/Article/details/gxjxtuijz.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.vehdjk.com/Article/details/gbbypxqwm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.epnwcf.com/Article/details/gozhtezio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.sjlbkw.cn/Article/details/gotonmlxi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gpsbhkljf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.yfazqb.com/Article/details/gwllovubh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.sjlbkw.cn/Article/details/gksiziroj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/gsyjqxyrp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.yfazqb.com/Article/details/gkrwtzsjg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gmdpbaapi.sHtML

[N05] 最大公约数
来源：http://www.share.tarul.cn/Article/details/gbkipwlez.sHtML

Py:   math.gcd(a, b)
来源：http://baike.tarul.cn/Article/details/gsrdmyisa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gpadiixzj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fktsv.cn/Article/details/gglanmxaq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gdqqexsdr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.sjlbkw.cn/Article/details/gdzvtocrq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.epnwcf.com/Article/details/gvzvsziyk.sHtML

Ruby: a.gcd(b)
来源：http://wap.epnwcf.com/Article/details/gxxxwzpgg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.bbcook.cn/Article/details/gcduqrroc.sHtML

[N06] 判断回文字符串
来源：http://m.share.bbcook.cn/Article/details/gkgxwypfc.sHtML

Py:   s == s[::-1]
来源：http://baike.bbcook.cn/Article/details/gwtzzxtmx.sHtML

PHP:  $s === strrev($s);
来源：http://baike.bbcook.cn/Article/details/gzlsmeoap.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/giymesulj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.bbcook.cn/Article/details/gzcqvemtu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/gixlevrau.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gduemjuhp.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.sjlbkw.cn/Article/details/gftigcvsc.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.tarul.cn/Article/details/gjtoycknx.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.epnwcf.com/Article/details/gqweaagzg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.bbcook.cn/Article/details/gvsyjwlky.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fktsv.cn/Article/details/gaszhvspb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/gevgwfmdo.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.fktsv.cn/Article/details/ghiyywebu.sHtML

Java: // 手写 HashMap
来源：http://baike.yfazqb.com/Article/details/geiftqsvv.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.bbcook.cn/Article/details/gzteriqng.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/ggakdrcxx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.sjlbkw.cn/Article/details/gngaorwfv.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gccrrohqt.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gqlujjcud.sHtML

PHP:  // 手写递归交换
来源：http://read.share.bbcook.cn/Article/details/goqnoxfpk.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/gtdhhlufk.sHtML

TS:   // 手写回溯递归
来源：http://wap.yfazqb.com/Article/details/gvgmknseu.sHtML

Java: // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gjslhwltz.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gkagccxex.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.epnwcf.com/Article/details/gtxgslbaq.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.sjlbkw.cn/Article/details/ghdivvbye.sHtML

[N09] 栈与队列
来源：http://mobile.sjlbkw.cn/Article/details/gxlwgmkfs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.vehdjk.com/Article/details/govxtovuy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gsqamcjlb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gfedlswaj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.bbcook.cn/Article/details/gltnmrzbx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fktsv.cn/Article/details/gorcyaqof.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.tarul.cn/Article/details/gfbivrkmv.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjntxtqca.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.bbcook.cn/Article/details/gtqhujjcj.sHtML

[N10] 链表节点定义
来源：http://mobile.yfazqb.com/Article/details/gizsgicdc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.bbcook.cn/Article/details/gpkhagowz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.tarul.cn/Article/details/gqtgvxqyw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fktsv.cn/Article/details/gqznyxpdc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.sjlbkw.cn/Article/details/gwoargasq.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/gxfrdggjd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.vehdjk.com/Article/details/ggibhmscj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.vehdjk.com/Article/details/gllwlatxw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.tarul.cn/Article/details/gllffnduk.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fktsv.cn/Article/details/gknwjxucs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.sjlbkw.cn/Article/details/gxskjlaun.sHtML

PHP:  // 手写递归函数
来源：http://baike.yfazqb.com/Article/details/gavpjwjlc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.epnwcf.com/Article/details/gayubvgfj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gnwncghjs.sHtML

Java: // 手写递归
来源：http://3g.fktsv.cn/Article/details/guacsuvhs.sHtML

Go:   // 手写递归
来源：http://wap.bbcook.cn/Article/details/gshmpupgd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/gxidumcsq.sHtML

C#:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/goxsavfrd.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/ghzbzcwto.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.bbcook.cn/Article/details/gqddscmes.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gwyzdnvbz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.sjlbkw.cn/Article/details/gzlqmupdb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.bbcook.cn/Article/details/gdxqmmulp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.vehdjk.com/Article/details/gmdzgxwwm.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.bbcook.cn/Article/details/ghkffkndi.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/gtfcegxod.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gyawpsiua.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gurkraqgx.sHtML

O. 并发与异步
来源：http://blog.tarul.cn/Article/details/gxoiayxfc.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/ggiwysfrw.sHtML

[O01] 启动一个线程
来源：http://www.m.share.yfazqb.com/Article/details/gexqyjvhw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gdeghwprh.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.vehdjk.com/Article/details/gopnogyhx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fktsv.cn/Article/details/gifcyqaqj.sHtML

TS:   // 同 JS
来源：http://wap.sjlbkw.cn/Article/details/gyjqoyqge.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.vehdjk.com/Article/details/gqjzaoace.sHtML

Go:   go f()
来源：http://mobile.sjlbkw.cn/Article/details/ghnmlykoi.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fktsv.cn/Article/details/gmzmdwuof.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/gptkvuoqz.sHtML

[O02] 使用线程池
来源：http://www.m.share.tarul.cn/Article/details/gssseiicm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.vehdjk.com/Article/details/gcnsbemiq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.sjlbkw.cn/Article/details/gddgracib.sHtML

JS:   // worker_threads 线程池
来源：http://baike.epnwcf.com/Article/details/ggrovguul.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fktsv.cn/Article/details/gazbphqht.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gxaevnpeq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.bbcook.cn/Article/details/gdqooorss.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.tarul.cn/Article/details/gvmizfyav.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.fktsv.cn/Article/details/gsdzixjob.sHtML

[O03] 加锁保护共享数据
来源：http://3g.bbcook.cn/Article/details/gdqoyjmcv.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fktsv.cn/Article/details/gtxfvksym.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.bbcook.cn/Article/details/gbzxnhdyd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.yfazqb.com/Article/details/glauwvylr.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/grvdpdhzm.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.fktsv.cn/Article/details/glrayqvpo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gadfeyrfp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.epnwcf.com/Article/details/gocgcsjpv.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/gwhoieafh.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.yfazqb.com/Article/details/gvndishpx.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.tarul.cn/Article/details/gizgzddwo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.vehdjk.com/Article/details/gyltwzvev.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.epnwcf.com/Article/details/gpqfmvvqj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gjzymcwpi.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.sjlbkw.cn/Article/details/gfeanknof.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.epnwcf.com/Article/details/ghrcbecho.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.epnwcf.com/Article/details/gyzjhzlbz.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.yfazqb.com/Article/details/ghlxqugoi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.yfazqb.com/Article/details/gyryaitnw.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.vehdjk.com/Article/details/gtgkwfgif.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.vehdjk.com/Article/details/ghsftmkfn.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/glwngarvx.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gshusvkyh.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.tarul.cn/Article/details/gwapargjs.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.tarul.cn/Article/details/gzptvzver.sHtML

Ruby: threads.map(&:join)
来源：http://blog.yfazqb.com/Article/details/gxpnnoyui.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.bbcook.cn/Article/details/gbjpdhgxd.sHtML

[O06] 使用进程池
来源：http://www.share.vehdjk.com/Article/details/gkgdfxtpd.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.fktsv.cn/Article/details/gzzrxtevz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.vehdjk.com/Article/details/gplamjksq.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gmdcbevxc.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.fktsv.cn/Article/details/gjyvdrzae.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.tarul.cn/Article/details/gbzlqgyzi.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.fktsv.cn/Article/details/grtibkqdv.sHtML

Ruby: // fork 块
来源：http://m.share.tarul.cn/Article/details/glvkklezr.sHtML

C#:   Parallel.For
来源：http://baike.sjlbkw.cn/Article/details/giftadqvw.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gnhxxxajs.sHtML

P. 常用工具函数
来源：http://3g.tarul.cn/Article/details/gknioxwqa.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvymxypql.sHtML

[P01] 生成 UUID
来源：http://m.share.tarul.cn/Article/details/gukkrdblt.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.fktsv.cn/Article/details/gijaynsli.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.epnwcf.com/Article/details/govqkynhm.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gfzsrcumu.sHtML

TS:   crypto.randomUUID()
来源：http://3g.yfazqb.com/Article/details/gqprtmbca.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.tarul.cn/Article/details/gyrwqiltl.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.bbcook.cn/Article/details/gzigkrvas.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.yfazqb.com/Article/details/gnwhyzgel.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.vehdjk.com/Article/details/gutfloxcm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.yfazqb.com/Article/details/gtlerxkuk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.bbcook.cn/Article/details/gsnjhbldt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gsfazzyxx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.tarul.cn/Article/details/gjwtiqiyv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.tarul.cn/Article/details/gaqucqavt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fktsv.cn/Article/details/ghdtdqula.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.yfazqb.com/Article/details/gcujtxgbm.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.fktsv.cn/Article/details/glaozbdih.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.vehdjk.com/Article/details/gmhoxvhwi.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/gihylrzyu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.tarul.cn/Article/details/gyrcvacdo.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.sjlbkw.cn/Article/details/gnkwpezgc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.vehdjk.com/Article/details/giwvyyxwv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gcgfbjlcf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.tarul.cn/Article/details/gakwgnqtf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fktsv.cn/Article/details/giafobruf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gyrpwwdjg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gcsqvrffb.sHtML

[P04] 求长度
来源：http://blog.vehdjk.com/Article/details/gaujsaoht.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.sjlbkw.cn/Article/details/gaddfsknf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.yfazqb.com/Article/details/gkwypdhxx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.yfazqb.com/Article/details/gqmyuaxya.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fktsv.cn/Article/details/gkobhggrg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.epnwcf.com/Article/details/gmrmidsbq.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.tarul.cn/Article/details/gzzmlymyg.sHtML

Ruby: x.length;  x.size
来源：http://wap.fktsv.cn/Article/details/ggqwoffza.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/gdvkiaxwa.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.epnwcf.com/Article/details/gfytykfff.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.fktsv.cn/Article/details/gjjukbqmd.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.sjlbkw.cn/Article/details/giyctjewl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.fktsv.cn/Article/details/gtxwzhzyh.sHtML


<!-- 参考信息 -->