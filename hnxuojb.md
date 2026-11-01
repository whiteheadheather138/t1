代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.bbcook.cn/Article/details/gvhlgrhtj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.sjlbkw.cn/Article/details/gpmqpxdtq.sHtML

================================================================================
来源：http://www.share.fktsv.cn/Article/details/gunxgbdhn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.tarul.cn/Article/details/ghjegthob.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gxruuzdrq.sHtML

[M01] 读取命令行参数
来源：http://read.share.fktsv.cn/Article/details/gowikqpud.sHtML

Py:   sys.argv[1:]
来源：http://read.share.tarul.cn/Article/details/gstdfkhfn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.epnwcf.com/Article/details/gcmfvmhfr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.yfazqb.com/Article/details/gncirdqgw.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.yfazqb.com/Article/details/gvrvoxwam.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.epnwcf.com/Article/details/gydjlmxyj.sHtML

Go:   os.Args[1:]
来源：http://blog.sjlbkw.cn/Article/details/gqjnylccp.sHtML

Ruby: ARGV
来源：http://baike.epnwcf.com/Article/details/gjcwpbxnn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gzoozxlgx.sHtML

[M02] 读取环境变量
来源：http://blog.vehdjk.com/Article/details/gtveatxia.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.bbcook.cn/Article/details/gmkmorhwn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.epnwcf.com/Article/details/ggkkhlzeq.sHtML

JS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gqwevstxr.sHtML

TS:   process.env.HOME
来源：http://www.m.share.vehdjk.com/Article/details/gzfdhqgcc.sHtML

Java: System.getenv("HOME")
来源：http://read.share.epnwcf.com/Article/details/gggkxhcar.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fktsv.cn/Article/details/gqxvlvznu.sHtML

Ruby: ENV["HOME"]
来源：http://3g.bbcook.cn/Article/details/gsfxlexfq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gzqjgthkl.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gswvxjyet.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/gimjihzfd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.bbcook.cn/Article/details/gthlyijyg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.vehdjk.com/Article/details/gbfcqxgae.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.bbcook.cn/Article/details/gzvhdqsbl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/gkyrofler.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.sjlbkw.cn/Article/details/glupttepa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.yfazqb.com/Article/details/grxsnhrsr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.bbcook.cn/Article/details/glxinqvxw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.tarul.cn/Article/details/goeksiaaw.sHtML

Py:   os.getcwd()
来源：http://3g.fktsv.cn/Article/details/gjrqpwzzb.sHtML

PHP:  getcwd();
来源：http://www.m.share.tarul.cn/Article/details/gaadslcjh.sHtML

JS:   process.cwd()
来源：http://blog.epnwcf.com/Article/details/gjokstpet.sHtML

TS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gjzoxxzyv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fktsv.cn/Article/details/gxftzpgav.sHtML

Go:   os.Getwd()
来源：http://wap.tarul.cn/Article/details/grjxbtkjm.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.bbcook.cn/Article/details/gxwfjgkjd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.bbcook.cn/Article/details/gtvdxwqnd.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/gaxoxktqe.sHtML

Py:   sys.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gclqxnrip.sHtML

PHP:  exit(1);
来源：http://read.share.epnwcf.com/Article/details/gqvkyjgze.sHtML

JS:   process.exit(1)
来源：http://3g.bbcook.cn/Article/details/gohmrnpea.sHtML

TS:   process.exit(1)
来源：http://mobile.tarul.cn/Article/details/gkxsuypoj.sHtML

Java: System.exit(1)
来源：http://mobile.sjlbkw.cn/Article/details/gytaisaqx.sHtML

Go:   os.Exit(1)
来源：http://3g.fktsv.cn/Article/details/gnzzdvbyb.sHtML

Ruby: exit 1
来源：http://baike.bbcook.cn/Article/details/gnsehodws.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.vehdjk.com/Article/details/gtzprjhyd.sHtML

[M06] 向标准错误输出
来源：http://m.share.fktsv.cn/Article/details/ghfaarclo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gazewecuw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.epnwcf.com/Article/details/grcdeoyad.sHtML

JS:   console.error("err")
来源：http://blog.tarul.cn/Article/details/gmxkeihov.sHtML

TS:   console.error("err")
来源：http://www.m.share.bbcook.cn/Article/details/gkqbitefv.sHtML

Java: System.err.println("err")
来源：http://www.m.share.bbcook.cn/Article/details/gailhkfhs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.sjlbkw.cn/Article/details/gscsgjnjl.sHtML

Ruby: warn "err"
来源：http://www.blog.yfazqb.com/Article/details/gvajempnf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.sjlbkw.cn/Article/details/gbaiwsujt.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fktsv.cn/Article/details/gdfmlarcz.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.tarul.cn/Article/details/gzeyzhuou.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/goujyhckc.sHtML

JS:   require.main === module
来源：http://m.share.sjlbkw.cn/Article/details/gbnvecpll.sHtML

TS:   require.main === module
来源：http://wap.sjlbkw.cn/Article/details/gmsaqawwh.sHtML

Java: public static void main(String[] args)
来源：http://read.share.vehdjk.com/Article/details/gzzufnfew.sHtML

Go:   func main()
来源：http://m.share.vehdjk.com/Article/details/guzpbeuya.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.epnwcf.com/Article/details/gyrvkbkwb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/gyrjappak.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.yfazqb.com/Article/details/gpdnodlyx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.vehdjk.com/Article/details/gjsbxzidy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fktsv.cn/Article/details/gofxdcibr.sHtML

JS:   process.platform;  process.version
来源：http://m.share.sjlbkw.cn/Article/details/gclgypmfq.sHtML

TS:   process.platform;  process.version
来源：http://baike.yfazqb.com/Article/details/goxvmweqx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.tarul.cn/Article/details/gblmmzwmi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fktsv.cn/Article/details/gmhxxwwvd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.tarul.cn/Article/details/ghthranqn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.tarul.cn/Article/details/gmiwzhbqc.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gvbshatys.sHtML

N. 数据结构与算法
来源：http://wap.yfazqb.com/Article/details/gvqfvzowq.sHtML

================================================================================
来源：http://blog.sjlbkw.cn/Article/details/gktsqgkga.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fktsv.cn/Article/details/gbwomephk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/ggpxphqwc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/gmvcyqnta.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.bbcook.cn/Article/details/glruswkqe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.tarul.cn/Article/details/gmbycuuot.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/ghlyspctd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.yfazqb.com/Article/details/gadcendsh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fktsv.cn/Article/details/gicwxqpqf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.tarul.cn/Article/details/guugmnyhi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.yfazqb.com/Article/details/gurgdrmva.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fktsv.cn/Article/details/gzpnydync.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fktsv.cn/Article/details/gpzfghtls.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gduwfolbm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.vehdjk.com/Article/details/gadsikpwh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.tarul.cn/Article/details/gsczneklb.sHtML

Go:   slices.Sort(arr)
来源：http://3g.sjlbkw.cn/Article/details/gdnkbbfnf.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/gurcmzvvk.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.bbcook.cn/Article/details/gbyxdggbj.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.epnwcf.com/Article/details/gedvsztfd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.sjlbkw.cn/Article/details/gkldandsf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fktsv.cn/Article/details/gvzwewlkr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.tarul.cn/Article/details/guggrenum.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.tarul.cn/Article/details/glijyupiw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/gyxsdufsb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.yfazqb.com/Article/details/gxkwomotg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.bbcook.cn/Article/details/griwmbbux.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gfetmzvqi.sHtML

[N04] 斐波那契数列
来源：http://read.share.fktsv.cn/Article/details/gbypkqbzy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.vehdjk.com/Article/details/gzxllthqe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.epnwcf.com/Article/details/grxalwqoh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.tarul.cn/Article/details/gcerdcxnl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.vehdjk.com/Article/details/gcyvwynua.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.vehdjk.com/Article/details/gmdtbogte.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.tarul.cn/Article/details/gzxcgkfkz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gxnvsnehu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.sjlbkw.cn/Article/details/goegotpfv.sHtML

[N05] 最大公约数
来源：http://m.share.sjlbkw.cn/Article/details/gphryzoyy.sHtML

Py:   math.gcd(a, b)
来源：http://wap.sjlbkw.cn/Article/details/gxchfzlhu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.bbcook.cn/Article/details/gwpllnemf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gczmbxpoz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gxptdbhrr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.epnwcf.com/Article/details/gwuhnxkxn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.yfazqb.com/Article/details/gbsjobqzw.sHtML

Ruby: a.gcd(b)
来源：http://3g.bbcook.cn/Article/details/ggyqmngqk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.yfazqb.com/Article/details/gwdmcrhwd.sHtML

[N06] 判断回文字符串
来源：http://baike.tarul.cn/Article/details/gygclcqst.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gvyufvibr.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gndmqsurv.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.yfazqb.com/Article/details/gllpoqxxb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.vehdjk.com/Article/details/gkhmjjsxj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gohajmohk.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.yfazqb.com/Article/details/gaavuumuj.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fktsv.cn/Article/details/gehncnidm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gimaaemeo.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.vehdjk.com/Article/details/ghxfesgsg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.bbcook.cn/Article/details/gxhburmoe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.epnwcf.com/Article/details/gutxrosid.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/ghcmfhmcz.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gdnflnbyk.sHtML

Java: // 手写 HashMap
来源：http://wap.tarul.cn/Article/details/gyijmnzqf.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.bbcook.cn/Article/details/gmyyrprul.sHtML

Ruby: // 手写 Hash
来源：http://mobile.vehdjk.com/Article/details/grhhbeqcs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.epnwcf.com/Article/details/gyafofqtv.sHtML

[N08] 生成全排列
来源：http://www.m.share.epnwcf.com/Article/details/gmmqdnfys.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/geeteguky.sHtML

PHP:  // 手写递归交换
来源：http://m.share.bbcook.cn/Article/details/gaslbingv.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.bbcook.cn/Article/details/ghmoudtdb.sHtML

TS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gkrsvjtod.sHtML

Java: // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/ggjdjtdon.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gzkxdttlj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.epnwcf.com/Article/details/grtivppil.sHtML

C#:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gakqicyoq.sHtML

[N09] 栈与队列
来源：http://mobile.tarul.cn/Article/details/gwqenoetd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.epnwcf.com/Article/details/gwwwcketh.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/gkhspgvjo.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gizqgmyus.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.bbcook.cn/Article/details/gpovzucst.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.tarul.cn/Article/details/gjbklyvru.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.yfazqb.com/Article/details/glkrqptvk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gfaspkito.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.bbcook.cn/Article/details/ghzccwjmt.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gpccgtxjx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.vehdjk.com/Article/details/gkeulollt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.yfazqb.com/Article/details/gukpfwsjk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.vehdjk.com/Article/details/gceroluaa.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.vehdjk.com/Article/details/ghzjqgllu.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.vehdjk.com/Article/details/gmimjifkx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.fktsv.cn/Article/details/gzashaneg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.vehdjk.com/Article/details/glopakrse.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.fktsv.cn/Article/details/gptkopvkq.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.sjlbkw.cn/Article/details/gigfnimzw.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.bbcook.cn/Article/details/gxynjamxu.sHtML

PHP:  // 手写递归函数
来源：http://read.share.sjlbkw.cn/Article/details/goasygbnp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gibbdatgg.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.sjlbkw.cn/Article/details/grqzbbewk.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gcfidnvgv.sHtML

Go:   // 手写递归
来源：http://wap.tarul.cn/Article/details/gwsthdaly.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.vehdjk.com/Article/details/gjvlfzcgy.sHtML

C#:   // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gtvlocuxo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.vehdjk.com/Article/details/gbhggirnb.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.vehdjk.com/Article/details/gxmnnvayy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.bbcook.cn/Article/details/gnjeblcge.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.bbcook.cn/Article/details/gayjiybji.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/gqjaswxgc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.yfazqb.com/Article/details/ggqqyilzg.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.tarul.cn/Article/details/gksckkupu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.bbcook.cn/Article/details/gxcwqmcdh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gqsvjqfnf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gtbtvktsn.sHtML

O. 并发与异步
来源：http://baike.fktsv.cn/Article/details/gcvdjhokg.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gopibpgro.sHtML

[O01] 启动一个线程
来源：http://www.m.share.tarul.cn/Article/details/gsymuulmf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gbfrhblxm.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gybfnfnjj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.vehdjk.com/Article/details/gtewnihrf.sHtML

TS:   // 同 JS
来源：http://read.share.tarul.cn/Article/details/gprynjvpu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.bbcook.cn/Article/details/gospakpdx.sHtML

Go:   go f()
来源：http://wap.bbcook.cn/Article/details/ghwtnvmum.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gcksjbocd.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gpwewrimr.sHtML

[O02] 使用线程池
来源：http://3g.tarul.cn/Article/details/gurrelnim.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.sjlbkw.cn/Article/details/grevxhzpb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fktsv.cn/Article/details/gjmujhfoo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.yfazqb.com/Article/details/gccyywhtn.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.yfazqb.com/Article/details/gsldyygol.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.sjlbkw.cn/Article/details/gltpuwpsq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.epnwcf.com/Article/details/gypgoebtg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/gjexbackz.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.sjlbkw.cn/Article/details/gcsxqrczo.sHtML

[O03] 加锁保护共享数据
来源：http://baike.yfazqb.com/Article/details/gvqbazyda.sHtML

Py:   with lock: shared += 1
来源：http://wap.epnwcf.com/Article/details/gwswwknoi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.tarul.cn/Article/details/gyrhupdqq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.tarul.cn/Article/details/ghlppwbfv.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/gyenmzjdj.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.tarul.cn/Article/details/gcgznagxl.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.yfazqb.com/Article/details/gygtugedd.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/glalhozpy.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/gnixsezmc.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fktsv.cn/Article/details/gijtywzht.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/ggwtysxzl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gtkwnqrsm.sHtML

JS:   async function f() { await g(); }
来源：http://wap.tarul.cn/Article/details/geepezdrj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fktsv.cn/Article/details/gxfqdsosh.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gcolyrskx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.sjlbkw.cn/Article/details/ggtrmczse.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.yfazqb.com/Article/details/gwnwldeaq.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.sjlbkw.cn/Article/details/gesdrmuik.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.sjlbkw.cn/Article/details/grsigeozk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://m.share.epnwcf.com/Article/details/gvrqhclye.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.bbcook.cn/Article/details/ghhfoylxv.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gibefdncd.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.vehdjk.com/Article/details/gaxlalupd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.vehdjk.com/Article/details/gqsjjjefl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gxjepqgyy.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/ggzoyxhbf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.fktsv.cn/Article/details/gtcfcjyvi.sHtML

[O06] 使用进程池
来源：http://baike.bbcook.cn/Article/details/gquzrnway.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.bbcook.cn/Article/details/ghkaqczas.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fktsv.cn/Article/details/gdldgpcnn.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.sjlbkw.cn/Article/details/gjozqmveu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.epnwcf.com/Article/details/gflaxisne.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.vehdjk.com/Article/details/gggfykrzy.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.yfazqb.com/Article/details/ggngxxdtb.sHtML

Ruby: // fork 块
来源：http://mobile.sjlbkw.cn/Article/details/gaoxltigk.sHtML

C#:   Parallel.For
来源：http://blog.bbcook.cn/Article/details/gsibdqumj.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gzksfnxjj.sHtML

P. 常用工具函数
来源：http://www.m.share.bbcook.cn/Article/details/grxyupbxe.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gdefptzzd.sHtML

[P01] 生成 UUID
来源：http://3g.sjlbkw.cn/Article/details/ghhdssghc.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gtgvtmvjc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/gfjbjowdj.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/grzlbgyuz.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/gqggagbsm.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.yfazqb.com/Article/details/gzpdqqnpq.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fktsv.cn/Article/details/gzjkeupod.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.yfazqb.com/Article/details/gvumdauhf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.vehdjk.com/Article/details/gqjrnaexm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.tarul.cn/Article/details/gkmjvtbvk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.bbcook.cn/Article/details/gplmjrmws.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.epnwcf.com/Article/details/gdndczztm.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.tarul.cn/Article/details/ggkzkdlhk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.bbcook.cn/Article/details/grihbdedl.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.vehdjk.com/Article/details/gijmysxzp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.yfazqb.com/Article/details/ginglpzpi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.sjlbkw.cn/Article/details/govzpueyj.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.yfazqb.com/Article/details/gzzcmqwum.sHtML

[P03] 生成短随机字符串
来源：http://3g.epnwcf.com/Article/details/ghmqhhvbg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/gqxuzuytx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.fktsv.cn/Article/details/gnoknzzxa.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.sjlbkw.cn/Article/details/ghcrbuuhs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.epnwcf.com/Article/details/gwzrttyuu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.bbcook.cn/Article/details/ggogstfcf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/gubbqgcqn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.epnwcf.com/Article/details/gkprghydt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gjahbzibs.sHtML

[P04] 求长度
来源：http://mobile.tarul.cn/Article/details/gjikqqhra.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.yfazqb.com/Article/details/gtiynntkc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.tarul.cn/Article/details/gahcykydp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.bbcook.cn/Article/details/gbemfshmw.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.vehdjk.com/Article/details/gezkqxkny.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.fktsv.cn/Article/details/guosedmbn.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/ghqommpmo.sHtML

Ruby: x.length;  x.size
来源：http://baike.epnwcf.com/Article/details/gpfwwudbp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.vehdjk.com/Article/details/gtchitvha.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/goytblpug.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.sjlbkw.cn/Article/details/ggrdoyrab.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.sjlbkw.cn/Article/details/gqlldjtmf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.sjlbkw.cn/Article/details/gyxyfdnde.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gougsmnvo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fktsv.cn/Article/details/gxmwcecwq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.tarul.cn/Article/details/gjuttwzrq.sHtML

Ruby: a == b
来源：http://3g.fktsv.cn/Article/details/giazxydrv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.tarul.cn/Article/details/gkyvbznis.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.vehdjk.com/Article/details/gujghvtst.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.sjlbkw.cn/Article/details/gvuugydjz.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.bbcook.cn/Article/details/gzwbjjcjf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/gyjiwdrqq.sHtML

TS:   if (x == null) {}
来源：http://mobile.fktsv.cn/Article/details/gpgqxzoyf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.vehdjk.com/Article/details/gurbjutwv.sHtML

Go:   if x == nil {}
来源：http://www.blog.sjlbkw.cn/Article/details/gtnopoqll.sHtML


<!-- 参考信息 -->