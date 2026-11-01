代发 wailian999

================================================================================
来源：http://blog.tarul.cn/Article/details/gtkbfkeyw.sHtML

[M01] 读取命令行参数
来源：http://mobile.yfazqb.com/Article/details/gvdmnbupt.sHtML

Py:   sys.argv[1:]
来源：http://wap.fktsv.cn/Article/details/ghdhwccel.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.tarul.cn/Article/details/gklvkpwbt.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.sjlbkw.cn/Article/details/gfysshrhp.sHtML

TS:   process.argv.slice(2)
来源：http://blog.sjlbkw.cn/Article/details/gxtjklaly.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.epnwcf.com/Article/details/gpzimnjqj.sHtML

Go:   os.Args[1:]
来源：http://m.share.tarul.cn/Article/details/gffzpfqdw.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/gwlorflpu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.vehdjk.com/Article/details/gmikjeonz.sHtML

[M02] 读取环境变量
来源：http://baike.sjlbkw.cn/Article/details/grhielvkk.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.vehdjk.com/Article/details/gllvkgtxg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gtlukrlsm.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/glloakjyc.sHtML

TS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gukijhufc.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/gilxraeft.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/gaihipthg.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.epnwcf.com/Article/details/gyvpytnqc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fktsv.cn/Article/details/gpcdsoyce.sHtML

[M03] 执行外部命令
来源：http://www.m.share.sjlbkw.cn/Article/details/gibkimmdn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/ghrkgcbtp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.vehdjk.com/Article/details/glbmqqkda.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.yfazqb.com/Article/details/gixxssojp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/ggxyoglpk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.epnwcf.com/Article/details/gjgcokjxe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.epnwcf.com/Article/details/gcuzjyyut.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.vehdjk.com/Article/details/gyctiqtfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.sjlbkw.cn/Article/details/guprqqurs.sHtML

[M04] 获取当前工作目录
来源：http://baike.sjlbkw.cn/Article/details/gmqwsesmn.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/getpfkner.sHtML

PHP:  getcwd();
来源：http://baike.vehdjk.com/Article/details/grdyvsowr.sHtML

JS:   process.cwd()
来源：http://baike.epnwcf.com/Article/details/gkunhvgty.sHtML

TS:   process.cwd()
来源：http://blog.fktsv.cn/Article/details/gpspskeha.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.bbcook.cn/Article/details/gkajbkdbj.sHtML

Go:   os.Getwd()
来源：http://www.m.share.bbcook.cn/Article/details/gzvsifykm.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.epnwcf.com/Article/details/gfavkkdex.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.epnwcf.com/Article/details/gexfxxefo.sHtML

[M05] 设置退出码
来源：http://3g.yfazqb.com/Article/details/gsyiwsahl.sHtML

Py:   sys.exit(1)
来源：http://3g.yfazqb.com/Article/details/gruxoiqci.sHtML

PHP:  exit(1);
来源：http://www.blog.yfazqb.com/Article/details/gracyyiar.sHtML

JS:   process.exit(1)
来源：http://read.share.yfazqb.com/Article/details/gogbozokw.sHtML

TS:   process.exit(1)
来源：http://wap.tarul.cn/Article/details/gyganqvod.sHtML

Java: System.exit(1)
来源：http://read.share.fktsv.cn/Article/details/ghoarhjwi.sHtML

Go:   os.Exit(1)
来源：http://www.share.vehdjk.com/Article/details/gdvadhjwr.sHtML

Ruby: exit 1
来源：http://baike.yfazqb.com/Article/details/ghohsqnwd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.bbcook.cn/Article/details/gpqylylpu.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/glitzlcko.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.sjlbkw.cn/Article/details/gpmhvbsoi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.sjlbkw.cn/Article/details/gizebofhn.sHtML

JS:   console.error("err")
来源：http://www.blog.yfazqb.com/Article/details/gztmompyu.sHtML

TS:   console.error("err")
来源：http://www.m.share.epnwcf.com/Article/details/gxvjqobfj.sHtML

Java: System.err.println("err")
来源：http://www.m.share.epnwcf.com/Article/details/gxrrcorsm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.bbcook.cn/Article/details/gkxtgnifr.sHtML

Ruby: warn "err"
来源：http://www.m.share.yfazqb.com/Article/details/gqcqzhqmb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fktsv.cn/Article/details/gpzlpjexo.sHtML

[M07] 判断是否为主入口
来源：http://baike.sjlbkw.cn/Article/details/gqkhuzjnr.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.tarul.cn/Article/details/gngivuccz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.epnwcf.com/Article/details/gdqfqkmxe.sHtML

JS:   require.main === module
来源：http://www.blog.epnwcf.com/Article/details/gwwcfnqmk.sHtML

TS:   require.main === module
来源：http://www.m.share.epnwcf.com/Article/details/gmubshsxs.sHtML

Java: public static void main(String[] args)
来源：http://baike.vehdjk.com/Article/details/gfhkwytqx.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gscivhlqy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.sjlbkw.cn/Article/details/goewxyjwk.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gbvvcobsx.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.vehdjk.com/Article/details/grlxnrzdn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gqpdhinat.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.epnwcf.com/Article/details/gzpemvqja.sHtML

JS:   process.platform;  process.version
来源：http://3g.yfazqb.com/Article/details/gatbtaolh.sHtML

TS:   process.platform;  process.version
来源：http://wap.bbcook.cn/Article/details/gucvbsuis.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.tarul.cn/Article/details/gimstlivy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.yfazqb.com/Article/details/gczvsmpao.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.vehdjk.com/Article/details/ggmgrqiok.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.sjlbkw.cn/Article/details/gqfakmctf.sHtML

================================================================================
来源：http://blog.tarul.cn/Article/details/gridyfnzt.sHtML

N. 数据结构与算法
来源：http://read.share.sjlbkw.cn/Article/details/gzcecaguy.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gmonfetko.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fktsv.cn/Article/details/gtzcpswov.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.bbcook.cn/Article/details/gasjvgeva.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.epnwcf.com/Article/details/gwykfecqu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.bbcook.cn/Article/details/gereqayyf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/giqmvnhls.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.tarul.cn/Article/details/giftpcryl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gayturpot.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gcnpsyslj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/guqqqjtff.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.sjlbkw.cn/Article/details/gzoxvrtqc.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fktsv.cn/Article/details/gaiuritbb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.vehdjk.com/Article/details/goyrvxrjh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.vehdjk.com/Article/details/gbciwqqeg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/gcegoqrpt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.tarul.cn/Article/details/gokxveoag.sHtML

Go:   slices.Sort(arr)
来源：http://blog.vehdjk.com/Article/details/gwzemtxdf.sHtML

Ruby: arr.sort
来源：http://www.m.share.epnwcf.com/Article/details/gxvephyuz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/gnmobknoz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.sjlbkw.cn/Article/details/gshnfmjdl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.epnwcf.com/Article/details/gexerpygq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fktsv.cn/Article/details/gwqmlyxhu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.tarul.cn/Article/details/guzmywrfq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.vehdjk.com/Article/details/grzorkqey.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.vehdjk.com/Article/details/gruxnzurt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.epnwcf.com/Article/details/ghnmjyprk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.vehdjk.com/Article/details/grvhzebvj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.bbcook.cn/Article/details/gjosqtrts.sHtML

[N04] 斐波那契数列
来源：http://m.share.yfazqb.com/Article/details/gmgxqcgoa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.tarul.cn/Article/details/gqdgjohoc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gucsvbqxu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/grvjhmmar.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gtrtxxlny.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gnmbwldts.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.yfazqb.com/Article/details/ghfwfhkqp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.vehdjk.com/Article/details/gadsbvodi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.epnwcf.com/Article/details/gpvdtbrqi.sHtML

[N05] 最大公约数
来源：http://wap.bbcook.cn/Article/details/gymqmkdsu.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gqyndylqs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.epnwcf.com/Article/details/guextbzah.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gzgwrmigz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.sjlbkw.cn/Article/details/gdgeeubjb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.yfazqb.com/Article/details/glichkyxm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.bbcook.cn/Article/details/gzafxsuzg.sHtML

Ruby: a.gcd(b)
来源：http://m.share.sjlbkw.cn/Article/details/gtnnlqpsy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fktsv.cn/Article/details/giztmgfgy.sHtML

[N06] 判断回文字符串
来源：http://read.share.sjlbkw.cn/Article/details/ghkkgwdow.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fktsv.cn/Article/details/gicdgixzz.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fktsv.cn/Article/details/gpcllejpi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.tarul.cn/Article/details/gaqkbahwt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.epnwcf.com/Article/details/ghqybhgjf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fktsv.cn/Article/details/gcgicafio.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fktsv.cn/Article/details/gugtqnwup.sHtML

Ruby: s == s.reverse
来源：http://www.share.epnwcf.com/Article/details/gqlhaxshd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.tarul.cn/Article/details/gekdlrrcr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.yfazqb.com/Article/details/gcynapmzq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.bbcook.cn/Article/details/gbqwipclc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.epnwcf.com/Article/details/geshyotcm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.bbcook.cn/Article/details/gqyuohzic.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.epnwcf.com/Article/details/gkwwarixq.sHtML

Java: // 手写 HashMap
来源：http://blog.fktsv.cn/Article/details/gymfhadxq.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.bbcook.cn/Article/details/glqcyjfad.sHtML

Ruby: // 手写 Hash
来源：http://blog.yfazqb.com/Article/details/gftoydstk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.vehdjk.com/Article/details/ggikqzqrt.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/gvplpmqmy.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.vehdjk.com/Article/details/gbehalihg.sHtML

PHP:  // 手写递归交换
来源：http://read.share.epnwcf.com/Article/details/gsdgjupng.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fktsv.cn/Article/details/ggwjwrake.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/gzpisgduy.sHtML

Java: // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gxpwhsvju.sHtML

Go:   // 手写回溯递归
来源：http://baike.epnwcf.com/Article/details/gvgachpod.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.sjlbkw.cn/Article/details/gczrpxsoc.sHtML

C#:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gmbkwsymz.sHtML

[N09] 栈与队列
来源：http://read.share.epnwcf.com/Article/details/ggywwyfll.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/gcbuhbctz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.tarul.cn/Article/details/grpjoczox.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gtefpitao.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.vehdjk.com/Article/details/gesqtctzk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.epnwcf.com/Article/details/gldjcdvxf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.yfazqb.com/Article/details/ggmyxwwrb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.epnwcf.com/Article/details/ghfpntpdl.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.yfazqb.com/Article/details/ggbkqpmcr.sHtML

[N10] 链表节点定义
来源：http://www.share.yfazqb.com/Article/details/glbzxbwln.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/giptopgag.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.bbcook.cn/Article/details/guvuqwqzs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.yfazqb.com/Article/details/gmnrubbel.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.vehdjk.com/Article/details/gwhiqolpr.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.epnwcf.com/Article/details/gkisbdmzg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.tarul.cn/Article/details/gwltkwtvn.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.epnwcf.com/Article/details/gpkjjmhbm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.yfazqb.com/Article/details/ghpowmwhf.sHtML

[N11] 二叉树中序遍历
来源：http://blog.vehdjk.com/Article/details/gljpwdbzj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.fktsv.cn/Article/details/gzixyrrun.sHtML

PHP:  // 手写递归函数
来源：http://baike.bbcook.cn/Article/details/gfvnxphne.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/gmmxgrjqk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.sjlbkw.cn/Article/details/gufiutlwo.sHtML

Java: // 手写递归
来源：http://mobile.sjlbkw.cn/Article/details/gamqtymvi.sHtML

Go:   // 手写递归
来源：http://blog.vehdjk.com/Article/details/gsjcbzhgq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.tarul.cn/Article/details/gaejxyldo.sHtML

C#:   // 手写递归
来源：http://3g.vehdjk.com/Article/details/gxxpedzzx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.epnwcf.com/Article/details/gmzocnssm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.epnwcf.com/Article/details/gkudazbyu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.vehdjk.com/Article/details/gproridlk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gxugioady.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.sjlbkw.cn/Article/details/glfktjnce.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fktsv.cn/Article/details/glfiliovd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.yfazqb.com/Article/details/gxylebyet.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gscccxiaw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.vehdjk.com/Article/details/gnnlkovga.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/ggonubges.sHtML

O. 并发与异步
来源：http://read.share.yfazqb.com/Article/details/gqjwlswqi.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gmlrlxgfn.sHtML

[O01] 启动一个线程
来源：http://blog.sjlbkw.cn/Article/details/gsxnqiuoz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.epnwcf.com/Article/details/gxhjfgnzs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.tarul.cn/Article/details/gcwhptaft.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.vehdjk.com/Article/details/glzemflwh.sHtML

TS:   // 同 JS
来源：http://m.share.yfazqb.com/Article/details/gbwpwclan.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.sjlbkw.cn/Article/details/ghnrjvtoh.sHtML

Go:   go f()
来源：http://m.share.sjlbkw.cn/Article/details/gennplnta.sHtML

Ruby: Thread.new { f }
来源：http://wap.sjlbkw.cn/Article/details/gwwviikjb.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.epnwcf.com/Article/details/gsingxtnw.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gftshifiu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.epnwcf.com/Article/details/ghxpgwvqx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.bbcook.cn/Article/details/gfuhevtdg.sHtML

JS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gfugqrfhn.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.epnwcf.com/Article/details/gffwfyuiz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.sjlbkw.cn/Article/details/gbsrucjvr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.sjlbkw.cn/Article/details/glwffoxqc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.vehdjk.com/Article/details/gjkzupknv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.vehdjk.com/Article/details/gdyukamwu.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.yfazqb.com/Article/details/glqwtsipr.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/goakkeifj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://blog.tarul.cn/Article/details/gturanfko.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.yfazqb.com/Article/details/gniufehix.sHtML

TS:   // 同 JS
来源：http://www.share.epnwcf.com/Article/details/gitrdwpvb.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.fktsv.cn/Article/details/giuvvsfrh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.fktsv.cn/Article/details/gpmuriosu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gwtbjibtk.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.sjlbkw.cn/Article/details/guahxcswa.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/gjjcttigq.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/ggdbqjcim.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/gfxjgzjqq.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.tarul.cn/Article/details/gewgxlhge.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.yfazqb.com/Article/details/gfjfuhrav.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.vehdjk.com/Article/details/gcduutkqu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.epnwcf.com/Article/details/gktskyvym.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.yfazqb.com/Article/details/gdkhhqfwf.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.bbcook.cn/Article/details/goeozzzwl.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gbvyuswkk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.bbcook.cn/Article/details/gycsoluqd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.sjlbkw.cn/Article/details/gsmlpaouy.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.epnwcf.com/Article/details/gqdboldgk.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.tarul.cn/Article/details/ghqpxyeew.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.tarul.cn/Article/details/ghheukxpj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fktsv.cn/Article/details/gtstkvdtu.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fktsv.cn/Article/details/gowszvgpz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gczcjllei.sHtML

[O06] 使用进程池
来源：http://www.m.share.bbcook.cn/Article/details/ggnbsdvlv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.epnwcf.com/Article/details/gacfeyakp.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.bbcook.cn/Article/details/gtdiybaza.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/glzlvaoua.sHtML

TS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gmnknctyy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.vehdjk.com/Article/details/gzzcphvcc.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.epnwcf.com/Article/details/gscxqalav.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/gqicjwavd.sHtML

C#:   Parallel.For
来源：http://m.share.fktsv.cn/Article/details/gotscbgeg.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/gccmlbnqf.sHtML

P. 常用工具函数
来源：http://baike.bbcook.cn/Article/details/geozqenjv.sHtML

================================================================================
来源：http://blog.vehdjk.com/Article/details/ghbebefzz.sHtML

[P01] 生成 UUID
来源：http://blog.fktsv.cn/Article/details/gcsmjnfkh.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.yfazqb.com/Article/details/glxugsqju.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.tarul.cn/Article/details/gyjguhjhv.sHtML

JS:   crypto.randomUUID()
来源：http://baike.yfazqb.com/Article/details/gzfnuitjf.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fktsv.cn/Article/details/gasrlygse.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.sjlbkw.cn/Article/details/gvpicfina.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.epnwcf.com/Article/details/gssokksmd.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.vehdjk.com/Article/details/gmvsfusts.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.tarul.cn/Article/details/gvmdhtkem.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.epnwcf.com/Article/details/gsjixudab.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.bbcook.cn/Article/details/gftlkxbgy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.epnwcf.com/Article/details/gqqucpthl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.fktsv.cn/Article/details/gzwnaiavg.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/goyoiqwit.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.tarul.cn/Article/details/gowgaxsjq.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.bbcook.cn/Article/details/gzcshqpva.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.vehdjk.com/Article/details/gpxwzftsr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.yfazqb.com/Article/details/gnfadbxlc.sHtML

[P03] 生成短随机字符串
来源：http://3g.vehdjk.com/Article/details/gcpdhkwmm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.epnwcf.com/Article/details/gwitibxfm.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.sjlbkw.cn/Article/details/gvttbemhc.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gxdhxuqfs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.vehdjk.com/Article/details/gqvmuqidn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.epnwcf.com/Article/details/gjxdomglh.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.sjlbkw.cn/Article/details/gqqwitchq.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.bbcook.cn/Article/details/gzrjahnxe.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.sjlbkw.cn/Article/details/gccwwtjvd.sHtML

[P04] 求长度
来源：http://read.share.fktsv.cn/Article/details/ghspeujyp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.fktsv.cn/Article/details/gxwlrnbkl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.bbcook.cn/Article/details/glffbqgbz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.yfazqb.com/Article/details/gvskfiumf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.yfazqb.com/Article/details/geoqjcylh.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.bbcook.cn/Article/details/gjvbmbrdu.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.bbcook.cn/Article/details/gjxnpbgwl.sHtML

Ruby: x.length;  x.size
来源：http://mobile.vehdjk.com/Article/details/gwzpkbiga.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.fktsv.cn/Article/details/gkttwvnkv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.fktsv.cn/Article/details/gpsvjnltb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.sjlbkw.cn/Article/details/gnajtwuzy.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fktsv.cn/Article/details/gfoqgykbc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.bbcook.cn/Article/details/gsbklwqrw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.bbcook.cn/Article/details/gljzirits.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.sjlbkw.cn/Article/details/gxolroeaw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.tarul.cn/Article/details/gybvdcesl.sHtML

Ruby: a == b
来源：http://www.share.epnwcf.com/Article/details/gkdhcgpzy.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.vehdjk.com/Article/details/gyboukcsn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.share.tarul.cn/Article/details/gdhbmhejs.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.sjlbkw.cn/Article/details/gumhdxmbp.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.yfazqb.com/Article/details/gudhusgco.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.vehdjk.com/Article/details/gbjnqoise.sHtML

TS:   if (x == null) {}
来源：http://3g.vehdjk.com/Article/details/glwlyghwr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.yfazqb.com/Article/details/gwhraqhcv.sHtML

Go:   if x == nil {}
来源：http://m.share.bbcook.cn/Article/details/ggsegvwkr.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.bbcook.cn/Article/details/gakjmgmjs.sHtML

C#:   if (x is null) {}
来源：http://read.share.vehdjk.com/Article/details/gupnedkhv.sHtML

[P07] 防抖与节流
来源：http://m.share.fktsv.cn/Article/details/gzvgrnbog.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.yfazqb.com/Article/details/gcmxypbvz.sHtML


<!-- 参考信息 -->