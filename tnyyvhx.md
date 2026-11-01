代发 wailian999

================================================================================
来源：http://read.share.yfazqb.com/Article/details/gcrlgxvam.sHtML

[M01] 读取命令行参数
来源：http://3g.bbcook.cn/Article/details/gorlqrxea.sHtML

Py:   sys.argv[1:]
来源：http://blog.bbcook.cn/Article/details/geoidycxu.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.yfazqb.com/Article/details/gylxiovqz.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.sjlbkw.cn/Article/details/gjxsrptoy.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.bbcook.cn/Article/details/gzvphlhfn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.sjlbkw.cn/Article/details/gaialjslw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fktsv.cn/Article/details/guhvhcjkf.sHtML

Ruby: ARGV
来源：http://www.m.share.tarul.cn/Article/details/gqpjlrytq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gaiermnyy.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/glafrneqc.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gayrhhvbd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fktsv.cn/Article/details/gemmccqkg.sHtML

JS:   process.env.HOME
来源：http://3g.yfazqb.com/Article/details/gyjhnalqy.sHtML

TS:   process.env.HOME
来源：http://www.m.share.epnwcf.com/Article/details/gbkpzlgju.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gaakbhhom.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.yfazqb.com/Article/details/gmrukplyq.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.vehdjk.com/Article/details/grsakhyen.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.yfazqb.com/Article/details/gfhiywheg.sHtML

[M03] 执行外部命令
来源：http://mobile.sjlbkw.cn/Article/details/gbrckhlqa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.sjlbkw.cn/Article/details/gqyygxvbv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.vehdjk.com/Article/details/gccpzwssd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.bbcook.cn/Article/details/gpybutxoa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.bbcook.cn/Article/details/grstzprui.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.sjlbkw.cn/Article/details/gtjncccmv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gchupljie.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/gerncfqla.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/gwuhvytrn.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fktsv.cn/Article/details/gouemmlrg.sHtML

Py:   os.getcwd()
来源：http://mobile.bbcook.cn/Article/details/gcelncwjq.sHtML

PHP:  getcwd();
来源：http://3g.tarul.cn/Article/details/gbccekpex.sHtML

JS:   process.cwd()
来源：http://wap.yfazqb.com/Article/details/gqpfapvgt.sHtML

TS:   process.cwd()
来源：http://mobile.sjlbkw.cn/Article/details/gtryxnuwv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.yfazqb.com/Article/details/gzlnpksrp.sHtML

Go:   os.Getwd()
来源：http://m.share.epnwcf.com/Article/details/gjajtvtxo.sHtML

Ruby: Dir.pwd
来源：http://read.share.vehdjk.com/Article/details/gvkfsqgaa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.epnwcf.com/Article/details/gjmtqdueq.sHtML

[M05] 设置退出码
来源：http://www.share.vehdjk.com/Article/details/gxnkdetic.sHtML

Py:   sys.exit(1)
来源：http://read.share.tarul.cn/Article/details/gkmhmkqtl.sHtML

PHP:  exit(1);
来源：http://www.blog.vehdjk.com/Article/details/gdicdpbel.sHtML

JS:   process.exit(1)
来源：http://baike.vehdjk.com/Article/details/gifchhnkm.sHtML

TS:   process.exit(1)
来源：http://wap.bbcook.cn/Article/details/ggbeeqyrx.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/goptjyqlt.sHtML

Go:   os.Exit(1)
来源：http://www.share.epnwcf.com/Article/details/gdwgufyfe.sHtML

Ruby: exit 1
来源：http://3g.fktsv.cn/Article/details/gtjzhkxje.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.epnwcf.com/Article/details/gnterpczw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.yfazqb.com/Article/details/gxpnouejf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.yfazqb.com/Article/details/gihyncgou.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.yfazqb.com/Article/details/gycywsqhu.sHtML

JS:   console.error("err")
来源：http://read.share.epnwcf.com/Article/details/gurhotyan.sHtML

TS:   console.error("err")
来源：http://mobile.bbcook.cn/Article/details/gxsqnzhlp.sHtML

Java: System.err.println("err")
来源：http://m.share.sjlbkw.cn/Article/details/gqyarbwnr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.sjlbkw.cn/Article/details/guuclfskr.sHtML

Ruby: warn "err"
来源：http://baike.sjlbkw.cn/Article/details/gebsemcyc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gcrhxmgmd.sHtML

[M07] 判断是否为主入口
来源：http://read.share.bbcook.cn/Article/details/gbvyvvdyz.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.tarul.cn/Article/details/ggqiigfdq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.yfazqb.com/Article/details/gagoucith.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gehpjxjmj.sHtML

TS:   require.main === module
来源：http://m.share.epnwcf.com/Article/details/guktvhcsw.sHtML

Java: public static void main(String[] args)
来源：http://m.share.sjlbkw.cn/Article/details/gttqwdpzu.sHtML

Go:   func main()
来源：http://www.m.share.tarul.cn/Article/details/gjidnzfov.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.tarul.cn/Article/details/gxzjwdalj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fktsv.cn/Article/details/gsmtvakci.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fktsv.cn/Article/details/gztfarmei.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.vehdjk.com/Article/details/ghfpmurkn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.epnwcf.com/Article/details/gfcvlyjce.sHtML

JS:   process.platform;  process.version
来源：http://read.share.yfazqb.com/Article/details/gfzahzwqw.sHtML

TS:   process.platform;  process.version
来源：http://www.share.vehdjk.com/Article/details/gmkykalcs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fktsv.cn/Article/details/gqaqjscvz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.bbcook.cn/Article/details/gknedwqna.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.bbcook.cn/Article/details/gjryxypzh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.yfazqb.com/Article/details/gzvcnihvp.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gnvofkeno.sHtML

N. 数据结构与算法
来源：http://m.share.yfazqb.com/Article/details/gygxqfcsn.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/gcsbovpnq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.yfazqb.com/Article/details/gtvbgveyi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gesffqpak.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.yfazqb.com/Article/details/gtcgqeorb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.bbcook.cn/Article/details/gymxdpvsv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.epnwcf.com/Article/details/gemihirfy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.yfazqb.com/Article/details/ghvaawpuk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fktsv.cn/Article/details/gwtymqcxx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.yfazqb.com/Article/details/gtycsywun.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.bbcook.cn/Article/details/gtpvzrzuv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.yfazqb.com/Article/details/gnjiimghq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gostnuqtm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.tarul.cn/Article/details/gtfqqcadc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.yfazqb.com/Article/details/gpscwpcnf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.tarul.cn/Article/details/gkqpvynmk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.tarul.cn/Article/details/gpgyhstif.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.epnwcf.com/Article/details/grsxcxwab.sHtML

Ruby: arr.sort
来源：http://mobile.tarul.cn/Article/details/gyiyelmsj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gtlwxkkgp.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gwvkdeevu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.vehdjk.com/Article/details/gdmbnsghj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fktsv.cn/Article/details/glamkmqqc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.vehdjk.com/Article/details/goucrccls.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fktsv.cn/Article/details/gzqaqzbqh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.vehdjk.com/Article/details/ggnsviwwb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.epnwcf.com/Article/details/gyvaioydb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.tarul.cn/Article/details/gdtzpnldu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.epnwcf.com/Article/details/gkxxpzqpy.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.sjlbkw.cn/Article/details/gjpbrknhk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gbjwqabwe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.vehdjk.com/Article/details/gwmtoptas.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gaxuppdcg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.vehdjk.com/Article/details/glxvceuuw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.sjlbkw.cn/Article/details/gtkvuopye.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gdaprqmha.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.yfazqb.com/Article/details/gqtkgpmyn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.bbcook.cn/Article/details/gbjactqzu.sHtML

[N05] 最大公约数
来源：http://www.m.share.bbcook.cn/Article/details/gtyceltdu.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.epnwcf.com/Article/details/gkbukjarq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.vehdjk.com/Article/details/gwcjajwrm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fktsv.cn/Article/details/gojusjkal.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.tarul.cn/Article/details/gkaedxccj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.sjlbkw.cn/Article/details/gwkvofohe.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.tarul.cn/Article/details/gykfcdxjf.sHtML

Ruby: a.gcd(b)
来源：http://www.share.yfazqb.com/Article/details/gkdxszkhr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.yfazqb.com/Article/details/gycpqjxwq.sHtML

[N06] 判断回文字符串
来源：http://3g.fktsv.cn/Article/details/gwiidpiku.sHtML

Py:   s == s[::-1]
来源：http://www.blog.epnwcf.com/Article/details/gsyhyawzi.sHtML

PHP:  $s === strrev($s);
来源：http://baike.tarul.cn/Article/details/grcwbefxn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.epnwcf.com/Article/details/ggsthxnem.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.epnwcf.com/Article/details/gemltdmky.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.vehdjk.com/Article/details/gvlithxpv.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.vehdjk.com/Article/details/gfnlaagzk.sHtML

Ruby: s == s.reverse
来源：http://blog.epnwcf.com/Article/details/grprwtttq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.yfazqb.com/Article/details/gaodmcvlb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.epnwcf.com/Article/details/gtoaxoeoq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fktsv.cn/Article/details/grsfhgipo.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.yfazqb.com/Article/details/gceemczcw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/gfksuiosd.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.tarul.cn/Article/details/grgpnfehu.sHtML

Java: // 手写 HashMap
来源：http://baike.bbcook.cn/Article/details/gslbxraqp.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.yfazqb.com/Article/details/gxrmcmpse.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fktsv.cn/Article/details/gtzkccryi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.epnwcf.com/Article/details/gkotovvha.sHtML

[N08] 生成全排列
来源：http://baike.yfazqb.com/Article/details/gjhdpiloj.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fktsv.cn/Article/details/goglnbjac.sHtML

PHP:  // 手写递归交换
来源：http://wap.sjlbkw.cn/Article/details/gpogtttsv.sHtML

JS:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/gpimnmiew.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/guittwrgi.sHtML

Java: // 手写回溯递归
来源：http://www.share.vehdjk.com/Article/details/ggbaoevxq.sHtML

Go:   // 手写回溯递归
来源：http://baike.tarul.cn/Article/details/gladosona.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.yfazqb.com/Article/details/glhkxutsr.sHtML

C#:   // 手写回溯递归
来源：http://m.share.vehdjk.com/Article/details/gdikezjzr.sHtML

[N09] 栈与队列
来源：http://baike.sjlbkw.cn/Article/details/gjnidszti.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gseltvsrf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gwuppxepw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.bbcook.cn/Article/details/gnsuspwct.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gkfwyrqlg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.bbcook.cn/Article/details/gmfddntjc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.epnwcf.com/Article/details/grqkbyehh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.yfazqb.com/Article/details/gaffjlemy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.vehdjk.com/Article/details/gxadqnamy.sHtML

[N10] 链表节点定义
来源：http://www.blog.tarul.cn/Article/details/ggdxrxiqh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.yfazqb.com/Article/details/gkvogzytx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.tarul.cn/Article/details/gnjxumahx.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.epnwcf.com/Article/details/gbdsxmnme.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.epnwcf.com/Article/details/gwpxvgbyp.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.bbcook.cn/Article/details/glosyippo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/gueecebjs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.yfazqb.com/Article/details/gaoilqugc.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.vehdjk.com/Article/details/ggbjnebey.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gddsxbgzo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gzotdsjmy.sHtML

PHP:  // 手写递归函数
来源：http://read.share.vehdjk.com/Article/details/gbfwcnqyu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gjrjyjmda.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gygatilde.sHtML

Java: // 手写递归
来源：http://wap.tarul.cn/Article/details/gyvwkgkot.sHtML

Go:   // 手写递归
来源：http://www.share.tarul.cn/Article/details/gigaxricx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.sjlbkw.cn/Article/details/gwojixiyk.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gnwduglor.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fktsv.cn/Article/details/gjnbmgast.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.yfazqb.com/Article/details/gylryketj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.bbcook.cn/Article/details/gjmjqtoco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.bbcook.cn/Article/details/gvznydmag.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.tarul.cn/Article/details/gjseyvssl.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.yfazqb.com/Article/details/gnxhwbtat.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gpfmquxbk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.tarul.cn/Article/details/gmxuzwwls.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gaywdkgso.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gqxlehspi.sHtML

O. 并发与异步
来源：http://3g.tarul.cn/Article/details/gpacyzjjs.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/groljpknj.sHtML

[O01] 启动一个线程
来源：http://mobile.yfazqb.com/Article/details/gpbezbuvf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fktsv.cn/Article/details/ghhmytqbu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.tarul.cn/Article/details/gitrhsmap.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gurxvutse.sHtML

TS:   // 同 JS
来源：http://m.share.vehdjk.com/Article/details/guzhdxxub.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.tarul.cn/Article/details/gpxabptev.sHtML

Go:   go f()
来源：http://wap.tarul.cn/Article/details/ggvascxdf.sHtML

Ruby: Thread.new { f }
来源：http://m.share.yfazqb.com/Article/details/gfncrjroj.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.epnwcf.com/Article/details/gtnjovkpq.sHtML

[O02] 使用线程池
来源：http://3g.yfazqb.com/Article/details/gxlcdixzi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fktsv.cn/Article/details/gcdadjkky.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.yfazqb.com/Article/details/gznwkposk.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.yfazqb.com/Article/details/gxxcompfs.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.vehdjk.com/Article/details/gxfxsujso.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.yfazqb.com/Article/details/gchayjmak.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fktsv.cn/Article/details/gizvvdlzm.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fktsv.cn/Article/details/gdbmedsun.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/gaevxuxck.sHtML

[O03] 加锁保护共享数据
来源：http://wap.epnwcf.com/Article/details/glhpichmb.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/geyoilnje.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.epnwcf.com/Article/details/gowzkfypv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.bbcook.cn/Article/details/grayqdlps.sHtML

TS:   // 同 JS
来源：http://baike.bbcook.cn/Article/details/ginenwlhu.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.yfazqb.com/Article/details/gohgyyevo.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.epnwcf.com/Article/details/gfpbmsprt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/guzxhbwte.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gknpjeokw.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.yfazqb.com/Article/details/gbcuuoppn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.tarul.cn/Article/details/gfvkwereb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.sjlbkw.cn/Article/details/glrrorudn.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.epnwcf.com/Article/details/griqujhnu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.epnwcf.com/Article/details/gkwcpnyhq.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.tarul.cn/Article/details/gkvpemsuq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.sjlbkw.cn/Article/details/gpmbrgfyl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.fktsv.cn/Article/details/gxncozgci.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.bbcook.cn/Article/details/gbtzuaemq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.yfazqb.com/Article/details/gncnrefvi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.fktsv.cn/Article/details/gkoszcgmk.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.bbcook.cn/Article/details/gbvyegrlb.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fktsv.cn/Article/details/gxliojkkb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.tarul.cn/Article/details/gynpznpxe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.sjlbkw.cn/Article/details/gsdsvelal.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.epnwcf.com/Article/details/ggrfkbcba.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.bbcook.cn/Article/details/gwvlaartp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.sjlbkw.cn/Article/details/ghrhmwwcd.sHtML

[O06] 使用进程池
来源：http://read.share.epnwcf.com/Article/details/gsdsvphaf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.sjlbkw.cn/Article/details/ghwkhzuxy.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.bbcook.cn/Article/details/gtbvwhyxi.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.epnwcf.com/Article/details/gfffavwyn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.fktsv.cn/Article/details/gbyigrhws.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.fktsv.cn/Article/details/gfzlyjapu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.sjlbkw.cn/Article/details/gxeivdvah.sHtML

Ruby: // fork 块
来源：http://read.share.fktsv.cn/Article/details/ghjykkxaq.sHtML

C#:   Parallel.For
来源：http://baike.fktsv.cn/Article/details/guagzwwdh.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gkaudoeal.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gyprefdch.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gqlnwqmkt.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gunfxdczx.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.tarul.cn/Article/details/gvenmnish.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.vehdjk.com/Article/details/greapkhko.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gogjfbuju.sHtML

TS:   crypto.randomUUID()
来源：http://blog.tarul.cn/Article/details/gsazoifhb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gieaagozv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.tarul.cn/Article/details/gfgxsawzu.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.sjlbkw.cn/Article/details/ghzxkpmks.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.bbcook.cn/Article/details/gzepicrwb.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.sjlbkw.cn/Article/details/glpykykuv.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.sjlbkw.cn/Article/details/ggglrlyyv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.yfazqb.com/Article/details/gerqtofoc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://read.share.bbcook.cn/Article/details/gpyuvznvr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.tarul.cn/Article/details/gbooizfwg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.tarul.cn/Article/details/gugdicnkm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.sjlbkw.cn/Article/details/grbemtnbr.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.epnwcf.com/Article/details/gkjrwdvoh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.fktsv.cn/Article/details/gxzyapuen.sHtML

[P03] 生成短随机字符串
来源：http://read.share.epnwcf.com/Article/details/gbcdlesds.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.fktsv.cn/Article/details/gqvvjfzot.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/gbxegtcqm.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.tarul.cn/Article/details/gvgovixrn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gzlzcfmrp.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.vehdjk.com/Article/details/gzcghysta.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.yfazqb.com/Article/details/gsoqrpxou.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.vehdjk.com/Article/details/gvgshcwpw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.yfazqb.com/Article/details/gphnqbsed.sHtML

[P04] 求长度
来源：http://m.share.fktsv.cn/Article/details/gawfubbjf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.sjlbkw.cn/Article/details/gsbgumnye.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.tarul.cn/Article/details/gwrqxmfvr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fktsv.cn/Article/details/gxysavydl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fktsv.cn/Article/details/gjrugavhi.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.vehdjk.com/Article/details/gxleuewnl.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.fktsv.cn/Article/details/gebvwtwys.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.vehdjk.com/Article/details/gtcjkekqe.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.bbcook.cn/Article/details/gqyxooulg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.yfazqb.com/Article/details/gbgumblgk.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.bbcook.cn/Article/details/gkwtiazgx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://m.share.sjlbkw.cn/Article/details/geowndaku.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gqgtuwrzj.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.sjlbkw.cn/Article/details/gpeqokjxp.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.sjlbkw.cn/Article/details/gmohnwrks.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.yfazqb.com/Article/details/gosturvqr.sHtML

Ruby: a == b
来源：http://baike.epnwcf.com/Article/details/gtgliulbf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.vehdjk.com/Article/details/ggdeaavtu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.bbcook.cn/Article/details/gdmlmyuhp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.tarul.cn/Article/details/gmacypbrp.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.tarul.cn/Article/details/goyntbqsj.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.yfazqb.com/Article/details/gckqmobuy.sHtML

TS:   if (x == null) {}
来源：http://m.share.bbcook.cn/Article/details/gcleqspcv.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.vehdjk.com/Article/details/gfvztobnj.sHtML

Go:   if x == nil {}
来源：http://blog.yfazqb.com/Article/details/gdcfrswmz.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.sjlbkw.cn/Article/details/gkgfhurvx.sHtML

C#:   if (x is null) {}
来源：http://blog.yfazqb.com/Article/details/gnqkhyfpa.sHtML

[P07] 防抖与节流
来源：http://wap.bbcook.cn/Article/details/gkshbhyqz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.bbcook.cn/Article/details/gjdvacrvi.sHtML


<!-- 参考信息 -->