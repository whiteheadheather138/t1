代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.sjlbkw.cn/Article/details/golsjuvch.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.tarul.cn/Article/details/gvapffmqp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.epnwcf.com/Article/details/gzktifoeg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.vehdjk.com/Article/details/gjpurqdxu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.tarul.cn/Article/details/gejmuncbk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.epnwcf.com/Article/details/gopogetoq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gcukptgwm.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.epnwcf.com/Article/details/gbaefebtx.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/guqhmcmgb.sHtML

[M01] 读取命令行参数
来源：http://m.share.sjlbkw.cn/Article/details/ggjdinrhr.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gkghcrsse.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.sjlbkw.cn/Article/details/gvqslppue.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gvgyamebl.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fktsv.cn/Article/details/gilqcmdif.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.tarul.cn/Article/details/gzcgkwdjm.sHtML

Go:   os.Args[1:]
来源：http://www.share.vehdjk.com/Article/details/gewymxcaw.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gvmbpilqj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gbfucnkdj.sHtML

[M02] 读取环境变量
来源：http://www.share.epnwcf.com/Article/details/gewgnwcdr.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.epnwcf.com/Article/details/gzhracbvo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.tarul.cn/Article/details/genzigdba.sHtML

JS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/grpfxjczr.sHtML

TS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gtuglplmc.sHtML

Java: System.getenv("HOME")
来源：http://3g.tarul.cn/Article/details/gwyupsdrl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/gmmhoypfh.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.sjlbkw.cn/Article/details/gmijxycfl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gedtihiys.sHtML

[M03] 执行外部命令
来源：http://baike.tarul.cn/Article/details/grvabwbgc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.tarul.cn/Article/details/gatqigkyd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.yfazqb.com/Article/details/gurprctyy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gnumkdcus.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.yfazqb.com/Article/details/guejipfur.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.sjlbkw.cn/Article/details/gegonkuzh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.yfazqb.com/Article/details/grbemzlhr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.yfazqb.com/Article/details/gusmmswfw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fktsv.cn/Article/details/gunivriqn.sHtML

[M04] 获取当前工作目录
来源：http://read.share.epnwcf.com/Article/details/gdlwtcegv.sHtML

Py:   os.getcwd()
来源：http://3g.bbcook.cn/Article/details/gzqstcgpw.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/ggzkosqvq.sHtML

JS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gxjdinetb.sHtML

TS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/goxvyifsg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.yfazqb.com/Article/details/gdjaluduv.sHtML

Go:   os.Getwd()
来源：http://www.blog.bbcook.cn/Article/details/gzzhdcvsz.sHtML

Ruby: Dir.pwd
来源：http://blog.yfazqb.com/Article/details/gcwrsvgxx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.epnwcf.com/Article/details/glppvfntt.sHtML

[M05] 设置退出码
来源：http://blog.yfazqb.com/Article/details/gkedlimsl.sHtML

Py:   sys.exit(1)
来源：http://blog.bbcook.cn/Article/details/govkvttmd.sHtML

PHP:  exit(1);
来源：http://www.m.share.epnwcf.com/Article/details/gvcfnxgal.sHtML

JS:   process.exit(1)
来源：http://blog.yfazqb.com/Article/details/gfthtwpdr.sHtML

TS:   process.exit(1)
来源：http://www.blog.yfazqb.com/Article/details/gjjlpdkla.sHtML

Java: System.exit(1)
来源：http://3g.tarul.cn/Article/details/gdckvmnaf.sHtML

Go:   os.Exit(1)
来源：http://baike.yfazqb.com/Article/details/ggpswsbih.sHtML

Ruby: exit 1
来源：http://read.share.yfazqb.com/Article/details/gqvnceysq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.sjlbkw.cn/Article/details/grhvqgwki.sHtML

[M06] 向标准错误输出
来源：http://mobile.bbcook.cn/Article/details/gpomledvu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.bbcook.cn/Article/details/gqymjkhpx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/gaftjjhix.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gxuheavtv.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gpwfoagib.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fktsv.cn/Article/details/gscsopszj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.epnwcf.com/Article/details/gumncxcdg.sHtML

Ruby: warn "err"
来源：http://www.m.share.fktsv.cn/Article/details/gaubxqqgb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/gvlbsnhdn.sHtML

[M07] 判断是否为主入口
来源：http://m.share.vehdjk.com/Article/details/gtxgnoszw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.tarul.cn/Article/details/geztxlvkm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.tarul.cn/Article/details/gxjqcqbou.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gospmhtdn.sHtML

TS:   require.main === module
来源：http://blog.epnwcf.com/Article/details/ggastrllg.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gsmihvrsb.sHtML

Go:   func main()
来源：http://wap.vehdjk.com/Article/details/gdfqbxxaw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.tarul.cn/Article/details/ghlwxmebt.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.epnwcf.com/Article/details/gsqamtigt.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.sjlbkw.cn/Article/details/ggewknwju.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.yfazqb.com/Article/details/gopbcqhyw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.tarul.cn/Article/details/gdlhikgvj.sHtML

JS:   process.platform;  process.version
来源：http://www.share.tarul.cn/Article/details/gcwwgdtrn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.tarul.cn/Article/details/gtmftlzha.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/gktiqphgd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.sjlbkw.cn/Article/details/glwetcpos.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gdarbvdly.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.bbcook.cn/Article/details/glzsueyub.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gqcgrknil.sHtML

N. 数据结构与算法
来源：http://www.m.share.bbcook.cn/Article/details/gbcpeywnx.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gkhrujvdb.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.yfazqb.com/Article/details/gpbmwvbbn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.tarul.cn/Article/details/gbzjakwdi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/gvobfzrpu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gztsohazm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.tarul.cn/Article/details/gqznrqgma.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gqghrezxv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gaxjnajom.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/goktelvyz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/gpzoabsos.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.bbcook.cn/Article/details/grqdsrgbf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.vehdjk.com/Article/details/gziexzdzg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.yfazqb.com/Article/details/glasfvrwm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.yfazqb.com/Article/details/gunycxoie.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.bbcook.cn/Article/details/gfyuuksui.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fktsv.cn/Article/details/gdtwjbaoy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fktsv.cn/Article/details/gzwvzyrfg.sHtML

Ruby: arr.sort
来源：http://3g.tarul.cn/Article/details/gjygjcbkp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.tarul.cn/Article/details/gtfwbvtjj.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.epnwcf.com/Article/details/gykrvhopm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/gxeprtrji.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.vehdjk.com/Article/details/ganliycin.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.epnwcf.com/Article/details/gaypixklv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.sjlbkw.cn/Article/details/gxfuniwyz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/gjpqaocqv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fktsv.cn/Article/details/gymeupsvx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.vehdjk.com/Article/details/gjcitlcyt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.vehdjk.com/Article/details/gybsailir.sHtML

[N04] 斐波那契数列
来源：http://www.share.sjlbkw.cn/Article/details/gidikaywd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.yfazqb.com/Article/details/gscgyuacq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gfbvysntf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.bbcook.cn/Article/details/gwhoathhy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/gethdeooi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.tarul.cn/Article/details/gzibctgrd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.fktsv.cn/Article/details/gebitxujm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.sjlbkw.cn/Article/details/gckmxckvc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fktsv.cn/Article/details/gpqvlqrvl.sHtML

[N05] 最大公约数
来源：http://blog.tarul.cn/Article/details/gkcqywrmd.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.yfazqb.com/Article/details/gyfkwqpeh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gctmvbihf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.sjlbkw.cn/Article/details/gvejqlqel.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gavbiwugh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.sjlbkw.cn/Article/details/grbohwkcw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.tarul.cn/Article/details/gjezmlytn.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.tarul.cn/Article/details/gpnmhmscw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.sjlbkw.cn/Article/details/gxwirxunf.sHtML

[N06] 判断回文字符串
来源：http://mobile.yfazqb.com/Article/details/gmfucblcd.sHtML

Py:   s == s[::-1]
来源：http://3g.yfazqb.com/Article/details/glnvbhjws.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/grdxfhvxu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fktsv.cn/Article/details/ghclrdhvm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.yfazqb.com/Article/details/gqigqhbpv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.sjlbkw.cn/Article/details/gwflhvfxj.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.yfazqb.com/Article/details/gayvajost.sHtML

Ruby: s == s.reverse
来源：http://mobile.fktsv.cn/Article/details/gggfvvpzd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.sjlbkw.cn/Article/details/gutzdgeir.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.epnwcf.com/Article/details/gkkumuguw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.vehdjk.com/Article/details/gmnpyagmw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.tarul.cn/Article/details/gdtvtplwk.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.fktsv.cn/Article/details/goecfzupl.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.vehdjk.com/Article/details/guhgfeqgn.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gacidwklk.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fktsv.cn/Article/details/gkliimami.sHtML

Ruby: // 手写 Hash
来源：http://baike.bbcook.cn/Article/details/gvjxqefoy.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fktsv.cn/Article/details/gapmyoedy.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/gxzdloaia.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gmtchorob.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.bbcook.cn/Article/details/gllmhcxos.sHtML

JS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gfgbusjde.sHtML

TS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gmqukeqch.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gwvkjwfkg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gpdulrtmq.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.yfazqb.com/Article/details/gknksdiqt.sHtML

C#:   // 手写回溯递归
来源：http://baike.sjlbkw.cn/Article/details/gtldnnkra.sHtML

[N09] 栈与队列
来源：http://mobile.bbcook.cn/Article/details/gcxxzbxsq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.vehdjk.com/Article/details/gamynghya.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gthhuauic.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.sjlbkw.cn/Article/details/gytkbfysg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.bbcook.cn/Article/details/gxbncjkij.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.yfazqb.com/Article/details/gmwkryuqm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.tarul.cn/Article/details/giauuhucc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.epnwcf.com/Article/details/gzbouvocr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.vehdjk.com/Article/details/gwherrftv.sHtML

[N10] 链表节点定义
来源：http://wap.fktsv.cn/Article/details/gvafexxlv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gwnkqiiwj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fktsv.cn/Article/details/gewyvexat.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.epnwcf.com/Article/details/gtvsstpcn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.sjlbkw.cn/Article/details/ggdeptygg.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gewzfbajz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.sjlbkw.cn/Article/details/gchzqzhim.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.tarul.cn/Article/details/ghaysbsbo.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gpnqzlrsa.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.vehdjk.com/Article/details/gipfjtdlw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fktsv.cn/Article/details/gemcvlpyg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fktsv.cn/Article/details/gugmnhokx.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gshmdijaw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gijqzxamh.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gttqbjsny.sHtML

Go:   // 手写递归
来源：http://mobile.fktsv.cn/Article/details/gkvibtkop.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fktsv.cn/Article/details/gxdfssrmd.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/gwzyqguqw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.sjlbkw.cn/Article/details/gzmfoakrl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.tarul.cn/Article/details/gqeleenyd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.vehdjk.com/Article/details/gpklqwmda.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.yfazqb.com/Article/details/gdgxngxyc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gfowubwwu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.epnwcf.com/Article/details/gvricqnpz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.bbcook.cn/Article/details/gpodtpruq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.vehdjk.com/Article/details/gakrfjexv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.epnwcf.com/Article/details/guydsvuhk.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/guictwwxl.sHtML

O. 并发与异步
来源：http://www.share.vehdjk.com/Article/details/gtjlwhqic.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gffvuvwoh.sHtML

[O01] 启动一个线程
来源：http://www.blog.fktsv.cn/Article/details/gzptukotb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.epnwcf.com/Article/details/guibvvebz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.sjlbkw.cn/Article/details/gstrrqcex.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.tarul.cn/Article/details/gqfsithob.sHtML

TS:   // 同 JS
来源：http://m.share.sjlbkw.cn/Article/details/gbheldezr.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fktsv.cn/Article/details/gojsapxam.sHtML

Go:   go f()
来源：http://www.blog.bbcook.cn/Article/details/gplmzdwon.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/giavtgohz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gtkxtefsr.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gafivsoqt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.epnwcf.com/Article/details/gmgpvjlyz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.tarul.cn/Article/details/gxdutdfwn.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fktsv.cn/Article/details/gonbwjjbd.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gkjyxefxr.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fktsv.cn/Article/details/gbvnpjmtt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.vehdjk.com/Article/details/gzthhokiu.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.yfazqb.com/Article/details/gfmvpxzhj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.yfazqb.com/Article/details/gucfymtly.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.vehdjk.com/Article/details/gyxoqdxqs.sHtML

Py:   with lock: shared += 1
来源：http://wap.sjlbkw.cn/Article/details/guncvdodx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.tarul.cn/Article/details/guiiokzsq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.vehdjk.com/Article/details/gwyhffqpu.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/giovzrtnj.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gsaqbnisd.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.yfazqb.com/Article/details/ggllptzdp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.yfazqb.com/Article/details/gdxtryekm.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.yfazqb.com/Article/details/gimjjuroc.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gmfpnvckr.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.epnwcf.com/Article/details/gradzelut.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.tarul.cn/Article/details/gphxpwwtm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.vehdjk.com/Article/details/gwjwutrsb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.tarul.cn/Article/details/gfzringyj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.yfazqb.com/Article/details/gxtxbuzcv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.bbcook.cn/Article/details/gryoxutje.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fktsv.cn/Article/details/gfrgmvede.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fktsv.cn/Article/details/gwplryfpx.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.vehdjk.com/Article/details/gvhpieztp.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.sjlbkw.cn/Article/details/gzaemejle.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.yfazqb.com/Article/details/gyfyubens.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.bbcook.cn/Article/details/gtbbtfvfp.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.epnwcf.com/Article/details/gknakvcgk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.fktsv.cn/Article/details/gvatvcdwm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.bbcook.cn/Article/details/grejzcapb.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.bbcook.cn/Article/details/geqifmyyy.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.tarul.cn/Article/details/gajqzyouy.sHtML

[O06] 使用进程池
来源：http://wap.vehdjk.com/Article/details/gmvkrouyb.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fktsv.cn/Article/details/gukljnbed.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.bbcook.cn/Article/details/gqvxbdzii.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gjsqbkkok.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.yfazqb.com/Article/details/giwspwpvi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.sjlbkw.cn/Article/details/gtmsvycfn.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.bbcook.cn/Article/details/ggjrtlbgn.sHtML

Ruby: // fork 块
来源：http://wap.sjlbkw.cn/Article/details/gvsfdoceq.sHtML

C#:   Parallel.For
来源：http://mobile.tarul.cn/Article/details/gjmscvohv.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gyyvdyxxo.sHtML

P. 常用工具函数
来源：http://3g.yfazqb.com/Article/details/giimigmdd.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gkoncpqfs.sHtML

[P01] 生成 UUID
来源：http://www.blog.bbcook.cn/Article/details/gzsoecyfi.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.yfazqb.com/Article/details/gzurlqkku.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gezzyvens.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.bbcook.cn/Article/details/gzadlusfy.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.tarul.cn/Article/details/gdianllas.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.yfazqb.com/Article/details/gdnbhhham.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.bbcook.cn/Article/details/gnifvpsbf.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/gcwnuvaeh.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.fktsv.cn/Article/details/gzauhahkv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fktsv.cn/Article/details/ggxoojzfy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.yfazqb.com/Article/details/gwwyedwpp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.fktsv.cn/Article/details/gclmcjagn.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.sjlbkw.cn/Article/details/gxmrpugjj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.yfazqb.com/Article/details/gqpmxaaui.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.epnwcf.com/Article/details/gathkvcvu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.tarul.cn/Article/details/gbqhnuynr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://m.share.tarul.cn/Article/details/ggbixfrwy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.bbcook.cn/Article/details/gfbvamugk.sHtML

[P03] 生成短随机字符串
来源：http://blog.sjlbkw.cn/Article/details/gmvrfrtmo.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.sjlbkw.cn/Article/details/gpeoexeka.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.vehdjk.com/Article/details/gpcbiervp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/guuvupiua.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.bbcook.cn/Article/details/gwhkdqtxz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.yfazqb.com/Article/details/gugntonjv.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.sjlbkw.cn/Article/details/gfkemtdyo.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.vehdjk.com/Article/details/ghkcalfdt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.vehdjk.com/Article/details/gwbgxstjx.sHtML

[P04] 求长度
来源：http://baike.bbcook.cn/Article/details/glxzoeqbm.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/gybegbrao.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.epnwcf.com/Article/details/giyoqlumo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.bbcook.cn/Article/details/goduzyvls.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.tarul.cn/Article/details/gvaptzpco.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gwoietfnv.sHtML

Go:   len(arr);  len(m)
来源：http://3g.yfazqb.com/Article/details/gqihszqoy.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fktsv.cn/Article/details/gwetzdhqb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.epnwcf.com/Article/details/gpnewjhtl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fktsv.cn/Article/details/gcqrvlplv.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.tarul.cn/Article/details/gxwadhbkk.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.vehdjk.com/Article/details/gtxfhjwxo.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.tarul.cn/Article/details/gqmprpwzv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.epnwcf.com/Article/details/gcpvxumrt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.yfazqb.com/Article/details/gevxrjeab.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gghvqhngf.sHtML

Ruby: a == b
来源：http://wap.tarul.cn/Article/details/ghglxfupj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.bbcook.cn/Article/details/gswkmroqe.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.sjlbkw.cn/Article/details/gsskshvzx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.epnwcf.com/Article/details/gywmuueyq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.bbcook.cn/Article/details/gydtdntek.sHtML


<!-- 参考信息 -->