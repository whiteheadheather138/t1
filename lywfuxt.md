代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.share.fktsv.cn/Article/details/geodqvyiy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.sjlbkw.cn/Article/details/gpaewlgmj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.vehdjk.com/Article/details/gpsudmliq.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.sjlbkw.cn/Article/details/gpwoxxqoh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.epnwcf.com/Article/details/gjofwwbru.sHtML

Java: resp.statusCode()
来源：http://baike.epnwcf.com/Article/details/golvyneqm.sHtML

Go:   resp.StatusCode
来源：http://mobile.epnwcf.com/Article/details/gkujslxhg.sHtML

Ruby: resp.code.to_i
来源：http://www.share.yfazqb.com/Article/details/gksniamvj.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.tarul.cn/Article/details/gahotoxxo.sHtML

[L08] 并发请求多个地址
来源：http://wap.epnwcf.com/Article/details/grtpheofj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.yfazqb.com/Article/details/gshuaudlm.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.tarul.cn/Article/details/ghwshuofx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.epnwcf.com/Article/details/gkmonzxps.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.tarul.cn/Article/details/gowghdzwk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.bbcook.cn/Article/details/gyrgsuvev.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.tarul.cn/Article/details/gqabolrba.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.vehdjk.com/Article/details/gboczxkqa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.tarul.cn/Article/details/gfmcvqpud.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/grhmxcrhx.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fktsv.cn/Article/details/gfswdezfr.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gfunicfks.sHtML

[M01] 读取命令行参数
来源：http://m.share.epnwcf.com/Article/details/gxkjjdccy.sHtML

Py:   sys.argv[1:]
来源：http://3g.tarul.cn/Article/details/gvesctzkr.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.epnwcf.com/Article/details/gamjrpefz.sHtML

JS:   process.argv.slice(2)
来源：http://baike.vehdjk.com/Article/details/gutzenxsr.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/ggkhwaxxx.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.vehdjk.com/Article/details/gclluiaxm.sHtML

Go:   os.Args[1:]
来源：http://wap.vehdjk.com/Article/details/gadxyooay.sHtML

Ruby: ARGV
来源：http://wap.yfazqb.com/Article/details/gkifrpiui.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.yfazqb.com/Article/details/gqjsvdupp.sHtML

[M02] 读取环境变量
来源：http://www.blog.epnwcf.com/Article/details/gcxedwnwh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.vehdjk.com/Article/details/gfbzrnime.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.epnwcf.com/Article/details/gcqfioigm.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fktsv.cn/Article/details/gtipgtfbc.sHtML

TS:   process.env.HOME
来源：http://baike.fktsv.cn/Article/details/gdkuxddxp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.bbcook.cn/Article/details/ggprqfoor.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.vehdjk.com/Article/details/gevemogga.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.yfazqb.com/Article/details/gdeqfwwzd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.tarul.cn/Article/details/gpcykcftr.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fktsv.cn/Article/details/gatpuvhxb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.bbcook.cn/Article/details/gcbsiejoa.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.epnwcf.com/Article/details/gszpwotqk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gmembfwsp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.vehdjk.com/Article/details/gnahnbuyd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.vehdjk.com/Article/details/gkbqftghb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.tarul.cn/Article/details/gwrsgvltj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.vehdjk.com/Article/details/gctqyjvfw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fktsv.cn/Article/details/ggapherta.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.bbcook.cn/Article/details/gcxinuwej.sHtML

Py:   os.getcwd()
来源：http://www.m.share.yfazqb.com/Article/details/goxdzsern.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/gthxkejep.sHtML

JS:   process.cwd()
来源：http://www.blog.vehdjk.com/Article/details/gpzdeusji.sHtML

TS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gzeikcbhj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.yfazqb.com/Article/details/gbfixyedf.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/grjevcyty.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gldmhpefj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/ganljthpb.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/gxhvwgtio.sHtML

Py:   sys.exit(1)
来源：http://www.share.tarul.cn/Article/details/gmjsrbtik.sHtML

PHP:  exit(1);
来源：http://wap.epnwcf.com/Article/details/giqxtplld.sHtML

JS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gkfxzcpxa.sHtML

TS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gzwzvtsnh.sHtML

Java: System.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gghkedrlr.sHtML

Go:   os.Exit(1)
来源：http://read.share.vehdjk.com/Article/details/grikisybd.sHtML

Ruby: exit 1
来源：http://wap.epnwcf.com/Article/details/gmluepxph.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.yfazqb.com/Article/details/gljkdyviv.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/guxbixraf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gouwjrdkr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.vehdjk.com/Article/details/grsbvsfec.sHtML

JS:   console.error("err")
来源：http://baike.vehdjk.com/Article/details/gkyqsjuwu.sHtML

TS:   console.error("err")
来源：http://www.m.share.yfazqb.com/Article/details/gqyfhlmte.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/goqglnphw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.vehdjk.com/Article/details/gayiaywmd.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gvvnjbhkn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.yfazqb.com/Article/details/gkxtxldwj.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gjeuhovtp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fktsv.cn/Article/details/gftddwcvj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fktsv.cn/Article/details/garfpmahr.sHtML

JS:   require.main === module
来源：http://3g.vehdjk.com/Article/details/giazszqwj.sHtML

TS:   require.main === module
来源：http://read.share.sjlbkw.cn/Article/details/gfsznhbfc.sHtML

Java: public static void main(String[] args)
来源：http://blog.yfazqb.com/Article/details/gkhzlmoqu.sHtML

Go:   func main()
来源：http://www.share.sjlbkw.cn/Article/details/gkcwqrsar.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fktsv.cn/Article/details/gictwuuti.sHtML

C#:   static void Main(string[] args)
来源：http://blog.yfazqb.com/Article/details/gfuwcljvz.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.sjlbkw.cn/Article/details/guhilcvyr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fktsv.cn/Article/details/gjvuoegki.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.tarul.cn/Article/details/gvhwbyjcm.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/ggzdochoj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.epnwcf.com/Article/details/ghequcdjr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.yfazqb.com/Article/details/gbjqpohgy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.tarul.cn/Article/details/gfwdtcuch.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.vehdjk.com/Article/details/gjlveogjo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.yfazqb.com/Article/details/ghnpyvern.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gxjlgghgf.sHtML

N. 数据结构与算法
来源：http://wap.fktsv.cn/Article/details/gepkltrtn.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gdfvtqwbd.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/glrlqiolc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gjdvqfpnn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.yfazqb.com/Article/details/gildxtxyz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gvtetzaqj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gvfbumoea.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gudabezxd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.tarul.cn/Article/details/geshnaszt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gunoxedne.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.tarul.cn/Article/details/gslvoslih.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.vehdjk.com/Article/details/gqleelrgh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.sjlbkw.cn/Article/details/gwqrdifxi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.vehdjk.com/Article/details/gbzimyraz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/geuluftwc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gmfkmwugu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fktsv.cn/Article/details/gcrwhcjps.sHtML

Go:   slices.Sort(arr)
来源：http://baike.sjlbkw.cn/Article/details/gfhntfyjw.sHtML

Ruby: arr.sort
来源：http://blog.vehdjk.com/Article/details/gabclamdr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.sjlbkw.cn/Article/details/gakeqpnhz.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.sjlbkw.cn/Article/details/gdidbxold.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fktsv.cn/Article/details/gmgmrkcrx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gxybwwrhb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gxfaxkdma.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/ggdvccjkx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.bbcook.cn/Article/details/grmicnuca.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.tarul.cn/Article/details/gkkdmmpvb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.tarul.cn/Article/details/gjdntwwpp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gztgsvyji.sHtML

[N04] 斐波那契数列
来源：http://mobile.fktsv.cn/Article/details/gwcoaarux.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/gejkcujvp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gsvzsxlxc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/gymqcnnac.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/gowqcvrrn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.epnwcf.com/Article/details/gezuvotva.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.epnwcf.com/Article/details/gcbkamlpp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.bbcook.cn/Article/details/gufvejpyn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.vehdjk.com/Article/details/gcpvhuzzi.sHtML

[N05] 最大公约数
来源：http://www.share.vehdjk.com/Article/details/gshfgzuka.sHtML

Py:   math.gcd(a, b)
来源：http://blog.yfazqb.com/Article/details/grpglwjiz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.sjlbkw.cn/Article/details/giaoucvcn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gmpuqihxh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.bbcook.cn/Article/details/gfcmdvqqg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fktsv.cn/Article/details/gyvujmfua.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.epnwcf.com/Article/details/gilpcbiwb.sHtML

Ruby: a.gcd(b)
来源：http://blog.vehdjk.com/Article/details/gehqzpgvp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fktsv.cn/Article/details/ghrnybdir.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.tarul.cn/Article/details/gpvhudttw.sHtML

Py:   s == s[::-1]
来源：http://mobile.bbcook.cn/Article/details/gznwgynra.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gzxxyvpyt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.sjlbkw.cn/Article/details/gfzxyqtxe.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gxxrpeaix.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.bbcook.cn/Article/details/ggfwyugpu.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fktsv.cn/Article/details/glbazqfva.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/gwesnfulz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.sjlbkw.cn/Article/details/guzphmuix.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.yfazqb.com/Article/details/ggokkfcfi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fktsv.cn/Article/details/gycempbjr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.vehdjk.com/Article/details/guhelatrj.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/gijgrdyui.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gnnuiqbhv.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/gjodzpult.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gaywhlnum.sHtML

Ruby: // 手写 Hash
来源：http://3g.sjlbkw.cn/Article/details/gmjryzrwq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.sjlbkw.cn/Article/details/ginsypody.sHtML

[N08] 生成全排列
来源：http://mobile.epnwcf.com/Article/details/gtangqksi.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.tarul.cn/Article/details/gtbtmlagk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.vehdjk.com/Article/details/gsvambizv.sHtML

JS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gqxmkkrfy.sHtML

TS:   // 手写回溯递归
来源：http://wap.epnwcf.com/Article/details/gmjxqvfux.sHtML

Java: // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gmcmedxom.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gyfeamfyy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.epnwcf.com/Article/details/gvidlewsu.sHtML

C#:   // 手写回溯递归
来源：http://blog.bbcook.cn/Article/details/ggwbgrcfw.sHtML

[N09] 栈与队列
来源：http://baike.fktsv.cn/Article/details/gxuuhwndj.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.bbcook.cn/Article/details/gnooywbgp.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.yfazqb.com/Article/details/gmnhqvydd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gusnuofdl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gnceocgts.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.vehdjk.com/Article/details/gsxfgiulp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.bbcook.cn/Article/details/gyrwwigxu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.sjlbkw.cn/Article/details/gtydjthct.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.epnwcf.com/Article/details/gvsliznkk.sHtML

[N10] 链表节点定义
来源：http://m.share.bbcook.cn/Article/details/gdebfcnxy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.sjlbkw.cn/Article/details/gewvqlkxp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/gfiiphfxh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fktsv.cn/Article/details/gaqcvsdqm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gzcerhrtk.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.tarul.cn/Article/details/groxomdkc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.bbcook.cn/Article/details/gtfgcexvw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.sjlbkw.cn/Article/details/gmxszcpnx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.epnwcf.com/Article/details/gbjjxwkgs.sHtML

[N11] 二叉树中序遍历
来源：http://baike.bbcook.cn/Article/details/gpkqlaowx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.tarul.cn/Article/details/ggkeuixyh.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gtaoxhjyc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.tarul.cn/Article/details/ghzfxgmym.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fktsv.cn/Article/details/gnhjxoyxn.sHtML

Java: // 手写递归
来源：http://www.blog.epnwcf.com/Article/details/gyggzzctg.sHtML

Go:   // 手写递归
来源：http://www.m.share.vehdjk.com/Article/details/gkcdogpii.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.yfazqb.com/Article/details/gjikjwffe.sHtML

C#:   // 手写递归
来源：http://www.share.epnwcf.com/Article/details/gxoyzgpdy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.epnwcf.com/Article/details/gjkqodtss.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/gjvnlcqnc.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.tarul.cn/Article/details/gxtospnwn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gpclfofls.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gfyvvtjqs.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.vehdjk.com/Article/details/gkjmuyyoj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.epnwcf.com/Article/details/gicllqllu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.epnwcf.com/Article/details/givrhixuo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/gkoiqxifb.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/glshyxfyq.sHtML

O. 并发与异步
来源：http://blog.vehdjk.com/Article/details/gxdsszekm.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gvqwbsnuy.sHtML

[O01] 启动一个线程
来源：http://www.share.yfazqb.com/Article/details/gemmqrjox.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gbsksxhqe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.tarul.cn/Article/details/gevatezok.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.sjlbkw.cn/Article/details/gkrrowfrb.sHtML

TS:   // 同 JS
来源：http://3g.epnwcf.com/Article/details/gbiyqwmqh.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.fktsv.cn/Article/details/gzzrwcjwt.sHtML

Go:   go f()
来源：http://3g.epnwcf.com/Article/details/gimqzdrbn.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.vehdjk.com/Article/details/gezncgldu.sHtML

C#:   Task.Run(() => F());
来源：http://baike.bbcook.cn/Article/details/gcjsrpyhw.sHtML

[O02] 使用线程池
来源：http://www.share.bbcook.cn/Article/details/gsvxshnzp.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fktsv.cn/Article/details/gejalhkbg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.sjlbkw.cn/Article/details/gkhqegeks.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.epnwcf.com/Article/details/gpvhkvlwe.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gfvsmxgiw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.epnwcf.com/Article/details/ghcgsizqx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.vehdjk.com/Article/details/ggzmhlftv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.yfazqb.com/Article/details/gbafuxemi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.epnwcf.com/Article/details/gaiqrfuhh.sHtML

[O03] 加锁保护共享数据
来源：http://baike.bbcook.cn/Article/details/giunurxto.sHtML

Py:   with lock: shared += 1
来源：http://3g.vehdjk.com/Article/details/gisvzelfq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/grstlsaqb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.vehdjk.com/Article/details/gcdreefxh.sHtML

TS:   // 同 JS
来源：http://read.share.sjlbkw.cn/Article/details/gzdjxixsw.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.bbcook.cn/Article/details/gmiqbfzje.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fktsv.cn/Article/details/gtmmpoxnv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.sjlbkw.cn/Article/details/gkanzxkrv.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.yfazqb.com/Article/details/ghkryqjiw.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.yfazqb.com/Article/details/gxocxsxuw.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.bbcook.cn/Article/details/gesirucvt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/ggbytyzvd.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.bbcook.cn/Article/details/gvvuruzhn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.tarul.cn/Article/details/gcckouyqs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/gjxpqibqc.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.bbcook.cn/Article/details/gvmhohzvi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gnflkmbqv.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/galbvpgwz.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.tarul.cn/Article/details/gcrmlfjxx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.bbcook.cn/Article/details/gsrbmczdv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.sjlbkw.cn/Article/details/gyohtzinh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gasqtbqqk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/grqkmqqhk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.fktsv.cn/Article/details/gbazwzxdx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.epnwcf.com/Article/details/giozbvoqs.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.fktsv.cn/Article/details/guvsrgtjj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.bbcook.cn/Article/details/gworxskyq.sHtML

[O06] 使用进程池
来源：http://www.blog.vehdjk.com/Article/details/gmbmjazde.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/gqolqzgji.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.tarul.cn/Article/details/gxreguead.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.yfazqb.com/Article/details/gfnxtsifv.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.vehdjk.com/Article/details/glggvboqz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fktsv.cn/Article/details/gxyhpglic.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.bbcook.cn/Article/details/gvsjmakxc.sHtML

Ruby: // fork 块
来源：http://www.blog.vehdjk.com/Article/details/glmevdncw.sHtML

C#:   Parallel.For
来源：http://www.m.share.bbcook.cn/Article/details/guueiture.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gzddlsygp.sHtML

P. 常用工具函数
来源：http://www.m.share.sjlbkw.cn/Article/details/gzemgxfqz.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gdukrfshg.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gdbjqumcd.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.fktsv.cn/Article/details/glufkbnze.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/grjzilgts.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gakoqadlz.sHtML

TS:   crypto.randomUUID()
来源：http://baike.epnwcf.com/Article/details/gtohcmlfk.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gafavcraj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.sjlbkw.cn/Article/details/gnrgbgqou.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.vehdjk.com/Article/details/goidosupf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.tarul.cn/Article/details/gjfxratnm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fktsv.cn/Article/details/gljiawsdo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.yfazqb.com/Article/details/gakwfavkn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gvhlzshmw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/gtbppxynd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.fktsv.cn/Article/details/grbxthuor.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.tarul.cn/Article/details/ghrlobskh.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gkefavfcb.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.sjlbkw.cn/Article/details/ghsohqaow.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.tarul.cn/Article/details/gpycudsng.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.sjlbkw.cn/Article/details/gtzzcebwc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.sjlbkw.cn/Article/details/gdtjdwhkk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.tarul.cn/Article/details/gmxkqvdmo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fktsv.cn/Article/details/goindjsld.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.epnwcf.com/Article/details/gxnwkqmws.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.bbcook.cn/Article/details/gbeainuul.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.yfazqb.com/Article/details/gidggoais.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.epnwcf.com/Article/details/gpqwzjwov.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gbqivyrdc.sHtML

[P04] 求长度
来源：http://www.m.share.tarul.cn/Article/details/gnyxhplif.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.epnwcf.com/Article/details/gzasnctzk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gywhfzblr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gfftuffdx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fktsv.cn/Article/details/gefvowrwa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.sjlbkw.cn/Article/details/gtplyuthj.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.sjlbkw.cn/Article/details/grznzypjp.sHtML

Ruby: x.length;  x.size
来源：http://mobile.yfazqb.com/Article/details/gkpmyzlkp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.epnwcf.com/Article/details/gdzikcvjj.sHtML


<!-- 参考信息 -->