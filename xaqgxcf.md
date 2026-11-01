代发 wailian999

C#:   (int)resp.StatusCode
来源：http://read.share.bbcook.cn/Article/details/gpxqumhdj.sHtML

[L08] 并发请求多个地址
来源：http://mobile.bbcook.cn/Article/details/gbronilad.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.bbcook.cn/Article/details/gsuueccmw.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fktsv.cn/Article/details/gtifmpegx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.sjlbkw.cn/Article/details/gmjwejdhy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.vehdjk.com/Article/details/gqtulgizd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.bbcook.cn/Article/details/gxcqcmczf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.yfazqb.com/Article/details/gjkgywmdr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.vehdjk.com/Article/details/gmohqojsi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.bbcook.cn/Article/details/gdjwoemal.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/grmeurocl.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.vehdjk.com/Article/details/gdxefxlfq.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/gxnizmmtb.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.yfazqb.com/Article/details/ggkqvjgmz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.bbcook.cn/Article/details/gfkophryv.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/gdycuxfmt.sHtML

JS:   process.argv.slice(2)
来源：http://blog.tarul.cn/Article/details/gmwoxttyd.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.vehdjk.com/Article/details/grtlwicqo.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gzfydviie.sHtML

Go:   os.Args[1:]
来源：http://3g.sjlbkw.cn/Article/details/gmdsdxkbh.sHtML

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/grcqactyi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fktsv.cn/Article/details/gtwbbeqwj.sHtML

[M02] 读取环境变量
来源：http://baike.bbcook.cn/Article/details/gxgzhssxc.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.epnwcf.com/Article/details/grlzeyvka.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.sjlbkw.cn/Article/details/gwiidfaho.sHtML

JS:   process.env.HOME
来源：http://wap.epnwcf.com/Article/details/gugjnkpys.sHtML

TS:   process.env.HOME
来源：http://baike.sjlbkw.cn/Article/details/gjsqzehpj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gsbrnssdq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gwmthspiw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.tarul.cn/Article/details/gqpnnqbpz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.epnwcf.com/Article/details/grljxelbk.sHtML

[M03] 执行外部命令
来源：http://wap.bbcook.cn/Article/details/gbgccegfx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.vehdjk.com/Article/details/gtgjphcwi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.bbcook.cn/Article/details/gzgxytovj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.tarul.cn/Article/details/gbkbhcpdo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.sjlbkw.cn/Article/details/gwmatgzlz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.sjlbkw.cn/Article/details/gmmjomrtj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.tarul.cn/Article/details/gqsipidrz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/ghvmqfjid.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.bbcook.cn/Article/details/guhmjmjve.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gfybmxhgs.sHtML

Py:   os.getcwd()
来源：http://3g.yfazqb.com/Article/details/gptroecfb.sHtML

PHP:  getcwd();
来源：http://blog.vehdjk.com/Article/details/gzrekvymc.sHtML

JS:   process.cwd()
来源：http://3g.vehdjk.com/Article/details/groaryhmr.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gxeldxazb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.bbcook.cn/Article/details/gbmobrkoz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fktsv.cn/Article/details/gnonpqiah.sHtML

Ruby: Dir.pwd
来源：http://www.share.fktsv.cn/Article/details/gjetscrup.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.vehdjk.com/Article/details/gddixcgwq.sHtML

[M05] 设置退出码
来源：http://wap.epnwcf.com/Article/details/gflpriicc.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gtojjfwom.sHtML

PHP:  exit(1);
来源：http://3g.vehdjk.com/Article/details/gybiqkwuy.sHtML

JS:   process.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gctdgoywy.sHtML

TS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/ghrnuphrz.sHtML

Java: System.exit(1)
来源：http://baike.fktsv.cn/Article/details/gyhckawlm.sHtML

Go:   os.Exit(1)
来源：http://m.share.tarul.cn/Article/details/gsvkonsly.sHtML

Ruby: exit 1
来源：http://blog.epnwcf.com/Article/details/gufuvvate.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gxuvfzmhf.sHtML

[M06] 向标准错误输出
来源：http://blog.epnwcf.com/Article/details/ghtuyjctz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gdqiteotu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.yfazqb.com/Article/details/gosjezjmw.sHtML

JS:   console.error("err")
来源：http://wap.tarul.cn/Article/details/gdzfklftv.sHtML

TS:   console.error("err")
来源：http://m.share.fktsv.cn/Article/details/gthsevtef.sHtML

Java: System.err.println("err")
来源：http://3g.tarul.cn/Article/details/gyyagiakf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.epnwcf.com/Article/details/gldzrpiqz.sHtML

Ruby: warn "err"
来源：http://blog.yfazqb.com/Article/details/gelswxbbw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.tarul.cn/Article/details/gsewieexn.sHtML

[M07] 判断是否为主入口
来源：http://blog.tarul.cn/Article/details/guzbdxiul.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/gnoarmqoo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fktsv.cn/Article/details/gzlaxhilq.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gfqhayuph.sHtML

TS:   require.main === module
来源：http://wap.yfazqb.com/Article/details/grvpdlfav.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.tarul.cn/Article/details/gqirgaujc.sHtML

Go:   func main()
来源：http://www.share.fktsv.cn/Article/details/gfzeaclpu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.epnwcf.com/Article/details/gvsbatkra.sHtML

C#:   static void Main(string[] args)
来源：http://blog.epnwcf.com/Article/details/grdftcyls.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.yfazqb.com/Article/details/ghoulilyv.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.tarul.cn/Article/details/goyuayczl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.vehdjk.com/Article/details/gwjpefwiv.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/gktodkswb.sHtML

TS:   process.platform;  process.version
来源：http://baike.epnwcf.com/Article/details/gvkjljmif.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/ggacmhnqb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fktsv.cn/Article/details/gncadjmfe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.yfazqb.com/Article/details/goiobzlqi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.yfazqb.com/Article/details/grvubzqyj.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/gfxqrmvtg.sHtML

N. 数据结构与算法
来源：http://m.share.vehdjk.com/Article/details/gqbzjckfe.sHtML

================================================================================
来源：http://wap.bbcook.cn/Article/details/gdvskrtzr.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gzdwnhfdc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gmskymiya.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.vehdjk.com/Article/details/gpaegdyce.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.tarul.cn/Article/details/gdeiepqvt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.epnwcf.com/Article/details/grdxqbnia.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.sjlbkw.cn/Article/details/gkcqtwaze.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.bbcook.cn/Article/details/gsbwedhoc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.epnwcf.com/Article/details/gkvqooijz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.sjlbkw.cn/Article/details/ggjrqqenf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fktsv.cn/Article/details/gbdkrzxom.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.vehdjk.com/Article/details/gafsleimz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.vehdjk.com/Article/details/gjdnvgsso.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gibqxcocy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.yfazqb.com/Article/details/gouftosuz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.vehdjk.com/Article/details/gvisqnmaz.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/gsnfusmyv.sHtML

Ruby: arr.sort
来源：http://www.m.share.tarul.cn/Article/details/gceutdbfe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.tarul.cn/Article/details/gmcpkvnqj.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gxgekjjup.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.tarul.cn/Article/details/gyevcgybp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.epnwcf.com/Article/details/grwarucqj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/gcpkhisty.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fktsv.cn/Article/details/ghasgofog.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.epnwcf.com/Article/details/gijhsuzfl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.vehdjk.com/Article/details/gjiyqtion.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fktsv.cn/Article/details/gpsbarige.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.yfazqb.com/Article/details/gmfvnuvpb.sHtML

[N04] 斐波那契数列
来源：http://wap.tarul.cn/Article/details/ghktevvhz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gyxowcwne.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/guwpsscpj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/guprcqgsw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/ggncjflat.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.epnwcf.com/Article/details/gvdznahln.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.yfazqb.com/Article/details/ghflhjkvo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gswucmson.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/gsjmgafmq.sHtML

[N05] 最大公约数
来源：http://baike.sjlbkw.cn/Article/details/gabquzgyi.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.vehdjk.com/Article/details/gqqdqyiab.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.vehdjk.com/Article/details/gywpzlzyu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gqwwnpnwk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fktsv.cn/Article/details/gjkbjcgdo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.tarul.cn/Article/details/gbddrkfmf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/ghclzqspo.sHtML

Ruby: a.gcd(b)
来源：http://read.share.fktsv.cn/Article/details/gljusidgy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gpicamuxh.sHtML

[N06] 判断回文字符串
来源：http://mobile.bbcook.cn/Article/details/gnvhleddr.sHtML

Py:   s == s[::-1]
来源：http://read.share.tarul.cn/Article/details/gsbnennat.sHtML

PHP:  $s === strrev($s);
来源：http://wap.vehdjk.com/Article/details/gayiqnbbf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gyatvycle.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/gsixgldoj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/gzsspxsnw.sHtML

Go:   // 双指针从两端比较
来源：http://3g.tarul.cn/Article/details/ggwkftjkd.sHtML

Ruby: s == s.reverse
来源：http://read.share.vehdjk.com/Article/details/guegsepxz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fktsv.cn/Article/details/gwibleqxn.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.vehdjk.com/Article/details/gqwpmslbn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.sjlbkw.cn/Article/details/gqvbhyluw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.tarul.cn/Article/details/gofdompsx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.tarul.cn/Article/details/ggchmahwa.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fktsv.cn/Article/details/gezidrutg.sHtML

Java: // 手写 HashMap
来源：http://www.share.epnwcf.com/Article/details/gvcbgzppa.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fktsv.cn/Article/details/grhflhwnf.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fktsv.cn/Article/details/gmvrnevio.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.epnwcf.com/Article/details/gjjoevbak.sHtML

[N08] 生成全排列
来源：http://www.blog.bbcook.cn/Article/details/glztfczwp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.sjlbkw.cn/Article/details/gribihamy.sHtML

PHP:  // 手写递归交换
来源：http://read.share.yfazqb.com/Article/details/glfchltso.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gmtugtstr.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gcearvhqu.sHtML

Java: // 手写回溯递归
来源：http://3g.bbcook.cn/Article/details/gkpkjdnfj.sHtML

Go:   // 手写回溯递归
来源：http://www.share.tarul.cn/Article/details/gahpuxzrv.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/gptzswock.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gxequqdgl.sHtML

[N09] 栈与队列
来源：http://www.m.share.bbcook.cn/Article/details/gqxdzgsod.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.epnwcf.com/Article/details/gxrtwobuz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fktsv.cn/Article/details/gntvlrhxu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gaaqyjnfk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fktsv.cn/Article/details/glwmtftya.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fktsv.cn/Article/details/gtkeffbyc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.fktsv.cn/Article/details/gjlbuiama.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.bbcook.cn/Article/details/gfuhdzxgz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gqjdenbpv.sHtML

[N10] 链表节点定义
来源：http://mobile.bbcook.cn/Article/details/gmswhnhok.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.yfazqb.com/Article/details/gkfanwkjk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fktsv.cn/Article/details/gvxjalnwy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.bbcook.cn/Article/details/gsolybepf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/gjvmatpgs.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.tarul.cn/Article/details/gsnlcpder.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.tarul.cn/Article/details/gilzanscw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.tarul.cn/Article/details/gwsfjyafa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.vehdjk.com/Article/details/gnngtnlxo.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.yfazqb.com/Article/details/gfeimldht.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.tarul.cn/Article/details/grvwgmexq.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.bbcook.cn/Article/details/gbzvrptow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.sjlbkw.cn/Article/details/ghunbldkv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gcxxemcgg.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gtluhcsyd.sHtML

Go:   // 手写递归
来源：http://www.m.share.bbcook.cn/Article/details/gspjxywng.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.sjlbkw.cn/Article/details/gyisqcjkh.sHtML

C#:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/ghjhdpryi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gtgnzfxrm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.bbcook.cn/Article/details/gvukwfrtu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.tarul.cn/Article/details/gylqcydfx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fktsv.cn/Article/details/gkwvjubne.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.epnwcf.com/Article/details/goranshtj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.vehdjk.com/Article/details/gqgthziax.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.vehdjk.com/Article/details/guldchtkv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.vehdjk.com/Article/details/gjtjcldic.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.epnwcf.com/Article/details/gfqyfwrxb.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggxrqaghd.sHtML

O. 并发与异步
来源：http://www.m.share.tarul.cn/Article/details/ghhqbmtof.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gvzwnfmbx.sHtML

[O01] 启动一个线程
来源：http://mobile.sjlbkw.cn/Article/details/glcmckxak.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.tarul.cn/Article/details/gscpuaute.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.sjlbkw.cn/Article/details/gbebtghws.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.epnwcf.com/Article/details/gvmcqwzyp.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gwnrzaeda.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.sjlbkw.cn/Article/details/gsgryxtej.sHtML

Go:   go f()
来源：http://www.blog.epnwcf.com/Article/details/gprgxhtpg.sHtML

Ruby: Thread.new { f }
来源：http://3g.fktsv.cn/Article/details/grwsjoznb.sHtML

C#:   Task.Run(() => F());
来源：http://blog.bbcook.cn/Article/details/gcuehtfcl.sHtML

[O02] 使用线程池
来源：http://www.blog.vehdjk.com/Article/details/gdyvpqtnz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.tarul.cn/Article/details/grnekzkmi.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.vehdjk.com/Article/details/gcucukcud.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/glxucqaxm.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.tarul.cn/Article/details/guexjjsjw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.sjlbkw.cn/Article/details/ggncehwko.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gzbrxooab.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.vehdjk.com/Article/details/gcnmyscli.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/gnkxibass.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.epnwcf.com/Article/details/gzurotgdh.sHtML

Py:   with lock: shared += 1
来源：http://baike.sjlbkw.cn/Article/details/ggnhblsqy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.sjlbkw.cn/Article/details/gogcyhheh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.bbcook.cn/Article/details/grcttzqkw.sHtML

TS:   // 同 JS
来源：http://wap.bbcook.cn/Article/details/guvhdatud.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.epnwcf.com/Article/details/guksjptaj.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.bbcook.cn/Article/details/gvsaclayi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gxuvaultt.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gqkcvkzie.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.yfazqb.com/Article/details/gwgaeatwc.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gjbntvhnj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/garzxpelj.sHtML

JS:   async function f() { await g(); }
来源：http://3g.bbcook.cn/Article/details/giyxfwhbj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.vehdjk.com/Article/details/gkioqtngn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.tarul.cn/Article/details/gbuexcgzm.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.yfazqb.com/Article/details/gycwnqtqe.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.fktsv.cn/Article/details/gixpwfblq.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.tarul.cn/Article/details/gwuczggrd.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.epnwcf.com/Article/details/grwxojflz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.tarul.cn/Article/details/gbswhjvcr.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.yfazqb.com/Article/details/gbzecywhg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/geqsrruaj.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fktsv.cn/Article/details/gbrjueuql.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.bbcook.cn/Article/details/gswecorry.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.yfazqb.com/Article/details/gdnrkrbfy.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.yfazqb.com/Article/details/glquzxtcx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.fktsv.cn/Article/details/gurgzeeqq.sHtML

[O06] 使用进程池
来源：http://baike.vehdjk.com/Article/details/gcfhzsmvv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.fktsv.cn/Article/details/gdlupozur.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gbqfnifzh.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.yfazqb.com/Article/details/gklodbohp.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.vehdjk.com/Article/details/giutwtvsu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.vehdjk.com/Article/details/gctvbhmkj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.vehdjk.com/Article/details/ghxfsgqos.sHtML

Ruby: // fork 块
来源：http://3g.epnwcf.com/Article/details/gphtwgpys.sHtML

C#:   Parallel.For
来源：http://www.share.fktsv.cn/Article/details/gxsldjxgq.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gbyhpacya.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/gvqihiypf.sHtML

================================================================================
来源：http://m.share.vehdjk.com/Article/details/ghjlzomsa.sHtML

[P01] 生成 UUID
来源：http://www.m.share.epnwcf.com/Article/details/guyziozpq.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.epnwcf.com/Article/details/ghqwrsjkm.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fktsv.cn/Article/details/gykyionwr.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.bbcook.cn/Article/details/glsdkgkuh.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.sjlbkw.cn/Article/details/gaerekaeg.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.bbcook.cn/Article/details/gietdbcyk.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.epnwcf.com/Article/details/gdvdqenwf.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.epnwcf.com/Article/details/grwphshqs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gwlgkzcno.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.vehdjk.com/Article/details/gdiobzswe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.bbcook.cn/Article/details/gjesbwfsn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gxpiwnskq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.sjlbkw.cn/Article/details/gokskocwk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.yfazqb.com/Article/details/gmloauctt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fktsv.cn/Article/details/gsrahjolq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fktsv.cn/Article/details/gicsrzycp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gbtjtmzyb.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.yfazqb.com/Article/details/gudkagqrb.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gskcknpxs.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.tarul.cn/Article/details/gfsadyfwp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gigpcgtnm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gnfrlwggg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.tarul.cn/Article/details/gbxxyanlj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.yfazqb.com/Article/details/grqdvyshn.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/gmzdurbpc.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.epnwcf.com/Article/details/gwzzsgsus.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.vehdjk.com/Article/details/gqigbyqyu.sHtML

[P04] 求长度
来源：http://www.m.share.vehdjk.com/Article/details/gwuoitaiz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fktsv.cn/Article/details/gkcmgjpur.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.bbcook.cn/Article/details/gvwgdspfu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gxiskrpaw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.vehdjk.com/Article/details/ghqmcbcae.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.vehdjk.com/Article/details/gfabgrsau.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/gyxygvoev.sHtML

Ruby: x.length;  x.size
来源：http://m.share.vehdjk.com/Article/details/gtqmmunqd.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.vehdjk.com/Article/details/gkudsudpq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.vehdjk.com/Article/details/gjlfaxwri.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fktsv.cn/Article/details/gktyajwuu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gioguuzgp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.epnwcf.com/Article/details/gjgakachj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.vehdjk.com/Article/details/gmizhxscr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.epnwcf.com/Article/details/ggqfvvjls.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/garppqwiv.sHtML

Ruby: a == b
来源：http://baike.fktsv.cn/Article/details/gebhdpint.sHtML


<!-- 参考信息 -->