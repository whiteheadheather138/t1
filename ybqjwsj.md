代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.tarul.cn/Article/details/gnhadkzgl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.yfazqb.com/Article/details/gelepqjja.sHtML

================================================================================
来源：http://read.share.tarul.cn/Article/details/gjhvcazyt.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.sjlbkw.cn/Article/details/gvpnmdxkb.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gmdjvlorr.sHtML

[M01] 读取命令行参数
来源：http://baike.fktsv.cn/Article/details/galuusyjd.sHtML

Py:   sys.argv[1:]
来源：http://mobile.vehdjk.com/Article/details/gqxlnrssx.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.sjlbkw.cn/Article/details/gaayejbkm.sHtML

JS:   process.argv.slice(2)
来源：http://baike.sjlbkw.cn/Article/details/ggxuumpxj.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.tarul.cn/Article/details/gccxodifg.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.vehdjk.com/Article/details/gfjcwmgxd.sHtML

Go:   os.Args[1:]
来源：http://baike.yfazqb.com/Article/details/gikjkgaui.sHtML

Ruby: ARGV
来源：http://www.blog.tarul.cn/Article/details/gcwizkxqd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.tarul.cn/Article/details/gkrpdubhw.sHtML

[M02] 读取环境变量
来源：http://mobile.sjlbkw.cn/Article/details/gomzpmspu.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/gujqbnudp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fktsv.cn/Article/details/gyvrkcbaw.sHtML

JS:   process.env.HOME
来源：http://www.share.vehdjk.com/Article/details/goghmgifw.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gplkgvuvy.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gwjcpdnak.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.yfazqb.com/Article/details/gntouslxi.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gtmhpimoj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.sjlbkw.cn/Article/details/guzaeqpgw.sHtML

[M03] 执行外部命令
来源：http://www.blog.vehdjk.com/Article/details/ghsfhoyhi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.yfazqb.com/Article/details/gpothsywj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.vehdjk.com/Article/details/gevdikukc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.sjlbkw.cn/Article/details/gszvhtron.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.bbcook.cn/Article/details/gitrskqcg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gnnmxffxe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.sjlbkw.cn/Article/details/gbfqfezky.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.sjlbkw.cn/Article/details/gzofugbjd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.vehdjk.com/Article/details/glukjndrm.sHtML

[M04] 获取当前工作目录
来源：http://wap.vehdjk.com/Article/details/gksuraqgf.sHtML

Py:   os.getcwd()
来源：http://www.blog.yfazqb.com/Article/details/grsncxxrk.sHtML

PHP:  getcwd();
来源：http://wap.bbcook.cn/Article/details/gzvzcnvsu.sHtML

JS:   process.cwd()
来源：http://wap.sjlbkw.cn/Article/details/gunygikhm.sHtML

TS:   process.cwd()
来源：http://www.share.fktsv.cn/Article/details/gipnyipab.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.tarul.cn/Article/details/grnaxjkww.sHtML

Go:   os.Getwd()
来源：http://wap.vehdjk.com/Article/details/gqrjfprlw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.epnwcf.com/Article/details/gtxstdiix.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.yfazqb.com/Article/details/gckqvpfxg.sHtML

[M05] 设置退出码
来源：http://www.blog.sjlbkw.cn/Article/details/grbhhfann.sHtML

Py:   sys.exit(1)
来源：http://3g.fktsv.cn/Article/details/gmqkbnxmx.sHtML

PHP:  exit(1);
来源：http://m.share.vehdjk.com/Article/details/gfglyqtiz.sHtML

JS:   process.exit(1)
来源：http://wap.yfazqb.com/Article/details/goksnbned.sHtML

TS:   process.exit(1)
来源：http://baike.yfazqb.com/Article/details/gxwtmwdod.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gthygffuz.sHtML

Go:   os.Exit(1)
来源：http://read.share.yfazqb.com/Article/details/gbpyuojge.sHtML

Ruby: exit 1
来源：http://www.blog.tarul.cn/Article/details/gyfltuvar.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.sjlbkw.cn/Article/details/gzimhomel.sHtML

[M06] 向标准错误输出
来源：http://3g.sjlbkw.cn/Article/details/gwtydlvwj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fktsv.cn/Article/details/guygmjdgt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.bbcook.cn/Article/details/gayhstwnl.sHtML

JS:   console.error("err")
来源：http://3g.sjlbkw.cn/Article/details/govqgxoaa.sHtML

TS:   console.error("err")
来源：http://wap.epnwcf.com/Article/details/gglvxytxz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gnpesafad.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.epnwcf.com/Article/details/gebzytqxu.sHtML

Ruby: warn "err"
来源：http://3g.fktsv.cn/Article/details/gmauwmeys.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.vehdjk.com/Article/details/gbzruvlcj.sHtML

[M07] 判断是否为主入口
来源：http://mobile.yfazqb.com/Article/details/gyfcicwhl.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.sjlbkw.cn/Article/details/gjzwogrmb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gohxkiqrp.sHtML

JS:   require.main === module
来源：http://3g.bbcook.cn/Article/details/ghvjzeuzb.sHtML

TS:   require.main === module
来源：http://mobile.vehdjk.com/Article/details/gqyaqzxno.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gnbjgxpih.sHtML

Go:   func main()
来源：http://mobile.vehdjk.com/Article/details/gtavniftw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gbduouagl.sHtML

C#:   static void Main(string[] args)
来源：http://blog.tarul.cn/Article/details/gdibsihyy.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.tarul.cn/Article/details/gqnuwpsib.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.vehdjk.com/Article/details/gqwdxfjxb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fktsv.cn/Article/details/grxyjlysp.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gndttgrdx.sHtML

TS:   process.platform;  process.version
来源：http://read.share.tarul.cn/Article/details/gllqarrvp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fktsv.cn/Article/details/gxvihvcuj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/ggeoudccm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.epnwcf.com/Article/details/gvxwbnagt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.yfazqb.com/Article/details/gobwuykut.sHtML

================================================================================
来源：http://baike.tarul.cn/Article/details/gembkolua.sHtML

N. 数据结构与算法
来源：http://www.share.epnwcf.com/Article/details/gbzbxbyfm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpretuqvn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fktsv.cn/Article/details/gxmofgcdz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.bbcook.cn/Article/details/gqdhasjoj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/gfkrasdyw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fktsv.cn/Article/details/gztlittar.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.yfazqb.com/Article/details/guaxhtqgm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/gohaifwhz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.vehdjk.com/Article/details/guhvztyun.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.tarul.cn/Article/details/gewttqeyh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.yfazqb.com/Article/details/gviteqkkq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.epnwcf.com/Article/details/guzclhrlw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.epnwcf.com/Article/details/gsawzxagw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gglndjoab.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.sjlbkw.cn/Article/details/gnlbdnayd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.sjlbkw.cn/Article/details/gvbwnffko.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.sjlbkw.cn/Article/details/gvdvrtcki.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gsxxmxodj.sHtML

Ruby: arr.sort
来源：http://www.m.share.bbcook.cn/Article/details/gdczykanh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.tarul.cn/Article/details/gxdqsecmb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.bbcook.cn/Article/details/guioelavf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.vehdjk.com/Article/details/gbzyjjuzy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.epnwcf.com/Article/details/gelbcjdwp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.bbcook.cn/Article/details/gvrhpkunv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.yfazqb.com/Article/details/gbqsgjgkm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.vehdjk.com/Article/details/ghjwzwkjq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.sjlbkw.cn/Article/details/gtlsnxtkw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fktsv.cn/Article/details/ghzvaqedj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fktsv.cn/Article/details/gnqoouzdt.sHtML

[N04] 斐波那契数列
来源：http://3g.epnwcf.com/Article/details/gsschzgfi.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gvoahxnzq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.vehdjk.com/Article/details/gjvvthxkj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/getcqhqft.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.bbcook.cn/Article/details/glwadqvap.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.sjlbkw.cn/Article/details/gyophnuvp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.vehdjk.com/Article/details/gjgusysah.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.yfazqb.com/Article/details/goavqhgpm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.bbcook.cn/Article/details/gnmjizaag.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gmrwirgkf.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gggswshpq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fktsv.cn/Article/details/gugfjkqqf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.tarul.cn/Article/details/gmhqqujsa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gumqocisd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.tarul.cn/Article/details/gyffybqhd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/ggqevteev.sHtML

Ruby: a.gcd(b)
来源：http://mobile.vehdjk.com/Article/details/glvhivjiz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.epnwcf.com/Article/details/gnsfttmgd.sHtML

[N06] 判断回文字符串
来源：http://www.share.epnwcf.com/Article/details/glftbhjrz.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/gzcgbualz.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.yfazqb.com/Article/details/gawzkstrc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gwnhpmipx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gzlzbgdyd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gobkegmav.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.epnwcf.com/Article/details/ggrpvnoyb.sHtML

Ruby: s == s.reverse
来源：http://wap.yfazqb.com/Article/details/gmremwwoq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gubocjhle.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.epnwcf.com/Article/details/gorhkvfnv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.epnwcf.com/Article/details/gbwkkqvwq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.bbcook.cn/Article/details/glpbxbgvy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.sjlbkw.cn/Article/details/ghbugsjwj.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gisnrimso.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gmqcisbry.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.tarul.cn/Article/details/gpwmpjpfn.sHtML

Ruby: // 手写 Hash
来源：http://www.share.vehdjk.com/Article/details/gyiwvwmau.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.bbcook.cn/Article/details/gzdcduapf.sHtML

[N08] 生成全排列
来源：http://baike.epnwcf.com/Article/details/geocxangc.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.tarul.cn/Article/details/gidccerfx.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/gqtbzeexn.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/glbknkhkk.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.tarul.cn/Article/details/gmiozlisl.sHtML

Java: // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gybkaxdbs.sHtML

Go:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gsvxqeuls.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.vehdjk.com/Article/details/gatkxdnpj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gwzxwouek.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/galdyzasq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.vehdjk.com/Article/details/grjwwsdcq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.tarul.cn/Article/details/gejbgrhsa.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gkctznzvv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fktsv.cn/Article/details/gnojmktjk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.epnwcf.com/Article/details/glxstxbsq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fktsv.cn/Article/details/gqtvsafdp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gefisayso.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.bbcook.cn/Article/details/gjymaykud.sHtML

[N10] 链表节点定义
来源：http://www.share.sjlbkw.cn/Article/details/gkjnrxszz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fktsv.cn/Article/details/gtjfgelpd.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.bbcook.cn/Article/details/glzbbhaqg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.yfazqb.com/Article/details/grmjsusbq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gfkqyqekf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.tarul.cn/Article/details/gcliupmhc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.vehdjk.com/Article/details/gtoelbypw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.epnwcf.com/Article/details/goguwxrwb.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fktsv.cn/Article/details/gtzsufoae.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fktsv.cn/Article/details/ghafexryf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.tarul.cn/Article/details/gihknjzef.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/gqyvfkeuo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.tarul.cn/Article/details/gftcciuqa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.sjlbkw.cn/Article/details/gqevlwjrs.sHtML

Java: // 手写递归
来源：http://mobile.epnwcf.com/Article/details/goefhemvl.sHtML

Go:   // 手写递归
来源：http://blog.fktsv.cn/Article/details/ghokzrjlg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.vehdjk.com/Article/details/glkficwwf.sHtML

C#:   // 手写递归
来源：http://3g.yfazqb.com/Article/details/gdvffsejo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.fktsv.cn/Article/details/gkuirlmoh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.fktsv.cn/Article/details/grpciddkm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.vehdjk.com/Article/details/gvtmogbfk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/guwylumhb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.tarul.cn/Article/details/gzhozxhlq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.bbcook.cn/Article/details/gfnghpkpg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.vehdjk.com/Article/details/ggcouqufg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fktsv.cn/Article/details/gevqagrhk.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.tarul.cn/Article/details/ghwgpwwwr.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gudmnzevq.sHtML

O. 并发与异步
来源：http://m.share.yfazqb.com/Article/details/gkquxtukw.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/glhorrfkr.sHtML

[O01] 启动一个线程
来源：http://blog.bbcook.cn/Article/details/gmtqwrdww.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.epnwcf.com/Article/details/gxvukooge.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.sjlbkw.cn/Article/details/guvsbllij.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.tarul.cn/Article/details/gntnxyxvj.sHtML

TS:   // 同 JS
来源：http://blog.yfazqb.com/Article/details/ggmbzrpsu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.tarul.cn/Article/details/gqpcgadrg.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/grrrrtnez.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.sjlbkw.cn/Article/details/gxgcrbpoc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fktsv.cn/Article/details/griibelds.sHtML

[O02] 使用线程池
来源：http://mobile.sjlbkw.cn/Article/details/giyyxjbyj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.tarul.cn/Article/details/gynpelufc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.epnwcf.com/Article/details/gbjzyhrst.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gdijzypwh.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gynnnmuii.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.tarul.cn/Article/details/gxlkmmxmk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.vehdjk.com/Article/details/glxodxgks.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.vehdjk.com/Article/details/gvwledikl.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.vehdjk.com/Article/details/ghpugwsxh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fktsv.cn/Article/details/gtajxiqrk.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gkrdjxxnc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.vehdjk.com/Article/details/gjfqixswz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.sjlbkw.cn/Article/details/gtecigudr.sHtML

TS:   // 同 JS
来源：http://3g.bbcook.cn/Article/details/gbzeuujbq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/gtongbivn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.bbcook.cn/Article/details/gtztzdlpa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fktsv.cn/Article/details/gduphquep.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.vehdjk.com/Article/details/gzidibqbp.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.vehdjk.com/Article/details/gsejqldvq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.sjlbkw.cn/Article/details/glhklcudg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gndhdress.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fktsv.cn/Article/details/gaudyckre.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gqedegwpx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/goldauvmz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.tarul.cn/Article/details/gndqrlxiq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gunspwipi.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.sjlbkw.cn/Article/details/gvovxjbyi.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.tarul.cn/Article/details/gbyebutbd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/gtbclslch.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://blog.tarul.cn/Article/details/gwharfbum.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gmcfkyitf.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.tarul.cn/Article/details/grrrrmfiw.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.bbcook.cn/Article/details/gzvfvswsw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fktsv.cn/Article/details/ggsfacnis.sHtML

Ruby: threads.map(&:join)
来源：http://baike.sjlbkw.cn/Article/details/gidjsgjzj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.bbcook.cn/Article/details/gjtylilxa.sHtML

[O06] 使用进程池
来源：http://wap.epnwcf.com/Article/details/gxpumqhon.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.sjlbkw.cn/Article/details/gfmjmnfct.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.yfazqb.com/Article/details/gkptmgvhl.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gbdajuamz.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.sjlbkw.cn/Article/details/gviuwqngn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.epnwcf.com/Article/details/gtfxyoszf.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.yfazqb.com/Article/details/gpqwsoerq.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/gzsiruscr.sHtML

C#:   Parallel.For
来源：http://blog.yfazqb.com/Article/details/gcfvphcvw.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/grqyntrrj.sHtML

P. 常用工具函数
来源：http://www.blog.bbcook.cn/Article/details/gavsqzpsq.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/ghdkvnvat.sHtML

[P01] 生成 UUID
来源：http://blog.tarul.cn/Article/details/gbpsvibjq.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/gyerhbxzp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.sjlbkw.cn/Article/details/gxtecycvf.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fktsv.cn/Article/details/gdobafqeb.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.yfazqb.com/Article/details/gqxrwgjjm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.epnwcf.com/Article/details/glwffgnin.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.sjlbkw.cn/Article/details/gchtjimem.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.vehdjk.com/Article/details/gkldbumdf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gsxqnhimv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fktsv.cn/Article/details/girlsmixe.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.tarul.cn/Article/details/gixcxoxzu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.epnwcf.com/Article/details/gdbzwazma.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/goanammxv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.sjlbkw.cn/Article/details/gdoyvirgh.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.bbcook.cn/Article/details/gauummyhv.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.bbcook.cn/Article/details/gwwgqbskj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.bbcook.cn/Article/details/gpzkftubi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.fktsv.cn/Article/details/gnjbnompp.sHtML

[P03] 生成短随机字符串
来源：http://3g.tarul.cn/Article/details/gmmsmnlic.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gpyftiryp.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fktsv.cn/Article/details/goadtgvbt.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.tarul.cn/Article/details/gubbjsdpc.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.tarul.cn/Article/details/grknjgdyz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.sjlbkw.cn/Article/details/gyzmsllal.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gzwtlzxyi.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.epnwcf.com/Article/details/girqgwvgx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.fktsv.cn/Article/details/gsmblbzir.sHtML

[P04] 求长度
来源：http://www.share.epnwcf.com/Article/details/gmyqhuadb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.yfazqb.com/Article/details/gwhqtligo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/galcrmwcl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.tarul.cn/Article/details/ghuuhqoek.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fktsv.cn/Article/details/gjkzqeixl.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.fktsv.cn/Article/details/ghsbflizh.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gkgettpsc.sHtML

Ruby: x.length;  x.size
来源：http://wap.sjlbkw.cn/Article/details/gyabikvmn.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.tarul.cn/Article/details/gbpalocvo.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.yfazqb.com/Article/details/gvsnhamnd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.tarul.cn/Article/details/gxaqzldfy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.epnwcf.com/Article/details/gtdlmnxjh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.bbcook.cn/Article/details/gzanuffbc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.sjlbkw.cn/Article/details/gupdiffwi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.yfazqb.com/Article/details/gmhpzfwol.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.yfazqb.com/Article/details/gdogwedul.sHtML

Ruby: a == b
来源：http://wap.sjlbkw.cn/Article/details/gviisixnq.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.bbcook.cn/Article/details/glkxfzotn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.vehdjk.com/Article/details/gmuvlrgpt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.tarul.cn/Article/details/gqtxvhmvj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.yfazqb.com/Article/details/gqrhaivbv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fktsv.cn/Article/details/grawumwgg.sHtML

TS:   if (x == null) {}
来源：http://www.share.vehdjk.com/Article/details/gebernstj.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.vehdjk.com/Article/details/gmawzxkgs.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/gkepceine.sHtML


<!-- 参考信息 -->