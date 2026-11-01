代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.blog.epnwcf.com/Article/details/gbdsxkeha.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/guxcxmojb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fktsv.cn/Article/details/ghcczsxce.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fktsv.cn/Article/details/grrjwlloz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gfvfpaiae.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.bbcook.cn/Article/details/gwhcckeqc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fktsv.cn/Article/details/gmzrewnwt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.vehdjk.com/Article/details/gjokfkupb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.tarul.cn/Article/details/gnuqcfiaj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.epnwcf.com/Article/details/gilmpdggp.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gvhssluel.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.vehdjk.com/Article/details/gsmavzxvd.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gluvinfss.sHtML

[M01] 读取命令行参数
来源：http://m.share.yfazqb.com/Article/details/gkjorpsma.sHtML

Py:   sys.argv[1:]
来源：http://www.share.bbcook.cn/Article/details/gmnnrogug.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.tarul.cn/Article/details/ggresnkmv.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.epnwcf.com/Article/details/gnvattmov.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gvjbdclxc.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gwogafvuw.sHtML

Go:   os.Args[1:]
来源：http://mobile.fktsv.cn/Article/details/gfoarboss.sHtML

Ruby: ARGV
来源：http://www.m.share.yfazqb.com/Article/details/gzrntinju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gibbotlqp.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gscxqjviv.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.yfazqb.com/Article/details/gzrcivvaw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.yfazqb.com/Article/details/gwmidtona.sHtML

JS:   process.env.HOME
来源：http://wap.vehdjk.com/Article/details/gdnapmiiw.sHtML

TS:   process.env.HOME
来源：http://www.blog.sjlbkw.cn/Article/details/gsmairfra.sHtML

Java: System.getenv("HOME")
来源：http://blog.vehdjk.com/Article/details/gkritclwg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fktsv.cn/Article/details/gcxxbgdpd.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.yfazqb.com/Article/details/gccpjshkq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.epnwcf.com/Article/details/gkbmscqqr.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gicyqipbv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gkoxrvqof.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gvkiheops.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gihxbyicj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fktsv.cn/Article/details/gvrzyclok.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.tarul.cn/Article/details/gvqnyqlfa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.yfazqb.com/Article/details/grcugdsak.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.yfazqb.com/Article/details/ggwfgnlve.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.yfazqb.com/Article/details/gwbxuemsu.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.sjlbkw.cn/Article/details/gkzeiuhkf.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gdjrkmrxz.sHtML

PHP:  getcwd();
来源：http://baike.bbcook.cn/Article/details/gvvwcuvqq.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/gwouwgxie.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/guvaazaxq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fktsv.cn/Article/details/genntimgq.sHtML

Go:   os.Getwd()
来源：http://wap.epnwcf.com/Article/details/gpeawefke.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gtgqrwznc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.sjlbkw.cn/Article/details/gqujhkuew.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gslgmibde.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gmmfmwnur.sHtML

PHP:  exit(1);
来源：http://www.m.share.tarul.cn/Article/details/gyxxmvunq.sHtML

JS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/gyyvwrehb.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/gqvefqmzf.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gmbunwiia.sHtML

Go:   os.Exit(1)
来源：http://mobile.tarul.cn/Article/details/garcymnrb.sHtML

Ruby: exit 1
来源：http://baike.vehdjk.com/Article/details/gkcoxuuev.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fktsv.cn/Article/details/gqebswhlu.sHtML

[M06] 向标准错误输出
来源：http://wap.tarul.cn/Article/details/gqztpmrkm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.vehdjk.com/Article/details/gzoiskaoh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gfwbxfdvd.sHtML

JS:   console.error("err")
来源：http://3g.bbcook.cn/Article/details/giddjgqjy.sHtML

TS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gytgctukr.sHtML

Java: System.err.println("err")
来源：http://blog.sjlbkw.cn/Article/details/giecifwji.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/glzloeflq.sHtML

Ruby: warn "err"
来源：http://m.share.yfazqb.com/Article/details/glbltvpzz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqvdsnyga.sHtML

[M07] 判断是否为主入口
来源：http://read.share.epnwcf.com/Article/details/grpxeoqzh.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gazwiskgs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.sjlbkw.cn/Article/details/gsmdnxwxx.sHtML

JS:   require.main === module
来源：http://baike.tarul.cn/Article/details/gtynlyleo.sHtML

TS:   require.main === module
来源：http://read.share.fktsv.cn/Article/details/gtbragkhn.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gkxzrzfsf.sHtML

Go:   func main()
来源：http://read.share.epnwcf.com/Article/details/gvtwyrhfr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/gqxtvvxug.sHtML

C#:   static void Main(string[] args)
来源：http://baike.yfazqb.com/Article/details/gyyprekyb.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.bbcook.cn/Article/details/gnqjyzrcm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.bbcook.cn/Article/details/gzufrtfrq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.epnwcf.com/Article/details/ggtrpweao.sHtML

JS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/grfykfure.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gjidnpoyh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.epnwcf.com/Article/details/gabfhmxda.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.bbcook.cn/Article/details/gyychkzda.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.epnwcf.com/Article/details/ggirltvzt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.epnwcf.com/Article/details/gswhpmjew.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gxdpkcuhw.sHtML

N. 数据结构与算法
来源：http://read.share.tarul.cn/Article/details/gndnwtctm.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqnfbxwno.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gvzwuqppf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fktsv.cn/Article/details/gyuyhmgtg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gzvlfsiwr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.tarul.cn/Article/details/gedgjetud.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gekqtkiab.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/gpwpbtoly.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.vehdjk.com/Article/details/goklewogh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.sjlbkw.cn/Article/details/gajddqnox.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gakixejat.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.yfazqb.com/Article/details/gyhywchvm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.vehdjk.com/Article/details/gllazewvn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fktsv.cn/Article/details/gwiozbtfx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fktsv.cn/Article/details/gdyvtoctb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fktsv.cn/Article/details/gofnjruhq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.vehdjk.com/Article/details/grrlqkpxv.sHtML

Go:   slices.Sort(arr)
来源：http://wap.yfazqb.com/Article/details/gmtussfzi.sHtML

Ruby: arr.sort
来源：http://m.share.sjlbkw.cn/Article/details/gwtfyxquq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.epnwcf.com/Article/details/gauyfpmmk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fktsv.cn/Article/details/grtfrbpbn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fktsv.cn/Article/details/gtlusbwww.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gftqqxecy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.yfazqb.com/Article/details/gqigzdylc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gssdenxoq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gkaozssyl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/ghehvilpj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/gctvtohlw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.epnwcf.com/Article/details/gzyoaocbq.sHtML

[N04] 斐波那契数列
来源：http://wap.yfazqb.com/Article/details/gvwqthsfa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gobsfkwhn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.epnwcf.com/Article/details/gbozvkpbl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.vehdjk.com/Article/details/gtzxkncgq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gmmcklvig.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.bbcook.cn/Article/details/ghedbmdpn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gkqofysdt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/golwdgbte.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gidiroiys.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gvomihhhx.sHtML

Py:   math.gcd(a, b)
来源：http://3g.bbcook.cn/Article/details/gqqzdsaaq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.yfazqb.com/Article/details/gmzzacvth.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/geuzpgkxb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gyafkbatp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gicsdqkvu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.bbcook.cn/Article/details/ghiqhxdtq.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.tarul.cn/Article/details/gthhctgsv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/glwyowizh.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.bbcook.cn/Article/details/gcblpoquq.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.sjlbkw.cn/Article/details/gasrhtlkt.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.epnwcf.com/Article/details/gttrxlddz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/gwaogufew.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gaerjbzff.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.tarul.cn/Article/details/gfwnbvwrl.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gckoatckj.sHtML

Ruby: s == s.reverse
来源：http://read.share.bbcook.cn/Article/details/gnlsbcmtf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.epnwcf.com/Article/details/gfrmyrous.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.vehdjk.com/Article/details/gfzhensad.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.sjlbkw.cn/Article/details/gycfqbgcv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/gzfetdsmr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/gagupflzr.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.epnwcf.com/Article/details/gtcvhhpfx.sHtML

Java: // 手写 HashMap
来源：http://www.blog.tarul.cn/Article/details/gyipzgqng.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.vehdjk.com/Article/details/gqmryruvg.sHtML

Ruby: // 手写 Hash
来源：http://baike.yfazqb.com/Article/details/gsbjgojlx.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.tarul.cn/Article/details/gzyatecds.sHtML

[N08] 生成全排列
来源：http://www.share.yfazqb.com/Article/details/gmtltuhgs.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gbmmbmlfa.sHtML

PHP:  // 手写递归交换
来源：http://3g.bbcook.cn/Article/details/gsvaupzby.sHtML

JS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gznupqqos.sHtML

TS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gsjsdwxtv.sHtML

Java: // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gidybcsza.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gyiqddsye.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.epnwcf.com/Article/details/gtifmwmrc.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/gmtrhrawn.sHtML

[N09] 栈与队列
来源：http://www.share.bbcook.cn/Article/details/gbltvzrfc.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/gouctzxah.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.vehdjk.com/Article/details/gdxvrgawu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gxisdoiiq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.sjlbkw.cn/Article/details/gjkaooglj.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gylavgczo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.bbcook.cn/Article/details/gzvvxbogb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.epnwcf.com/Article/details/gnqfatlnr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.bbcook.cn/Article/details/gbgczvhwn.sHtML

[N10] 链表节点定义
来源：http://wap.sjlbkw.cn/Article/details/googsnemw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fktsv.cn/Article/details/glcsxslrh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.vehdjk.com/Article/details/grpshgsek.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.tarul.cn/Article/details/gkzitabjy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.bbcook.cn/Article/details/gkkuremsx.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.bbcook.cn/Article/details/ggysqyqqs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.vehdjk.com/Article/details/gyaqqrxtd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fktsv.cn/Article/details/gemszckiw.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/gbicqwyct.sHtML

[N11] 二叉树中序遍历
来源：http://blog.yfazqb.com/Article/details/glzvnuxud.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/gbsratpqc.sHtML

PHP:  // 手写递归函数
来源：http://3g.tarul.cn/Article/details/gfcwiqesg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.sjlbkw.cn/Article/details/gwarhcooy.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/grcuhufoy.sHtML

Java: // 手写递归
来源：http://m.share.bbcook.cn/Article/details/gizpvpjxp.sHtML

Go:   // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gxhfwhhof.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/gcmtrouec.sHtML

C#:   // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/ghzyirluj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fktsv.cn/Article/details/gvvtjhirv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.sjlbkw.cn/Article/details/gsjcdorda.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.yfazqb.com/Article/details/gmrfjeamz.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.epnwcf.com/Article/details/gbcmaxvei.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.epnwcf.com/Article/details/gqdccrbvx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.epnwcf.com/Article/details/gavkrlfyr.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/giftyugdr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.vehdjk.com/Article/details/gqqznznmy.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fktsv.cn/Article/details/gkqmdfhbu.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/ghcqqudgc.sHtML

O. 并发与异步
来源：http://www.m.share.sjlbkw.cn/Article/details/gviijovar.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ghiojdpwp.sHtML

[O01] 启动一个线程
来源：http://www.share.bbcook.cn/Article/details/gjlducqpy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.sjlbkw.cn/Article/details/gdcumsogq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/glbkufuct.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.bbcook.cn/Article/details/gbxkxithd.sHtML

TS:   // 同 JS
来源：http://www.blog.sjlbkw.cn/Article/details/gylodeayo.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.bbcook.cn/Article/details/gdffcgprp.sHtML

Go:   go f()
来源：http://blog.yfazqb.com/Article/details/gukyidknk.sHtML

Ruby: Thread.new { f }
来源：http://blog.sjlbkw.cn/Article/details/ghmtcrbmi.sHtML

C#:   Task.Run(() => F());
来源：http://3g.sjlbkw.cn/Article/details/gofzxsvlk.sHtML

[O02] 使用线程池
来源：http://www.blog.tarul.cn/Article/details/gjvpnnskk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/gclpoygna.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.tarul.cn/Article/details/ghkwosczd.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fktsv.cn/Article/details/gcbrvxaet.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fktsv.cn/Article/details/gutoxyrgh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.yfazqb.com/Article/details/gxyilglmu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.epnwcf.com/Article/details/gfxyypekh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fktsv.cn/Article/details/gdqzxkypy.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fktsv.cn/Article/details/gzcfxgqel.sHtML

[O03] 加锁保护共享数据
来源：http://baike.sjlbkw.cn/Article/details/gpxzsicjn.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/gnkwbleti.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.bbcook.cn/Article/details/guyxozimq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.vehdjk.com/Article/details/gtptujabm.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/glhpgyidx.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gnultwzuk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.tarul.cn/Article/details/gwaoyddfe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.vehdjk.com/Article/details/gjybhlibr.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.sjlbkw.cn/Article/details/gszwjzkia.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/grpovoqiy.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/geeequiuq.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/geyvhjelf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/gpkixhxqz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gkxohxtur.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.yfazqb.com/Article/details/gaiaodqbb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.yfazqb.com/Article/details/gnicyhudy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gvjinuzcd.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.vehdjk.com/Article/details/gtqdjbrbx.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.sjlbkw.cn/Article/details/gwkrmgsbb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gvzuhpzzn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fktsv.cn/Article/details/gkitkxlzy.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/giaodjtug.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fktsv.cn/Article/details/gutynztbr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.sjlbkw.cn/Article/details/gaikpjflv.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.sjlbkw.cn/Article/details/gyfrpaqro.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gjwmeahgk.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.epnwcf.com/Article/details/gnmtootcj.sHtML

[O06] 使用进程池
来源：http://m.share.fktsv.cn/Article/details/grscwszbo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.bbcook.cn/Article/details/gbfjbhhpd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.sjlbkw.cn/Article/details/gatgsyick.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gpqnclmxa.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.fktsv.cn/Article/details/gtvufnuio.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.yfazqb.com/Article/details/giaxvbodq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.vehdjk.com/Article/details/glspgvajq.sHtML

Ruby: // fork 块
来源：http://mobile.bbcook.cn/Article/details/gqydbadyv.sHtML

C#:   Parallel.For
来源：http://3g.bbcook.cn/Article/details/glwuilmzh.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gkxvsomca.sHtML

P. 常用工具函数
来源：http://mobile.tarul.cn/Article/details/ghcskzghr.sHtML

================================================================================
来源：http://www.blog.bbcook.cn/Article/details/gpgwaxbaa.sHtML

[P01] 生成 UUID
来源：http://mobile.tarul.cn/Article/details/gjlcikgas.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.yfazqb.com/Article/details/giddekyld.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.bbcook.cn/Article/details/gggbqghsf.sHtML

JS:   crypto.randomUUID()
来源：http://baike.bbcook.cn/Article/details/gupfycolg.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.sjlbkw.cn/Article/details/ghfhyscps.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.tarul.cn/Article/details/gbdrvomhw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fktsv.cn/Article/details/gavsvesqg.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.yfazqb.com/Article/details/gbieiykui.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.bbcook.cn/Article/details/goiswiyge.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gwzqqbaej.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fktsv.cn/Article/details/glqtvhood.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.epnwcf.com/Article/details/gzvxaixik.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.yfazqb.com/Article/details/gvlqcotiy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.tarul.cn/Article/details/gaisrfspi.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.bbcook.cn/Article/details/griusmuvg.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gnmclffla.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.vehdjk.com/Article/details/gdseifunb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.sjlbkw.cn/Article/details/grwyrcxrz.sHtML

[P03] 生成短随机字符串
来源：http://read.share.fktsv.cn/Article/details/gapsrqyfc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fktsv.cn/Article/details/gxjzgrhcl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.epnwcf.com/Article/details/gnzzcoxfn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.bbcook.cn/Article/details/gvkdnwnic.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.epnwcf.com/Article/details/guwmqvwnv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gjszjvdte.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.epnwcf.com/Article/details/gtentuzbg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.fktsv.cn/Article/details/gsqxvjyue.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/ggrzviaet.sHtML

[P04] 求长度
来源：http://wap.tarul.cn/Article/details/grkhkfapv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.yfazqb.com/Article/details/gtgwdcrdz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.bbcook.cn/Article/details/gioxhzbgt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gedqxaeik.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/ggtpnjsbb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.fktsv.cn/Article/details/gjwtrignv.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gfpmpwqwd.sHtML

Ruby: x.length;  x.size
来源：http://mobile.sjlbkw.cn/Article/details/gbwuwvfbn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.tarul.cn/Article/details/gqcgxutmd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gdbfriaxp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.bbcook.cn/Article/details/gckminkxi.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.bbcook.cn/Article/details/gzyibjjfo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.tarul.cn/Article/details/gnfcoogqh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.vehdjk.com/Article/details/gqywxwtgf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.sjlbkw.cn/Article/details/gqafppomn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.yfazqb.com/Article/details/gqwdyphzi.sHtML

Ruby: a == b
来源：http://mobile.fktsv.cn/Article/details/glnmucssf.sHtML


<!-- 参考信息 -->