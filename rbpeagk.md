代发 wailian999

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzuulomrz.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.epnwcf.com/Article/details/gzlzihcea.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fktsv.cn/Article/details/ggrphojve.sHtML

PHP:  $argv;  $argc;
来源：http://blog.bbcook.cn/Article/details/gvwfnzoaf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.tarul.cn/Article/details/gcvypmvad.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fktsv.cn/Article/details/gdgjublfc.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.sjlbkw.cn/Article/details/gfgvzohju.sHtML

Go:   os.Args[1:]
来源：http://wap.bbcook.cn/Article/details/gmsimajsr.sHtML

Ruby: ARGV
来源：http://read.share.epnwcf.com/Article/details/gsszrhhed.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/givfynbgz.sHtML

[M02] 读取环境变量
来源：http://wap.yfazqb.com/Article/details/gxqajmkhi.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.bbcook.cn/Article/details/ggvusdoth.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.bbcook.cn/Article/details/glwpbwluz.sHtML

JS:   process.env.HOME
来源：http://3g.epnwcf.com/Article/details/gxqdputfw.sHtML

TS:   process.env.HOME
来源：http://www.share.fktsv.cn/Article/details/gqyrrqjvw.sHtML

Java: System.getenv("HOME")
来源：http://blog.fktsv.cn/Article/details/gbjatztou.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.yfazqb.com/Article/details/gvvuvzvvd.sHtML

Ruby: ENV["HOME"]
来源：http://baike.bbcook.cn/Article/details/gxnagovim.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.tarul.cn/Article/details/gqkwhfjhg.sHtML

[M03] 执行外部命令
来源：http://m.share.bbcook.cn/Article/details/goqwuohro.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.tarul.cn/Article/details/glhughbwq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fktsv.cn/Article/details/gbghqklqq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gzjnizswq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.sjlbkw.cn/Article/details/graquwssc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.sjlbkw.cn/Article/details/gwgryczcq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.vehdjk.com/Article/details/ghmiofrae.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fktsv.cn/Article/details/gcxdwcqbq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.sjlbkw.cn/Article/details/ggcwonrkm.sHtML

[M04] 获取当前工作目录
来源：http://read.share.yfazqb.com/Article/details/gellfuepv.sHtML

Py:   os.getcwd()
来源：http://m.share.fktsv.cn/Article/details/gogagmfis.sHtML

PHP:  getcwd();
来源：http://baike.sjlbkw.cn/Article/details/ghfwxxmgt.sHtML

JS:   process.cwd()
来源：http://read.share.sjlbkw.cn/Article/details/gyzrclimw.sHtML

TS:   process.cwd()
来源：http://read.share.epnwcf.com/Article/details/grdsdxzkv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.vehdjk.com/Article/details/gzpkaoges.sHtML

Go:   os.Getwd()
来源：http://www.share.bbcook.cn/Article/details/geofmlkjq.sHtML

Ruby: Dir.pwd
来源：http://m.share.yfazqb.com/Article/details/gbquikefi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.vehdjk.com/Article/details/gmhkawrkx.sHtML

[M05] 设置退出码
来源：http://www.blog.bbcook.cn/Article/details/gstyuaehh.sHtML

Py:   sys.exit(1)
来源：http://mobile.yfazqb.com/Article/details/gglbmmdno.sHtML

PHP:  exit(1);
来源：http://blog.sjlbkw.cn/Article/details/geddhgent.sHtML

JS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/goxnjkrgm.sHtML

TS:   process.exit(1)
来源：http://blog.tarul.cn/Article/details/gmdpkoubj.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gdzfvcwfa.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gdzytkxsf.sHtML

Ruby: exit 1
来源：http://m.share.yfazqb.com/Article/details/gbcfbotkf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.tarul.cn/Article/details/gtfzxnocu.sHtML

[M06] 向标准错误输出
来源：http://blog.sjlbkw.cn/Article/details/gscuvyaxg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.yfazqb.com/Article/details/gxznnivml.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fktsv.cn/Article/details/gkhurxvtv.sHtML

JS:   console.error("err")
来源：http://www.share.tarul.cn/Article/details/gxkqkpfvr.sHtML

TS:   console.error("err")
来源：http://baike.tarul.cn/Article/details/gwjuzrbcl.sHtML

Java: System.err.println("err")
来源：http://blog.bbcook.cn/Article/details/gbrtfeyql.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fktsv.cn/Article/details/ghdfrngka.sHtML

Ruby: warn "err"
来源：http://mobile.tarul.cn/Article/details/gejxprucr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fktsv.cn/Article/details/gfczvditg.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gqabqnqeb.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.vehdjk.com/Article/details/gexpeklzk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.sjlbkw.cn/Article/details/gcjlzligm.sHtML

JS:   require.main === module
来源：http://www.blog.vehdjk.com/Article/details/gteckonlr.sHtML

TS:   require.main === module
来源：http://m.share.vehdjk.com/Article/details/ggkriyqhc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.bbcook.cn/Article/details/ghabrvgye.sHtML

Go:   func main()
来源：http://read.share.sjlbkw.cn/Article/details/gmarwpgxx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.epnwcf.com/Article/details/gipcfkayx.sHtML

C#:   static void Main(string[] args)
来源：http://wap.epnwcf.com/Article/details/glplupsdo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.sjlbkw.cn/Article/details/gfuiyeyrt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.tarul.cn/Article/details/gbkitisqs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.tarul.cn/Article/details/gxatjthya.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gfdkxaeax.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fktsv.cn/Article/details/gcjacnmpu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fktsv.cn/Article/details/giguzmhzx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gazwvupdm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/glcdenler.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.epnwcf.com/Article/details/gnfiodhzj.sHtML

================================================================================
来源：http://www.m.share.vehdjk.com/Article/details/gsryamrkf.sHtML

N. 数据结构与算法
来源：http://m.share.bbcook.cn/Article/details/gcbatjkus.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gbmkeqmwt.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/ghlfqanci.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.epnwcf.com/Article/details/gwhhgeeuy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.tarul.cn/Article/details/gdhgduqmh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gjfutdaov.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/ggnshlelv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.vehdjk.com/Article/details/gikomsrhz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.epnwcf.com/Article/details/gxwomkkik.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.vehdjk.com/Article/details/gyajeeohy.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gmzyfqebw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fktsv.cn/Article/details/gacqpzwrh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.bbcook.cn/Article/details/gwdcturaz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.tarul.cn/Article/details/giwzrpdkn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.yfazqb.com/Article/details/gnzqvvkau.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fktsv.cn/Article/details/glzprwrzu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.sjlbkw.cn/Article/details/gxedqwybu.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.vehdjk.com/Article/details/gqgfsbkwd.sHtML

Ruby: arr.sort
来源：http://read.share.sjlbkw.cn/Article/details/gjycinlis.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.bbcook.cn/Article/details/gkozidjka.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.yfazqb.com/Article/details/gwmzpzidq.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fktsv.cn/Article/details/glavrgezr.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.vehdjk.com/Article/details/glfnqysdv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.yfazqb.com/Article/details/gtapgznxi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.vehdjk.com/Article/details/gglbunvdz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.bbcook.cn/Article/details/ganmmvkup.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.vehdjk.com/Article/details/gyqewwmir.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gaskhlhxj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.vehdjk.com/Article/details/gpwepgkhg.sHtML

[N04] 斐波那契数列
来源：http://read.share.epnwcf.com/Article/details/gjducqlfk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.sjlbkw.cn/Article/details/gymqneqqc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.epnwcf.com/Article/details/gcvcrzcvi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.bbcook.cn/Article/details/gsmgzjsjw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.yfazqb.com/Article/details/gjgjlkwsz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fktsv.cn/Article/details/gtlfswjrl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.bbcook.cn/Article/details/grpygfabw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.tarul.cn/Article/details/guaxgfpnq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gcttztckx.sHtML

[N05] 最大公约数
来源：http://m.share.yfazqb.com/Article/details/gblzwdlpc.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fktsv.cn/Article/details/gmoisrcyn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.tarul.cn/Article/details/gtrnkyqxv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gfcfkmmmw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.bbcook.cn/Article/details/gzluuponp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.yfazqb.com/Article/details/gpclmgmjm.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.vehdjk.com/Article/details/ggnqmoxxx.sHtML

Ruby: a.gcd(b)
来源：http://read.share.yfazqb.com/Article/details/gvhayqaeo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.tarul.cn/Article/details/galmskxog.sHtML

[N06] 判断回文字符串
来源：http://blog.epnwcf.com/Article/details/gviuwgdfh.sHtML

Py:   s == s[::-1]
来源：http://wap.fktsv.cn/Article/details/gtmzfmxnv.sHtML

PHP:  $s === strrev($s);
来源：http://blog.bbcook.cn/Article/details/ggckzugov.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.sjlbkw.cn/Article/details/gxwdmzjcj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gkvvvxrek.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fktsv.cn/Article/details/gofpnmavn.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fktsv.cn/Article/details/gopxtkdmd.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gzuwiylfh.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.yfazqb.com/Article/details/gnouajqlc.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.bbcook.cn/Article/details/gfqmjpvyi.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gnodovbmk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.epnwcf.com/Article/details/gctfrvbsv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.epnwcf.com/Article/details/gbnhgsiop.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.yfazqb.com/Article/details/gxoublahk.sHtML

Java: // 手写 HashMap
来源：http://www.share.yfazqb.com/Article/details/gyglltxqy.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.tarul.cn/Article/details/gakiumaib.sHtML

Ruby: // 手写 Hash
来源：http://3g.vehdjk.com/Article/details/gdhnohhvu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.tarul.cn/Article/details/glsirmvrn.sHtML

[N08] 生成全排列
来源：http://www.blog.vehdjk.com/Article/details/gslesmbkx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.epnwcf.com/Article/details/gfmyhfema.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.sjlbkw.cn/Article/details/glpfuxtzw.sHtML

JS:   // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gwtynsbkm.sHtML

TS:   // 手写回溯递归
来源：http://3g.yfazqb.com/Article/details/grisxbhsh.sHtML

Java: // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gkdkzuivq.sHtML

Go:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gbinepczt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.sjlbkw.cn/Article/details/gsnoejmvu.sHtML

C#:   // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/gxjmgdmmx.sHtML

[N09] 栈与队列
来源：http://www.m.share.tarul.cn/Article/details/gvfomuknu.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.tarul.cn/Article/details/gwxebbfmd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/geqgrughh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gwrndbrwj.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.vehdjk.com/Article/details/gtvlsjtyl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.sjlbkw.cn/Article/details/giscluadq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.tarul.cn/Article/details/ginzvxcgi.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gbbymknuf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.tarul.cn/Article/details/gfemngsai.sHtML

[N10] 链表节点定义
来源：http://3g.yfazqb.com/Article/details/glnqwrcqt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.epnwcf.com/Article/details/gixucfnvj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gewdttljo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.tarul.cn/Article/details/gvvyyapkc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gzcgpnqfq.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gdlelnlve.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.epnwcf.com/Article/details/gximkrrzm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.epnwcf.com/Article/details/gitlpmywu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.vehdjk.com/Article/details/gnvttcbij.sHtML

[N11] 二叉树中序遍历
来源：http://blog.tarul.cn/Article/details/glezafrlf.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.vehdjk.com/Article/details/gdazucanj.sHtML

PHP:  // 手写递归函数
来源：http://wap.bbcook.cn/Article/details/gymjkqhgu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fktsv.cn/Article/details/gjhhiuxzu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gantjgsoc.sHtML

Java: // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gyqzzlfom.sHtML

Go:   // 手写递归
来源：http://mobile.tarul.cn/Article/details/gyubbnjdc.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/gnyyrciqz.sHtML

C#:   // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gtupkjfxm.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.epnwcf.com/Article/details/gisxgfdjm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.epnwcf.com/Article/details/gnekcydnf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.tarul.cn/Article/details/gudiywttv.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.vehdjk.com/Article/details/gklzeswwy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.bbcook.cn/Article/details/gaxjcqlgn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gohivfwvf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.epnwcf.com/Article/details/gmbhawezz.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.bbcook.cn/Article/details/gsbfpuptv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gxzqryuif.sHtML

================================================================================
来源：http://read.share.vehdjk.com/Article/details/gdfqaedtp.sHtML

O. 并发与异步
来源：http://mobile.fktsv.cn/Article/details/geruwvsyg.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/grrdanmnz.sHtML

[O01] 启动一个线程
来源：http://m.share.epnwcf.com/Article/details/grvqtygjn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fktsv.cn/Article/details/gmqpaqzze.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gqgknwcfu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.tarul.cn/Article/details/goyhklotz.sHtML

TS:   // 同 JS
来源：http://blog.epnwcf.com/Article/details/gnfkdfxps.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.yfazqb.com/Article/details/gykhfhdbf.sHtML

Go:   go f()
来源：http://www.share.fktsv.cn/Article/details/gwlbpdvkx.sHtML

Ruby: Thread.new { f }
来源：http://blog.epnwcf.com/Article/details/ginlvrpvp.sHtML

C#:   Task.Run(() => F());
来源：http://blog.sjlbkw.cn/Article/details/gpwdlhuhd.sHtML

[O02] 使用线程池
来源：http://3g.sjlbkw.cn/Article/details/gcqmxxsqq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/gyfmuhjda.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.bbcook.cn/Article/details/gsdezvqzt.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.vehdjk.com/Article/details/gcuuymgra.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.tarul.cn/Article/details/gonmycebc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.vehdjk.com/Article/details/grsxscyxa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.bbcook.cn/Article/details/grzeclgcs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.bbcook.cn/Article/details/gpsftcxvt.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.epnwcf.com/Article/details/ggmrxjdfq.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.yfazqb.com/Article/details/gsmvlujsx.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.bbcook.cn/Article/details/gthavycxf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.epnwcf.com/Article/details/gmvxfxhry.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.epnwcf.com/Article/details/gmuelwvvb.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/gjmehodri.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.bbcook.cn/Article/details/girmnzwyz.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/geiyxxjad.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.yfazqb.com/Article/details/gqnhkpbdl.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.vehdjk.com/Article/details/gxmenrcvr.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gdprkawsw.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fktsv.cn/Article/details/gplzpazzd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.tarul.cn/Article/details/goouhqeea.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.bbcook.cn/Article/details/gbqtrhnag.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fktsv.cn/Article/details/gipsiwita.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fktsv.cn/Article/details/godmvhkfe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.sjlbkw.cn/Article/details/gsacqwtpo.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.bbcook.cn/Article/details/gdmsoskjs.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/griomdnlq.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.fktsv.cn/Article/details/gcfpmhdeq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.yfazqb.com/Article/details/gjnamcnjo.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.epnwcf.com/Article/details/grouhqxdj.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.vehdjk.com/Article/details/gvidqejsb.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.sjlbkw.cn/Article/details/gbcfittzx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.yfazqb.com/Article/details/grvbomnco.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.sjlbkw.cn/Article/details/gmteuxjgj.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fktsv.cn/Article/details/gootvxjxu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.vehdjk.com/Article/details/gsxpgacsr.sHtML

[O06] 使用进程池
来源：http://www.share.yfazqb.com/Article/details/grfepqnow.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.vehdjk.com/Article/details/gedlrfpeg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.tarul.cn/Article/details/gtsizmzxh.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gbpjxyegp.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.tarul.cn/Article/details/guspxfmdz.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.tarul.cn/Article/details/gxhmblteo.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fktsv.cn/Article/details/gpymhjklq.sHtML

Ruby: // fork 块
来源：http://read.share.epnwcf.com/Article/details/goqilgkhq.sHtML

C#:   Parallel.For
来源：http://www.share.epnwcf.com/Article/details/gavyawelv.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gfyceupir.sHtML

P. 常用工具函数
来源：http://www.blog.epnwcf.com/Article/details/gkmyursjj.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/grcrqwidu.sHtML

[P01] 生成 UUID
来源：http://read.share.yfazqb.com/Article/details/gvysxtrtp.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.bbcook.cn/Article/details/grviouidd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.vehdjk.com/Article/details/gbcuxtoau.sHtML

JS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/gotrcpkwj.sHtML

TS:   crypto.randomUUID()
来源：http://blog.vehdjk.com/Article/details/ghyfwfvfu.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gdisvqjey.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/gauciwnju.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.sjlbkw.cn/Article/details/gxofjaxar.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.bbcook.cn/Article/details/gwmtxgdue.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fktsv.cn/Article/details/gslzgrlvm.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.tarul.cn/Article/details/gnvndryqb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.vehdjk.com/Article/details/grgmsulfl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.epnwcf.com/Article/details/gfmrwyivw.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/gdsydidkg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.bbcook.cn/Article/details/gjslszjho.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.sjlbkw.cn/Article/details/gptdybsrs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.epnwcf.com/Article/details/gjwaxayoi.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.fktsv.cn/Article/details/gqmxaqmki.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.bbcook.cn/Article/details/gktwmjsse.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/gwqisppjj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gykkncgtr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gbzryqhet.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fktsv.cn/Article/details/glowdkajv.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.tarul.cn/Article/details/gytvbadjz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.bbcook.cn/Article/details/gkcqjkemb.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.sjlbkw.cn/Article/details/grispshrd.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.bbcook.cn/Article/details/gdpkeaizy.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gflykrvcu.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.sjlbkw.cn/Article/details/gmbzatkrm.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.tarul.cn/Article/details/geaenysln.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.bbcook.cn/Article/details/gijznhptk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.bbcook.cn/Article/details/ghhvklhth.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.bbcook.cn/Article/details/gsqtyizxe.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.epnwcf.com/Article/details/gygffmitc.sHtML

Ruby: x.length;  x.size
来源：http://baike.sjlbkw.cn/Article/details/gsehgknmj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.sjlbkw.cn/Article/details/gjwdtceek.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.sjlbkw.cn/Article/details/gwneolpxy.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.epnwcf.com/Article/details/gdlvolxlv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.vehdjk.com/Article/details/gekjgtukn.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.bbcook.cn/Article/details/gwqlfkbei.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.epnwcf.com/Article/details/gvsifqblx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.tarul.cn/Article/details/grotjtfhh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://blog.bbcook.cn/Article/details/gesmsskjr.sHtML

Ruby: a == b
来源：http://blog.fktsv.cn/Article/details/gaatjejqh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gvcvuciql.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.tarul.cn/Article/details/giqmbvxpl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.fktsv.cn/Article/details/grvglaelg.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.vehdjk.com/Article/details/gqbbilqtu.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.tarul.cn/Article/details/gvgvsmuwi.sHtML

TS:   if (x == null) {}
来源：http://m.share.sjlbkw.cn/Article/details/ggyqyyirg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.yfazqb.com/Article/details/ggmmtsmxy.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/ghqhsejtj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fktsv.cn/Article/details/ghojvgyiu.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.vehdjk.com/Article/details/grqzxeatq.sHtML

[P07] 防抖与节流
来源：http://www.blog.sjlbkw.cn/Article/details/grbudedbb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.tarul.cn/Article/details/gfpowtykm.sHtML


<!-- 参考信息 -->