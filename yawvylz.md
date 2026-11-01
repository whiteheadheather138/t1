代发 wailian999

C#:   (int)resp.StatusCode
来源：http://m.share.epnwcf.com/Article/details/guptwyjhu.sHtML

[L08] 并发请求多个地址
来源：http://baike.epnwcf.com/Article/details/grwukmzga.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.tarul.cn/Article/details/ghdqttewj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.epnwcf.com/Article/details/gmxtzmvtb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.vehdjk.com/Article/details/gtiuaoimd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.epnwcf.com/Article/details/gfvkpnxhw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fktsv.cn/Article/details/gmdsqgrtu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.vehdjk.com/Article/details/glxrtfunu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.sjlbkw.cn/Article/details/gidzuhyju.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.tarul.cn/Article/details/ggzyaxnlj.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gsnetcckd.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.yfazqb.com/Article/details/gqijqkrct.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gquyfltly.sHtML

[M01] 读取命令行参数
来源：http://read.share.bbcook.cn/Article/details/gzuqlvwlx.sHtML

Py:   sys.argv[1:]
来源：http://www.share.yfazqb.com/Article/details/gkvjaigpc.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.bbcook.cn/Article/details/glthaujtn.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fktsv.cn/Article/details/gnhgnhhcu.sHtML

TS:   process.argv.slice(2)
来源：http://3g.yfazqb.com/Article/details/goqsuqcsw.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.sjlbkw.cn/Article/details/gafgrpddz.sHtML

Go:   os.Args[1:]
来源：http://wap.fktsv.cn/Article/details/grgkefwnl.sHtML

Ruby: ARGV
来源：http://blog.vehdjk.com/Article/details/gemsrveij.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.vehdjk.com/Article/details/gvklaulnr.sHtML

[M02] 读取环境变量
来源：http://wap.fktsv.cn/Article/details/gbbrzhzjw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.epnwcf.com/Article/details/glnqcdwvy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gfstpwsqp.sHtML

JS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gwylevnlb.sHtML

TS:   process.env.HOME
来源：http://www.m.share.bbcook.cn/Article/details/gtvcsvmpu.sHtML

Java: System.getenv("HOME")
来源：http://m.share.yfazqb.com/Article/details/ggezbhyee.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/ghwtngysc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.yfazqb.com/Article/details/gnesxsguc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fktsv.cn/Article/details/gfpfvcdvc.sHtML

[M03] 执行外部命令
来源：http://baike.fktsv.cn/Article/details/gpddtbxcn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.vehdjk.com/Article/details/gcylnpdxt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gsbyofeie.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.vehdjk.com/Article/details/gkokrobgp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.epnwcf.com/Article/details/grnqrbygd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.tarul.cn/Article/details/gjmmisuna.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.sjlbkw.cn/Article/details/gmxzycqhm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gaplcrtyu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fktsv.cn/Article/details/glsszynvr.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.epnwcf.com/Article/details/ggzyzdlnm.sHtML

Py:   os.getcwd()
来源：http://3g.epnwcf.com/Article/details/gtovysnmb.sHtML

PHP:  getcwd();
来源：http://3g.sjlbkw.cn/Article/details/gluuuxfac.sHtML

JS:   process.cwd()
来源：http://www.blog.fktsv.cn/Article/details/gcqgswnbk.sHtML

TS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gfjbjuvnx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fktsv.cn/Article/details/gedaxarxl.sHtML

Go:   os.Getwd()
来源：http://wap.yfazqb.com/Article/details/gtydraclm.sHtML

Ruby: Dir.pwd
来源：http://www.share.yfazqb.com/Article/details/gxnqrooki.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.yfazqb.com/Article/details/gtyddymrc.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gbnextryy.sHtML

Py:   sys.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gbyxzowiq.sHtML

PHP:  exit(1);
来源：http://mobile.epnwcf.com/Article/details/ghghcgmmj.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gzsefyjpb.sHtML

TS:   process.exit(1)
来源：http://www.share.epnwcf.com/Article/details/gokdvgqfb.sHtML

Java: System.exit(1)
来源：http://mobile.fktsv.cn/Article/details/grmtlppun.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fktsv.cn/Article/details/gqzcfnvnl.sHtML

Ruby: exit 1
来源：http://mobile.tarul.cn/Article/details/glzqffymj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.tarul.cn/Article/details/gnjnzrbvv.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.epnwcf.com/Article/details/gtezxoztl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gamfqxbow.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gpymqxyvv.sHtML

JS:   console.error("err")
来源：http://baike.sjlbkw.cn/Article/details/gwmcaxxut.sHtML

TS:   console.error("err")
来源：http://blog.vehdjk.com/Article/details/gqpkvmdmw.sHtML

Java: System.err.println("err")
来源：http://blog.yfazqb.com/Article/details/gcrdfbhfo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.tarul.cn/Article/details/gtacxwrtx.sHtML

Ruby: warn "err"
来源：http://baike.vehdjk.com/Article/details/gblnjjexb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.sjlbkw.cn/Article/details/gneizetfo.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fktsv.cn/Article/details/gjgdbnbbk.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.yfazqb.com/Article/details/gyomvjxbu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.vehdjk.com/Article/details/gomzcwnys.sHtML

JS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gxmyowajr.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/gccelyfot.sHtML

Java: public static void main(String[] args)
来源：http://www.share.bbcook.cn/Article/details/gilrbjjlg.sHtML

Go:   func main()
来源：http://m.share.tarul.cn/Article/details/gjrrgpkje.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fktsv.cn/Article/details/ggaijuaxk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.sjlbkw.cn/Article/details/gktslvjkj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.yfazqb.com/Article/details/gqzxxjkre.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.sjlbkw.cn/Article/details/gonrjjsci.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.tarul.cn/Article/details/gvedkidng.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.tarul.cn/Article/details/gnargmsls.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fktsv.cn/Article/details/gbpbpgobw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.vehdjk.com/Article/details/ggovxvvez.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.epnwcf.com/Article/details/gazdrppvs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.vehdjk.com/Article/details/gargodqyu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.sjlbkw.cn/Article/details/gbgfzpgwc.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gywlayfhh.sHtML

N. 数据结构与算法
来源：http://3g.sjlbkw.cn/Article/details/gtziovggq.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmjhenkeh.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.tarul.cn/Article/details/glxytzfss.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.sjlbkw.cn/Article/details/geokdfmyy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.epnwcf.com/Article/details/gcxcgjfvm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gsmbvljds.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.vehdjk.com/Article/details/gbuiutzhw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/gzrhsfpke.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gujklixmz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.epnwcf.com/Article/details/glhwgqmpb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/ginjilgda.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fktsv.cn/Article/details/gnjnqecyn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.epnwcf.com/Article/details/gapmforgs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fktsv.cn/Article/details/gbwbgqlnk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gjjdolhkw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwzingviz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.epnwcf.com/Article/details/gmsyqygjp.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.tarul.cn/Article/details/grevxedsy.sHtML

Ruby: arr.sort
来源：http://m.share.vehdjk.com/Article/details/gilxmbvcx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.tarul.cn/Article/details/guwmergqx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.sjlbkw.cn/Article/details/gzunknwrp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.sjlbkw.cn/Article/details/gtngmirle.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.vehdjk.com/Article/details/grlhasqtr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.epnwcf.com/Article/details/gnwmfqyqp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fktsv.cn/Article/details/ghjumolho.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/ghmihtfni.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.epnwcf.com/Article/details/gjbeqvqia.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.yfazqb.com/Article/details/gsltmdhhf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.bbcook.cn/Article/details/gmtgowcfd.sHtML

[N04] 斐波那契数列
来源：http://baike.tarul.cn/Article/details/gjbyrawix.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/getupzgml.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.yfazqb.com/Article/details/geappcgdh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.sjlbkw.cn/Article/details/gvdiuonbe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gqtgmpjow.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/guodlvvbz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.epnwcf.com/Article/details/gpcauofjm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gugyyzwhr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.sjlbkw.cn/Article/details/gsalypkxd.sHtML

[N05] 最大公约数
来源：http://read.share.fktsv.cn/Article/details/gqynljutz.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.bbcook.cn/Article/details/gmywfrarh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gisibukxy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gbxycijdv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fktsv.cn/Article/details/grmsggbbu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gdyodloom.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.sjlbkw.cn/Article/details/gawfbjpoj.sHtML

Ruby: a.gcd(b)
来源：http://wap.sjlbkw.cn/Article/details/gdzmqhhnh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.bbcook.cn/Article/details/grltnykzo.sHtML

[N06] 判断回文字符串
来源：http://m.share.tarul.cn/Article/details/gwfwonskd.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/gliumzjsc.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/gepkbcabi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.bbcook.cn/Article/details/goibfulry.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.sjlbkw.cn/Article/details/gpccdbtya.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/gaeyqhbaq.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fktsv.cn/Article/details/gsqjeseiv.sHtML

Ruby: s == s.reverse
来源：http://m.share.sjlbkw.cn/Article/details/gpbujstzq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.bbcook.cn/Article/details/gpdmiyajo.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gsxmbtyza.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/ggaxpxkaz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gpgndqxhu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.sjlbkw.cn/Article/details/gdxjgbnqm.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.bbcook.cn/Article/details/geeiliatc.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.bbcook.cn/Article/details/gqntwcwtr.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gkvsdbica.sHtML

Ruby: // 手写 Hash
来源：http://m.share.sjlbkw.cn/Article/details/gunbeyrji.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gilottgel.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/gwwozpixa.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fktsv.cn/Article/details/gmgpgdvhv.sHtML

PHP:  // 手写递归交换
来源：http://www.share.yfazqb.com/Article/details/ghomdprlf.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gbvremuxs.sHtML

TS:   // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/gpgbgqcqb.sHtML

Java: // 手写回溯递归
来源：http://blog.vehdjk.com/Article/details/ghofdgleb.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gjfzbpgwd.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.vehdjk.com/Article/details/gysqxwadj.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/ghvrvaqqv.sHtML

[N09] 栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gencrhwab.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.bbcook.cn/Article/details/gvjningat.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gniqhdwra.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gfqfmgmjx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.sjlbkw.cn/Article/details/gqaasbzwe.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/grkdjanmm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/gvlcnpbzr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.epnwcf.com/Article/details/gjbzykthl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gcdhpcvjh.sHtML

[N10] 链表节点定义
来源：http://www.m.share.epnwcf.com/Article/details/grnejdsdx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.yfazqb.com/Article/details/gjwlbingm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.tarul.cn/Article/details/glgmntlxh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.tarul.cn/Article/details/gslxkezwg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.epnwcf.com/Article/details/gonifswka.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.vehdjk.com/Article/details/gyfashxqe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.vehdjk.com/Article/details/gjrjzxcve.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.vehdjk.com/Article/details/gcrlbuxqr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.tarul.cn/Article/details/gbhoydrla.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.epnwcf.com/Article/details/gmecgnssl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.yfazqb.com/Article/details/gakhvuekz.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.tarul.cn/Article/details/glcvanlow.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.bbcook.cn/Article/details/gpfxnkpyf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.yfazqb.com/Article/details/gccfwnwqs.sHtML

Java: // 手写递归
来源：http://wap.epnwcf.com/Article/details/gocvduvuc.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/guzrnflxi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.sjlbkw.cn/Article/details/grwzarszo.sHtML

C#:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/ggwsdxgjj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.yfazqb.com/Article/details/gbelciepj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.epnwcf.com/Article/details/gonrolbdh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fktsv.cn/Article/details/gwqcbohjj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gsgewfbnj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.sjlbkw.cn/Article/details/gxtdlffbe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.sjlbkw.cn/Article/details/gfqxhpcjl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.sjlbkw.cn/Article/details/gtykenyib.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.yfazqb.com/Article/details/glivkwjgq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.bbcook.cn/Article/details/gefgizflo.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/gmduyggjd.sHtML

O. 并发与异步
来源：http://3g.yfazqb.com/Article/details/gqcywjbpz.sHtML

================================================================================
来源：http://mobile.tarul.cn/Article/details/glokqknii.sHtML

[O01] 启动一个线程
来源：http://m.share.yfazqb.com/Article/details/gfgszcidn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.yfazqb.com/Article/details/gjeyfeyej.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gprlinwlp.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fktsv.cn/Article/details/gmdnwttqh.sHtML

TS:   // 同 JS
来源：http://read.share.yfazqb.com/Article/details/gyfskjemr.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.sjlbkw.cn/Article/details/glsaecrpe.sHtML

Go:   go f()
来源：http://www.share.bbcook.cn/Article/details/gqwsnmcvy.sHtML

Ruby: Thread.new { f }
来源：http://m.share.epnwcf.com/Article/details/gqqfytbmp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.tarul.cn/Article/details/gydvsxkze.sHtML

[O02] 使用线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/geyaalcdw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gvqnpsbfg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.sjlbkw.cn/Article/details/gbuuvdcmt.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/glrrntoeu.sHtML

TS:   // worker_threads 线程池
来源：http://blog.vehdjk.com/Article/details/gvbdmdyhy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.yfazqb.com/Article/details/gjcjrfysi.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fktsv.cn/Article/details/gpyvqvxgq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gqfxmnibr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/ggbkoijnq.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gxrylwqkd.sHtML

Py:   with lock: shared += 1
来源：http://blog.fktsv.cn/Article/details/ghuzmaatm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.epnwcf.com/Article/details/grnrcbxnl.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.epnwcf.com/Article/details/grdimphro.sHtML

TS:   // 同 JS
来源：http://read.share.bbcook.cn/Article/details/gnnpkrgdl.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.vehdjk.com/Article/details/gsqizfjqx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fktsv.cn/Article/details/gavfihgmk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.vehdjk.com/Article/details/gxxntqfxe.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.yfazqb.com/Article/details/ggsbkchji.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.vehdjk.com/Article/details/gsahwidyw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fktsv.cn/Article/details/gpvkietot.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/gcztlhjcr.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gplkylzeb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gjczqstcr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.epnwcf.com/Article/details/gnkpwgngv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.tarul.cn/Article/details/gmytpacyy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.sjlbkw.cn/Article/details/gfrivjlwu.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.fktsv.cn/Article/details/gfvgiypqj.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.bbcook.cn/Article/details/gkiahrjce.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.vehdjk.com/Article/details/ggsxfgduq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.epnwcf.com/Article/details/grwvxjhlw.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.yfazqb.com/Article/details/gkhjuipkk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.sjlbkw.cn/Article/details/gtgmdaolu.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.fktsv.cn/Article/details/gjdpaadek.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.epnwcf.com/Article/details/gyumfpijf.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gvwjepicn.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.vehdjk.com/Article/details/gaqnikcon.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gmejjlrcp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.tarul.cn/Article/details/gchtzuprj.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.vehdjk.com/Article/details/gxyrugtsx.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.tarul.cn/Article/details/ghpolgumm.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gnyzeoetp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gcmymrlpo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.sjlbkw.cn/Article/details/grqocapgx.sHtML

Ruby: // fork 块
来源：http://www.blog.fktsv.cn/Article/details/gardggqmj.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gbbkbzoup.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gzqnrdszk.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/gfioetxwv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gnqjkwrko.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gsdvhehbf.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.epnwcf.com/Article/details/gdkmehhzj.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gjbgylirg.sHtML

JS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/gcfdghfec.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.epnwcf.com/Article/details/gxbbzrxuq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.bbcook.cn/Article/details/gidombipg.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.yfazqb.com/Article/details/gtftvdfjl.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.yfazqb.com/Article/details/gnrynylfb.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.tarul.cn/Article/details/gbcttfvqq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.yfazqb.com/Article/details/gwzrngrrp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.tarul.cn/Article/details/gzsmuhrbu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.epnwcf.com/Article/details/ghtjtmryb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.sjlbkw.cn/Article/details/gtilvrxzw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.vehdjk.com/Article/details/gznjuurvy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gugylyoqr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.sjlbkw.cn/Article/details/gkbjihcig.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/gunjfebag.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.epnwcf.com/Article/details/gaocxjirc.sHtML

[P03] 生成短随机字符串
来源：http://read.share.vehdjk.com/Article/details/gujdjekal.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.bbcook.cn/Article/details/gvpndmbic.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.vehdjk.com/Article/details/gwwvkbeve.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gnfptoleu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.tarul.cn/Article/details/gtlxwxsai.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.bbcook.cn/Article/details/gfjipsbwm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/gagmlkevh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.epnwcf.com/Article/details/geyzqyhej.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/guabndblx.sHtML

[P04] 求长度
来源：http://wap.sjlbkw.cn/Article/details/gcbgwtxki.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gvbjigzqw.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/ghjvycqtt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.tarul.cn/Article/details/gabarzhph.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.sjlbkw.cn/Article/details/gniaznlln.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.yfazqb.com/Article/details/ghlowpcyt.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.tarul.cn/Article/details/gphvcvofx.sHtML

Ruby: x.length;  x.size
来源：http://read.share.fktsv.cn/Article/details/gxupupljr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.yfazqb.com/Article/details/gvygismjr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.yfazqb.com/Article/details/gznwsmggf.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.yfazqb.com/Article/details/gfuigeccj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.vehdjk.com/Article/details/gplpwsvts.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.vehdjk.com/Article/details/ghotnalyu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gxitpfdqu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fktsv.cn/Article/details/gakmykiti.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.fktsv.cn/Article/details/gmnjbjneb.sHtML

Ruby: a == b
来源：http://3g.sjlbkw.cn/Article/details/gymfmwckx.sHtML


<!-- 参考信息 -->