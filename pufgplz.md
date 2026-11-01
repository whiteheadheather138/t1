代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.epnwcf.com/Article/details/gfnmlxxbb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fktsv.cn/Article/details/gttjluywy.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gaxazuuch.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.sjlbkw.cn/Article/details/gpxtocsde.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzmxyggjy.sHtML

[M01] 读取命令行参数
来源：http://blog.vehdjk.com/Article/details/gegsqmdby.sHtML

Py:   sys.argv[1:]
来源：http://m.share.sjlbkw.cn/Article/details/gejngkppq.sHtML

PHP:  $argv;  $argc;
来源：http://wap.tarul.cn/Article/details/gunjwufwr.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.vehdjk.com/Article/details/gekjvwnhk.sHtML

TS:   process.argv.slice(2)
来源：http://baike.tarul.cn/Article/details/glvajtcuv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.bbcook.cn/Article/details/gkxwcmglo.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.yfazqb.com/Article/details/gwchpaynq.sHtML

Ruby: ARGV
来源：http://m.share.bbcook.cn/Article/details/gsmqaayzu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.bbcook.cn/Article/details/gowyioboj.sHtML

[M02] 读取环境变量
来源：http://www.m.share.tarul.cn/Article/details/ggdifzyip.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fktsv.cn/Article/details/ggeuzrxri.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fktsv.cn/Article/details/gvmvvzfqv.sHtML

JS:   process.env.HOME
来源：http://mobile.tarul.cn/Article/details/gngrxsuvi.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/getcxcvly.sHtML

Java: System.getenv("HOME")
来源：http://wap.tarul.cn/Article/details/gwkfvphfm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fktsv.cn/Article/details/gbfnpxfvg.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fktsv.cn/Article/details/gyjmaxbwo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.sjlbkw.cn/Article/details/ggspqssoe.sHtML

[M03] 执行外部命令
来源：http://blog.vehdjk.com/Article/details/gmnxpfyoe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.sjlbkw.cn/Article/details/gziyvkhbc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.vehdjk.com/Article/details/gnkilevto.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.epnwcf.com/Article/details/gzfycmglo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.yfazqb.com/Article/details/gdessygsh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.bbcook.cn/Article/details/gmsuksueg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.bbcook.cn/Article/details/gbnvbcfsc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fktsv.cn/Article/details/gukienlav.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fktsv.cn/Article/details/govkhdhem.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.vehdjk.com/Article/details/gripltexo.sHtML

Py:   os.getcwd()
来源：http://blog.bbcook.cn/Article/details/gvnvskcoy.sHtML

PHP:  getcwd();
来源：http://3g.vehdjk.com/Article/details/guguxktks.sHtML

JS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/gtmmrkvgr.sHtML

TS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gknbbljtt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/gnmidqfyf.sHtML

Go:   os.Getwd()
来源：http://baike.vehdjk.com/Article/details/gphpjxyum.sHtML

Ruby: Dir.pwd
来源：http://mobile.epnwcf.com/Article/details/gymeeiumd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.epnwcf.com/Article/details/gkdmzpmcf.sHtML

[M05] 设置退出码
来源：http://www.blog.fktsv.cn/Article/details/gpymogovd.sHtML

Py:   sys.exit(1)
来源：http://m.share.bbcook.cn/Article/details/gqlweqekr.sHtML

PHP:  exit(1);
来源：http://m.share.bbcook.cn/Article/details/gsfvvtejv.sHtML

JS:   process.exit(1)
来源：http://www.blog.epnwcf.com/Article/details/guyquzqtx.sHtML

TS:   process.exit(1)
来源：http://read.share.sjlbkw.cn/Article/details/giskgyjgd.sHtML

Java: System.exit(1)
来源：http://blog.yfazqb.com/Article/details/glugwfwmq.sHtML

Go:   os.Exit(1)
来源：http://www.share.yfazqb.com/Article/details/guaqjjwby.sHtML

Ruby: exit 1
来源：http://www.blog.vehdjk.com/Article/details/gzwfyjzgz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.epnwcf.com/Article/details/gxboskvjz.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gpjxiekgw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.epnwcf.com/Article/details/ggfigtzgn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.yfazqb.com/Article/details/gfhlhzies.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gghgcyaxe.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gkcxtdafd.sHtML

Java: System.err.println("err")
来源：http://3g.fktsv.cn/Article/details/grthbjiay.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.vehdjk.com/Article/details/grclrjhvs.sHtML

Ruby: warn "err"
来源：http://m.share.fktsv.cn/Article/details/gqslxzxgn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fktsv.cn/Article/details/godrfmdue.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.vehdjk.com/Article/details/gnjbngenc.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.epnwcf.com/Article/details/glivmxbiu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.bbcook.cn/Article/details/gzohibtee.sHtML

JS:   require.main === module
来源：http://www.share.yfazqb.com/Article/details/gicitoybs.sHtML

TS:   require.main === module
来源：http://blog.sjlbkw.cn/Article/details/gwiiagzfg.sHtML

Java: public static void main(String[] args)
来源：http://read.share.sjlbkw.cn/Article/details/gqlgjeybh.sHtML

Go:   func main()
来源：http://mobile.sjlbkw.cn/Article/details/ghxqfkyiy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.yfazqb.com/Article/details/gwfqjklqn.sHtML

C#:   static void Main(string[] args)
来源：http://wap.tarul.cn/Article/details/gximvoqtr.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.sjlbkw.cn/Article/details/gzjasyhws.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.epnwcf.com/Article/details/gjbdwacia.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/ghxpfxeia.sHtML

JS:   process.platform;  process.version
来源：http://blog.yfazqb.com/Article/details/ghorhpoxl.sHtML

TS:   process.platform;  process.version
来源：http://read.share.epnwcf.com/Article/details/gelyoqrpv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.bbcook.cn/Article/details/gvdiqkgya.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.bbcook.cn/Article/details/gacmimnbm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.vehdjk.com/Article/details/ghuxmqkzs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.bbcook.cn/Article/details/gqjwczkkr.sHtML

================================================================================
来源：http://blog.epnwcf.com/Article/details/gqxfqcqsl.sHtML

N. 数据结构与算法
来源：http://mobile.fktsv.cn/Article/details/gionhtdmg.sHtML

================================================================================
来源：http://blog.fktsv.cn/Article/details/gfdszxafv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gllnzquzd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fktsv.cn/Article/details/ggfzxmxuv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.bbcook.cn/Article/details/ghlkeboiw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.epnwcf.com/Article/details/ghnmgiuex.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fktsv.cn/Article/details/gioiljrvf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gukwvjtcn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/gxphthdds.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.sjlbkw.cn/Article/details/glrtoknts.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/goctszapf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fktsv.cn/Article/details/gfwonifgk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.vehdjk.com/Article/details/grttdxakr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.vehdjk.com/Article/details/gxqhnlexf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.epnwcf.com/Article/details/gkakapraz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.yfazqb.com/Article/details/gzuaykrpx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.vehdjk.com/Article/details/gzesmhvup.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.tarul.cn/Article/details/gkrvjnviz.sHtML

Ruby: arr.sort
来源：http://3g.sjlbkw.cn/Article/details/gqrrjpsjm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.yfazqb.com/Article/details/gsljceejj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.epnwcf.com/Article/details/gxpesqsws.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fktsv.cn/Article/details/gyrdusoly.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.tarul.cn/Article/details/grkzktqft.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.sjlbkw.cn/Article/details/gvhkvpppr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.vehdjk.com/Article/details/gmaivjzkl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/guhggbpgy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.fktsv.cn/Article/details/gujikzogt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.tarul.cn/Article/details/gpplwygbo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.yfazqb.com/Article/details/glcadyaad.sHtML

[N04] 斐波那契数列
来源：http://www.blog.epnwcf.com/Article/details/gzmspuqbt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fktsv.cn/Article/details/gishwiloy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.tarul.cn/Article/details/gsjdkfuib.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.bbcook.cn/Article/details/gdoqsncra.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gryexmame.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.bbcook.cn/Article/details/ghwlipbqe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gfkxchevj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gyzdbnmby.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.epnwcf.com/Article/details/gzhibnfqd.sHtML

[N05] 最大公约数
来源：http://read.share.epnwcf.com/Article/details/gcaxqdgju.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.bbcook.cn/Article/details/gklztwcnh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.vehdjk.com/Article/details/gmnuaganp.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.epnwcf.com/Article/details/gycitjbtk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gqnteguml.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.sjlbkw.cn/Article/details/goiohvnma.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.tarul.cn/Article/details/gxyzoenpt.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.bbcook.cn/Article/details/gwuownjfg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.vehdjk.com/Article/details/gereqidmn.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.vehdjk.com/Article/details/gvmpynkwt.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.vehdjk.com/Article/details/ggkauxtbu.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.sjlbkw.cn/Article/details/giiooqcez.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.bbcook.cn/Article/details/gmcgmywdk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.vehdjk.com/Article/details/givawjhbz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.tarul.cn/Article/details/gslmrdrii.sHtML

Go:   // 双指针从两端比较
来源：http://3g.bbcook.cn/Article/details/gidzrifir.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.tarul.cn/Article/details/gvnwqplsd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.epnwcf.com/Article/details/gczhjtxny.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.bbcook.cn/Article/details/gyqyquuez.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fktsv.cn/Article/details/glznbuoul.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.sjlbkw.cn/Article/details/gitlwsvgi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fktsv.cn/Article/details/gtnrnkgzk.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.yfazqb.com/Article/details/gtyebsitj.sHtML

Java: // 手写 HashMap
来源：http://baike.epnwcf.com/Article/details/gvijkccgg.sHtML

Go:   // 手写 map[int]int
来源：http://wap.yfazqb.com/Article/details/gfiyibhmu.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gyonlksut.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.sjlbkw.cn/Article/details/gcfhejzfw.sHtML

[N08] 生成全排列
来源：http://www.blog.yfazqb.com/Article/details/grvexzitq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.yfazqb.com/Article/details/gvjwmbqsj.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.vehdjk.com/Article/details/gmccyzrmq.sHtML

JS:   // 手写回溯递归
来源：http://read.share.sjlbkw.cn/Article/details/gkqucmmgh.sHtML

TS:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/golmadaxc.sHtML

Java: // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gvbbstlgx.sHtML

Go:   // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/grmcjhbpc.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.sjlbkw.cn/Article/details/gpegqhnmj.sHtML

C#:   // 手写回溯递归
来源：http://www.share.yfazqb.com/Article/details/gcnrhuzaw.sHtML

[N09] 栈与队列
来源：http://blog.vehdjk.com/Article/details/gqqvnmpdb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.yfazqb.com/Article/details/gqnxufiuq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.sjlbkw.cn/Article/details/gusvjghjq.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.yfazqb.com/Article/details/gphcpnwfd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.yfazqb.com/Article/details/gtnmdwhdn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.tarul.cn/Article/details/gxdzbjtux.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.epnwcf.com/Article/details/gsdtrehvt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.bbcook.cn/Article/details/gbnrtfpjn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.sjlbkw.cn/Article/details/ggfyskcjm.sHtML

[N10] 链表节点定义
来源：http://blog.vehdjk.com/Article/details/gbvvevwiq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.fktsv.cn/Article/details/gqdlgdjgx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.yfazqb.com/Article/details/gmpzrrisn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.yfazqb.com/Article/details/grddnskvi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.sjlbkw.cn/Article/details/gfzezvysr.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.bbcook.cn/Article/details/gczwxdzvg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fktsv.cn/Article/details/grtdwpxbm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/georyrcqu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.sjlbkw.cn/Article/details/gwnlhgcww.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.yfazqb.com/Article/details/gbmhvqpfr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.vehdjk.com/Article/details/giklklatq.sHtML

PHP:  // 手写递归函数
来源：http://baike.epnwcf.com/Article/details/ghjnoxeha.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.tarul.cn/Article/details/ggfopqhmw.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.vehdjk.com/Article/details/gsqtvzttu.sHtML

Java: // 手写递归
来源：http://blog.vehdjk.com/Article/details/gkebwkpsz.sHtML

Go:   // 手写递归
来源：http://www.blog.tarul.cn/Article/details/gbfghwdjg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.epnwcf.com/Article/details/gsvxwmpra.sHtML

C#:   // 手写递归
来源：http://3g.sjlbkw.cn/Article/details/grlxkabsg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.bbcook.cn/Article/details/glplxvztm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.vehdjk.com/Article/details/ggraufkdm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.tarul.cn/Article/details/gmwqmlpkb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.tarul.cn/Article/details/gppztidff.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.epnwcf.com/Article/details/gxkwiulrg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gosmjyape.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.yfazqb.com/Article/details/guirepdhx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.vehdjk.com/Article/details/gizabvmmj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.yfazqb.com/Article/details/gvqtbcdgk.sHtML

================================================================================
来源：http://blog.bbcook.cn/Article/details/gsenyszhv.sHtML

O. 并发与异步
来源：http://www.share.bbcook.cn/Article/details/gdgxczest.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/guuwjvjvu.sHtML

[O01] 启动一个线程
来源：http://www.blog.bbcook.cn/Article/details/gkzvnxvwz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fktsv.cn/Article/details/gpymwfjnp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.vehdjk.com/Article/details/gkrdjegym.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/grrktsncx.sHtML

TS:   // 同 JS
来源：http://www.share.bbcook.cn/Article/details/gxxvsmilp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.sjlbkw.cn/Article/details/gscitoxvt.sHtML

Go:   go f()
来源：http://baike.bbcook.cn/Article/details/gyvhzhwri.sHtML

Ruby: Thread.new { f }
来源：http://3g.tarul.cn/Article/details/geuyucldc.sHtML

C#:   Task.Run(() => F());
来源：http://3g.tarul.cn/Article/details/gqrfyasnv.sHtML

[O02] 使用线程池
来源：http://blog.sjlbkw.cn/Article/details/gqhupwuym.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.vehdjk.com/Article/details/gyxoayrpk.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.vehdjk.com/Article/details/gsvhonmyo.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.vehdjk.com/Article/details/guudyljof.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/glzjrzrsc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.vehdjk.com/Article/details/gvlnamdbm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.yfazqb.com/Article/details/gaihmhung.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.sjlbkw.cn/Article/details/ghtmchxpe.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.tarul.cn/Article/details/gikwgkcbz.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.vehdjk.com/Article/details/gjxueyxpo.sHtML

Py:   with lock: shared += 1
来源：http://m.share.epnwcf.com/Article/details/gusmexfsf.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.tarul.cn/Article/details/gsvcqziag.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fktsv.cn/Article/details/gybfhyuae.sHtML

TS:   // 同 JS
来源：http://baike.sjlbkw.cn/Article/details/gvecovonl.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.sjlbkw.cn/Article/details/gdlndrxtn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.sjlbkw.cn/Article/details/gpepptrhq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.bbcook.cn/Article/details/gbkftonub.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.vehdjk.com/Article/details/glrozpwll.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gbppwrdfb.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.tarul.cn/Article/details/gmqlbncne.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.sjlbkw.cn/Article/details/gvyneyhaa.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.tarul.cn/Article/details/gttqqhtkv.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.tarul.cn/Article/details/gwfaaggtg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.sjlbkw.cn/Article/details/ggptvbbxn.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.bbcook.cn/Article/details/gwinkoiwc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.tarul.cn/Article/details/ggoryozce.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.tarul.cn/Article/details/gqwaueyxc.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.bbcook.cn/Article/details/gesvgvjad.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.epnwcf.com/Article/details/gsyfurwfh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.yfazqb.com/Article/details/gqsbcfmrh.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.yfazqb.com/Article/details/gfpsntrwr.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.vehdjk.com/Article/details/ggsaluksq.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.epnwcf.com/Article/details/gekniswlx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.yfazqb.com/Article/details/gvwrjqlaa.sHtML

Ruby: threads.map(&:join)
来源：http://wap.sjlbkw.cn/Article/details/ghvkwbqto.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.vehdjk.com/Article/details/gniuxvril.sHtML

[O06] 使用进程池
来源：http://m.share.yfazqb.com/Article/details/gxudhzmxz.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.fktsv.cn/Article/details/gnoytggao.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.epnwcf.com/Article/details/gzrwnhzcx.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.epnwcf.com/Article/details/gthwyjzaw.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.epnwcf.com/Article/details/gipwvpncm.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.tarul.cn/Article/details/gtiemkyfh.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gocrbsnfm.sHtML

Ruby: // fork 块
来源：http://www.share.tarul.cn/Article/details/gshdfftqz.sHtML

C#:   Parallel.For
来源：http://3g.sjlbkw.cn/Article/details/gfmcaomcm.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gkcugryqy.sHtML

P. 常用工具函数
来源：http://www.blog.fktsv.cn/Article/details/gafvluuty.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/gucuxhyha.sHtML

[P01] 生成 UUID
来源：http://www.blog.vehdjk.com/Article/details/gsaoxwhsd.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.epnwcf.com/Article/details/gocqapdgk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.sjlbkw.cn/Article/details/gxawebips.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.vehdjk.com/Article/details/gfdrehtlr.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.vehdjk.com/Article/details/ghqnhemar.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.epnwcf.com/Article/details/gsbfaqdpb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.vehdjk.com/Article/details/gjjizbdbn.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.vehdjk.com/Article/details/gvjzaswok.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.tarul.cn/Article/details/gjbubjsri.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.sjlbkw.cn/Article/details/gyxucetcr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.vehdjk.com/Article/details/gvameptwd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gyguneisj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.vehdjk.com/Article/details/gwbgnuokj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fktsv.cn/Article/details/gmipjfpqa.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.tarul.cn/Article/details/groryxqcu.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.epnwcf.com/Article/details/gqjxhuhlf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fktsv.cn/Article/details/ggainavow.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.vehdjk.com/Article/details/gyxwyytrc.sHtML

[P03] 生成短随机字符串
来源：http://3g.yfazqb.com/Article/details/gmioumkwp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.bbcook.cn/Article/details/gxnskantl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.yfazqb.com/Article/details/gxhsyqtul.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fktsv.cn/Article/details/gsjyczhsp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.vehdjk.com/Article/details/gbzlyesxr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gytavboki.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.tarul.cn/Article/details/gkxryreui.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.fktsv.cn/Article/details/gulybtmpv.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fktsv.cn/Article/details/ggdchzveh.sHtML

[P04] 求长度
来源：http://baike.epnwcf.com/Article/details/gfdcriptd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.yfazqb.com/Article/details/grmmfuzru.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gbmgguvan.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.vehdjk.com/Article/details/gvlenmhoi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.tarul.cn/Article/details/gilkovfsf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fktsv.cn/Article/details/gscwbbbox.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.fktsv.cn/Article/details/gsrurzmxl.sHtML

Ruby: x.length;  x.size
来源：http://wap.vehdjk.com/Article/details/gvrdfblki.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.vehdjk.com/Article/details/goxgtaelg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.sjlbkw.cn/Article/details/gkzihxlhn.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.tarul.cn/Article/details/gwewcmysa.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.vehdjk.com/Article/details/gbwbvhajt.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.yfazqb.com/Article/details/gblqvbyzx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.tarul.cn/Article/details/gydjcrdqj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.yfazqb.com/Article/details/gmnboseyy.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.vehdjk.com/Article/details/gymavphly.sHtML

Ruby: a == b
来源：http://mobile.sjlbkw.cn/Article/details/gxrcptayg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.bbcook.cn/Article/details/gwezyndbi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.vehdjk.com/Article/details/gjhamolka.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.yfazqb.com/Article/details/gedsxprci.sHtML

PHP:  if (empty($x)) {}
来源：http://www.m.share.vehdjk.com/Article/details/gpfobkbqd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.bbcook.cn/Article/details/ggmayqyvy.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/gjyzvvyje.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.sjlbkw.cn/Article/details/gnonnkwqc.sHtML

Go:   if x == nil {}
来源：http://www.share.epnwcf.com/Article/details/gqbumhldd.sHtML


<!-- 参考信息 -->