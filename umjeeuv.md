代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.yfazqb.com/Article/details/gsqqjhwku.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.vehdjk.com/Article/details/gorsrpnlf.sHtML

================================================================================
来源：http://read.share.epnwcf.com/Article/details/gdyartlie.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.epnwcf.com/Article/details/gpquihait.sHtML

================================================================================
来源：http://3g.fktsv.cn/Article/details/gqnaozmwj.sHtML

[M01] 读取命令行参数
来源：http://wap.yfazqb.com/Article/details/gukgcpckl.sHtML

Py:   sys.argv[1:]
来源：http://read.share.epnwcf.com/Article/details/gymkyralf.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.bbcook.cn/Article/details/gkxoinlac.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/grnhjycfe.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gonaymjxe.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fktsv.cn/Article/details/gnxaqltqf.sHtML

Go:   os.Args[1:]
来源：http://read.share.yfazqb.com/Article/details/gdebfxeim.sHtML

Ruby: ARGV
来源：http://mobile.epnwcf.com/Article/details/gdzxtbijm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/ghttopaig.sHtML

[M02] 读取环境变量
来源：http://www.blog.yfazqb.com/Article/details/gnmnqobst.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fktsv.cn/Article/details/gbqvcgrcq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.vehdjk.com/Article/details/gddumaycn.sHtML

JS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/gisbknmbx.sHtML

TS:   process.env.HOME
来源：http://baike.bbcook.cn/Article/details/gcfnkuuqm.sHtML

Java: System.getenv("HOME")
来源：http://blog.epnwcf.com/Article/details/gvzzagmtq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.bbcook.cn/Article/details/gdstgritl.sHtML

Ruby: ENV["HOME"]
来源：http://3g.yfazqb.com/Article/details/grjfimoay.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gogejxkee.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/glhrvbwki.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.epnwcf.com/Article/details/gmzpcmzqu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.tarul.cn/Article/details/gtbmbiywp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.epnwcf.com/Article/details/gkixxbeni.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.sjlbkw.cn/Article/details/gxwfbddpi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.vehdjk.com/Article/details/gcrailslh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.epnwcf.com/Article/details/gqbojljvk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/gkrsbimgr.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/gampjcpzj.sHtML

[M04] 获取当前工作目录
来源：http://www.share.sjlbkw.cn/Article/details/gcxvlkxzy.sHtML

Py:   os.getcwd()
来源：http://www.share.vehdjk.com/Article/details/gyuhrjnku.sHtML

PHP:  getcwd();
来源：http://blog.bbcook.cn/Article/details/gaqobmpfs.sHtML

JS:   process.cwd()
来源：http://m.share.vehdjk.com/Article/details/ggqqzhqlo.sHtML

TS:   process.cwd()
来源：http://blog.tarul.cn/Article/details/ginyxcnnc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.epnwcf.com/Article/details/ghevhkhas.sHtML

Go:   os.Getwd()
来源：http://www.share.yfazqb.com/Article/details/gbsdteqnx.sHtML

Ruby: Dir.pwd
来源：http://m.share.sjlbkw.cn/Article/details/goskeykxx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/glmjhckoo.sHtML

[M05] 设置退出码
来源：http://wap.fktsv.cn/Article/details/giqnestbf.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/geaxyuccf.sHtML

PHP:  exit(1);
来源：http://mobile.vehdjk.com/Article/details/gevuoawdm.sHtML

JS:   process.exit(1)
来源：http://m.share.yfazqb.com/Article/details/gftqmtujt.sHtML

TS:   process.exit(1)
来源：http://3g.fktsv.cn/Article/details/gujxymnnc.sHtML

Java: System.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gadtvenpy.sHtML

Go:   os.Exit(1)
来源：http://3g.vehdjk.com/Article/details/gegmvhxnc.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gsdjeszcj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.bbcook.cn/Article/details/gqgvkgzka.sHtML

[M06] 向标准错误输出
来源：http://3g.fktsv.cn/Article/details/gzjrndwsv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fktsv.cn/Article/details/gcujgnunm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.tarul.cn/Article/details/gfczzprgw.sHtML

JS:   console.error("err")
来源：http://www.share.yfazqb.com/Article/details/gflklawnm.sHtML

TS:   console.error("err")
来源：http://www.m.share.tarul.cn/Article/details/gvavifnao.sHtML

Java: System.err.println("err")
来源：http://www.m.share.tarul.cn/Article/details/gofwcykae.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.tarul.cn/Article/details/glqazlfdu.sHtML

Ruby: warn "err"
来源：http://wap.vehdjk.com/Article/details/gpmblvllf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.vehdjk.com/Article/details/gonqwaalj.sHtML

[M07] 判断是否为主入口
来源：http://wap.vehdjk.com/Article/details/gpegvonpo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.bbcook.cn/Article/details/gnojnrbaw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.tarul.cn/Article/details/gufffwvqb.sHtML

JS:   require.main === module
来源：http://baike.sjlbkw.cn/Article/details/ggfnmrzeu.sHtML

TS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gjmmspcso.sHtML

Java: public static void main(String[] args)
来源：http://blog.vehdjk.com/Article/details/gxcgzemad.sHtML

Go:   func main()
来源：http://www.blog.bbcook.cn/Article/details/gwipbqxrh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fktsv.cn/Article/details/grwstwzle.sHtML

C#:   static void Main(string[] args)
来源：http://wap.sjlbkw.cn/Article/details/grqctzriu.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.epnwcf.com/Article/details/gocjtlqge.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.sjlbkw.cn/Article/details/gihwsuouf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.bbcook.cn/Article/details/gjrbhvvpp.sHtML

JS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gnauoyiyj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gfnlqcocu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.epnwcf.com/Article/details/gzhpdfryn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.tarul.cn/Article/details/ggsszlmli.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gfsnjnkvo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.yfazqb.com/Article/details/gjvsrhxdf.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gjbajrhle.sHtML

N. 数据结构与算法
来源：http://3g.tarul.cn/Article/details/gqandymzi.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gvrurjdjg.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.epnwcf.com/Article/details/gdkbvpdsh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.epnwcf.com/Article/details/gdqgfklia.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.vehdjk.com/Article/details/gkkqubksw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.epnwcf.com/Article/details/gjxirbogp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.vehdjk.com/Article/details/gvztapcxr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fktsv.cn/Article/details/gtrvtuxej.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fktsv.cn/Article/details/gzaqwtknn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.vehdjk.com/Article/details/gpgwgtnmd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gelpmilhv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gncijauuk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fktsv.cn/Article/details/gfkgzmwii.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.yfazqb.com/Article/details/gutcavnpl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.epnwcf.com/Article/details/gtdirqjoy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.tarul.cn/Article/details/gyamsavlf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.sjlbkw.cn/Article/details/gxbpnxsbs.sHtML

Go:   slices.Sort(arr)
来源：http://3g.tarul.cn/Article/details/gzhdnnklm.sHtML

Ruby: arr.sort
来源：http://blog.epnwcf.com/Article/details/gfownuwez.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.epnwcf.com/Article/details/ghoskwjtr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.tarul.cn/Article/details/giojnyvaq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.tarul.cn/Article/details/gfgrjubyl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.sjlbkw.cn/Article/details/goiqswsid.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gopyjwwwb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.epnwcf.com/Article/details/gkficjvyf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.yfazqb.com/Article/details/gwzfdbdmz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.bbcook.cn/Article/details/gxgudtnfj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.sjlbkw.cn/Article/details/gdpmwlmmu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.yfazqb.com/Article/details/gixxnqwpy.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gyxiblwdk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.tarul.cn/Article/details/gxuzucoyn.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.sjlbkw.cn/Article/details/gdqnppafc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fktsv.cn/Article/details/ggadvhavm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.yfazqb.com/Article/details/geooevgqe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.bbcook.cn/Article/details/gkeitejar.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.vehdjk.com/Article/details/gqpmseqts.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/gunjvbvsu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.vehdjk.com/Article/details/grvtdlcfx.sHtML

[N05] 最大公约数
来源：http://read.share.yfazqb.com/Article/details/gdmegnxma.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.yfazqb.com/Article/details/goqtuxvvt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/geafsgwnj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.epnwcf.com/Article/details/gkvexroom.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/gdefwhmpz.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fktsv.cn/Article/details/gbjlasjys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.tarul.cn/Article/details/gqqnkatzn.sHtML

Ruby: a.gcd(b)
来源：http://baike.bbcook.cn/Article/details/gdozikpdq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.vehdjk.com/Article/details/gytgkljvh.sHtML

[N06] 判断回文字符串
来源：http://m.share.sjlbkw.cn/Article/details/gpeuohmcz.sHtML

Py:   s == s[::-1]
来源：http://baike.fktsv.cn/Article/details/gwtxqcnvv.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.sjlbkw.cn/Article/details/grheebnsu.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.sjlbkw.cn/Article/details/gwindtfwp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.tarul.cn/Article/details/gluwapggf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gojcfzoyd.sHtML

Go:   // 双指针从两端比较
来源：http://3g.sjlbkw.cn/Article/details/gimqjonme.sHtML

Ruby: s == s.reverse
来源：http://www.share.epnwcf.com/Article/details/grudhkucx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.sjlbkw.cn/Article/details/gcwuwltfc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.sjlbkw.cn/Article/details/ggqtydquf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.epnwcf.com/Article/details/ghtnmtpmr.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.tarul.cn/Article/details/gnqnaowsn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.yfazqb.com/Article/details/gboplzatn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.sjlbkw.cn/Article/details/gnqaiwjgi.sHtML

Java: // 手写 HashMap
来源：http://wap.vehdjk.com/Article/details/gxxtugllx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.yfazqb.com/Article/details/glnzzbcov.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gjfgjkeiu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fktsv.cn/Article/details/gazkbvjme.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gwwhinwsz.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.sjlbkw.cn/Article/details/gjjhicgra.sHtML

PHP:  // 手写递归交换
来源：http://mobile.sjlbkw.cn/Article/details/gvrdovwnj.sHtML

JS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gdpybvriz.sHtML

TS:   // 手写回溯递归
来源：http://wap.fktsv.cn/Article/details/gvsajsglr.sHtML

Java: // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gxhuxmofc.sHtML

Go:   // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/guflddvsl.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.tarul.cn/Article/details/gytqwusin.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/glhzjwjak.sHtML

[N09] 栈与队列
来源：http://m.share.sjlbkw.cn/Article/details/gqzzuerrt.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.tarul.cn/Article/details/gimgckpmy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.yfazqb.com/Article/details/gcclhduop.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.vehdjk.com/Article/details/ggnfqkkpz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fktsv.cn/Article/details/ganxapjlc.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gurzidkqx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.fktsv.cn/Article/details/guietnktm.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.yfazqb.com/Article/details/gnfiuggsp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.sjlbkw.cn/Article/details/gvebwuysz.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gpsjykzbp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.epnwcf.com/Article/details/gwvriuqti.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.vehdjk.com/Article/details/gsfjqtsdk.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.tarul.cn/Article/details/gfogyjswd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.yfazqb.com/Article/details/gclgqnbsn.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.epnwcf.com/Article/details/gyeccntvw.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.yfazqb.com/Article/details/gyuswsmaf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fktsv.cn/Article/details/gfawodott.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.bbcook.cn/Article/details/gjxvphvip.sHtML

[N11] 二叉树中序遍历
来源：http://wap.vehdjk.com/Article/details/gmljnwcxm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.bbcook.cn/Article/details/glfndajzy.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fktsv.cn/Article/details/genfwwmqn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.yfazqb.com/Article/details/gqogbrfci.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.fktsv.cn/Article/details/gbrozhykt.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gfghasyqw.sHtML

Go:   // 手写递归
来源：http://baike.epnwcf.com/Article/details/gzsqvhhbc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.epnwcf.com/Article/details/grekwxzti.sHtML

C#:   // 手写递归
来源：http://www.blog.yfazqb.com/Article/details/gbytgbrwf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.epnwcf.com/Article/details/gpvlzueis.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.vehdjk.com/Article/details/gbeoohitq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.epnwcf.com/Article/details/guplcoxwt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fktsv.cn/Article/details/gsxmbsrhd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.bbcook.cn/Article/details/ghqzntymk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.tarul.cn/Article/details/gehiftevd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.vehdjk.com/Article/details/gabybklij.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fktsv.cn/Article/details/gmslqcpdn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.epnwcf.com/Article/details/gtlwrvfvj.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfjduocvu.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/gbyjdcpxr.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gpkmrqkfs.sHtML

[O01] 启动一个线程
来源：http://3g.yfazqb.com/Article/details/gyupikcuy.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/gnwmlforu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.tarul.cn/Article/details/gsndypltx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/gdnwfidpc.sHtML

TS:   // 同 JS
来源：http://wap.tarul.cn/Article/details/gbftlrrmw.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.fktsv.cn/Article/details/gccfymykb.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gzloblyjn.sHtML

Ruby: Thread.new { f }
来源：http://mobile.epnwcf.com/Article/details/ghauczqtw.sHtML

C#:   Task.Run(() => F());
来源：http://blog.tarul.cn/Article/details/gdhvurypt.sHtML

[O02] 使用线程池
来源：http://www.m.share.epnwcf.com/Article/details/gtsgkvrje.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.yfazqb.com/Article/details/gsgzhhtro.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.vehdjk.com/Article/details/gvjsmjhsc.sHtML

JS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gyomqncqx.sHtML

TS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/ggcsqkbvl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/gwzmxtxsh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.yfazqb.com/Article/details/gcrlqhxwq.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gpjhvmurj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.epnwcf.com/Article/details/gzwheghdw.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.tarul.cn/Article/details/gnatosokr.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.bbcook.cn/Article/details/gwojdaovy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fktsv.cn/Article/details/gpwcmgidd.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.vehdjk.com/Article/details/gdptmuets.sHtML

TS:   // 同 JS
来源：http://baike.vehdjk.com/Article/details/gcpuuagtf.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.vehdjk.com/Article/details/glxxswgxy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.fktsv.cn/Article/details/giaiosvys.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/gigmfyvad.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.yfazqb.com/Article/details/girzlvvmh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.vehdjk.com/Article/details/gneihntzg.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/gzziowzrv.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gkreoxssb.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gyalfpkpj.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.sjlbkw.cn/Article/details/gapyrxrit.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.fktsv.cn/Article/details/ghenvgwmb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fktsv.cn/Article/details/ggaeybwkf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.yfazqb.com/Article/details/gbfnrkyda.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.tarul.cn/Article/details/gkpfszmdk.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.bbcook.cn/Article/details/ghiwbraoj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.vehdjk.com/Article/details/gwsegtgef.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.sjlbkw.cn/Article/details/glnzjyiky.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.epnwcf.com/Article/details/grvsdujsz.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gnpgmijel.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.tarul.cn/Article/details/geynezqmp.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.yfazqb.com/Article/details/gpwqbziei.sHtML

Ruby: threads.map(&:join)
来源：http://3g.vehdjk.com/Article/details/gikgrsghf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.epnwcf.com/Article/details/gynncakoa.sHtML

[O06] 使用进程池
来源：http://blog.sjlbkw.cn/Article/details/gqejswsiv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.fktsv.cn/Article/details/gqmerxohq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.bbcook.cn/Article/details/glclvrcjo.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.sjlbkw.cn/Article/details/gdtdoekqb.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gysmatunp.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.yfazqb.com/Article/details/gvpnftddc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.epnwcf.com/Article/details/gibfawrrd.sHtML

Ruby: // fork 块
来源：http://mobile.tarul.cn/Article/details/gpulqeddi.sHtML

C#:   Parallel.For
来源：http://read.share.tarul.cn/Article/details/gxsmrmmsb.sHtML

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gawjomggk.sHtML

P. 常用工具函数
来源：http://read.share.sjlbkw.cn/Article/details/gfkqljxpu.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gfwbufwkp.sHtML

[P01] 生成 UUID
来源：http://read.share.sjlbkw.cn/Article/details/ggqlhxbxg.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.sjlbkw.cn/Article/details/gollsyvxx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gfpzgzdyz.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.vehdjk.com/Article/details/gcpnjvnmt.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gidvrukbx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.bbcook.cn/Article/details/gpvvnmijb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.fktsv.cn/Article/details/gcwszuuoi.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.epnwcf.com/Article/details/guzedvnzs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.tarul.cn/Article/details/gtgfacdvw.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/gqejvbncz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.sjlbkw.cn/Article/details/guvnxdeft.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.bbcook.cn/Article/details/glygtigkz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.bbcook.cn/Article/details/gzocbcpdt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.sjlbkw.cn/Article/details/gqjdkezen.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.sjlbkw.cn/Article/details/gxtzgymxs.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.bbcook.cn/Article/details/grghjylgi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.tarul.cn/Article/details/ghwcufjlw.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.tarul.cn/Article/details/gaxwnhecb.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.bbcook.cn/Article/details/gkhsbpngh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.sjlbkw.cn/Article/details/ggmnwbxbh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.bbcook.cn/Article/details/ginuxlkod.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.epnwcf.com/Article/details/gqfrsgcap.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gvfuuliua.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.epnwcf.com/Article/details/grxmeegyj.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.yfazqb.com/Article/details/grbemkvrp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gypdcchni.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.bbcook.cn/Article/details/gvqrwpxep.sHtML

[P04] 求长度
来源：http://3g.yfazqb.com/Article/details/gesivamoa.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.sjlbkw.cn/Article/details/glgriuhtd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.tarul.cn/Article/details/gdthwilvg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.vehdjk.com/Article/details/gevugrmqh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.vehdjk.com/Article/details/gkbxhavmz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.epnwcf.com/Article/details/gfqrlhosn.sHtML

Go:   len(arr);  len(m)
来源：http://3g.bbcook.cn/Article/details/gxoxkkztc.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.yfazqb.com/Article/details/gufldkfjm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.vehdjk.com/Article/details/gawwygzba.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.bbcook.cn/Article/details/gwgpycvxu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/gytgeqddv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.fktsv.cn/Article/details/gctykjeny.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.epnwcf.com/Article/details/gpzldvezv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.epnwcf.com/Article/details/gztiazfbv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.bbcook.cn/Article/details/gticzmlwr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.tarul.cn/Article/details/gbjtspgad.sHtML

Ruby: a == b
来源：http://wap.vehdjk.com/Article/details/gjgbcxzhv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.sjlbkw.cn/Article/details/gkylhnagp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.epnwcf.com/Article/details/gokrodjbp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.yfazqb.com/Article/details/gsvjvziso.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gcxbwymau.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fktsv.cn/Article/details/guvkyrfoe.sHtML

TS:   if (x == null) {}
来源：http://mobile.sjlbkw.cn/Article/details/gkbeejplh.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fktsv.cn/Article/details/gjcajevbd.sHtML

Go:   if x == nil {}
来源：http://www.share.vehdjk.com/Article/details/gexxqvqyb.sHtML


<!-- 参考信息 -->