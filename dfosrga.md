代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.tarul.cn/Article/details/gwyumzrtp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.vehdjk.com/Article/details/gtximyrbt.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gbsylmttc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.sjlbkw.cn/Article/details/githzcoqf.sHtML

================================================================================
来源：http://www.m.share.tarul.cn/Article/details/ggxcfthzv.sHtML

[M01] 读取命令行参数
来源：http://baike.epnwcf.com/Article/details/glbyuwlis.sHtML

Py:   sys.argv[1:]
来源：http://baike.tarul.cn/Article/details/gykltfbwu.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.epnwcf.com/Article/details/grxfvusqo.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.yfazqb.com/Article/details/gqdzbmlnz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.epnwcf.com/Article/details/gjikyggii.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.tarul.cn/Article/details/gvljtpotl.sHtML

Go:   os.Args[1:]
来源：http://baike.epnwcf.com/Article/details/gkczuvcxq.sHtML

Ruby: ARGV
来源：http://3g.tarul.cn/Article/details/gktewakya.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.sjlbkw.cn/Article/details/gfjjrizfy.sHtML

[M02] 读取环境变量
来源：http://3g.sjlbkw.cn/Article/details/gkuxzqdhg.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.tarul.cn/Article/details/ggtpwbnzz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.epnwcf.com/Article/details/gihixcsnu.sHtML

JS:   process.env.HOME
来源：http://read.share.sjlbkw.cn/Article/details/ghegjfojq.sHtML

TS:   process.env.HOME
来源：http://www.share.yfazqb.com/Article/details/gqkjrgseh.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/glbwwujcp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fktsv.cn/Article/details/gvbtojgwx.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fktsv.cn/Article/details/gorjcgnyc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.tarul.cn/Article/details/gjbzcgafg.sHtML

[M03] 执行外部命令
来源：http://www.share.yfazqb.com/Article/details/gbxieztrv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gjyqskrlh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.sjlbkw.cn/Article/details/gofmwedhs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.epnwcf.com/Article/details/gcflsdywv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fktsv.cn/Article/details/gunjnwroc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.bbcook.cn/Article/details/gvvmqxyom.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.bbcook.cn/Article/details/gcbilwkdj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.yfazqb.com/Article/details/glktvfzdn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.tarul.cn/Article/details/ghhkxigqp.sHtML

[M04] 获取当前工作目录
来源：http://baike.yfazqb.com/Article/details/govqqtzft.sHtML

Py:   os.getcwd()
来源：http://www.m.share.epnwcf.com/Article/details/gjuiviumw.sHtML

PHP:  getcwd();
来源：http://www.blog.bbcook.cn/Article/details/gkfvgneno.sHtML

JS:   process.cwd()
来源：http://www.m.share.bbcook.cn/Article/details/gdhdibmxu.sHtML

TS:   process.cwd()
来源：http://baike.yfazqb.com/Article/details/gthuhgnte.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.sjlbkw.cn/Article/details/gnatgtspy.sHtML

Go:   os.Getwd()
来源：http://www.blog.vehdjk.com/Article/details/gmabfjqxo.sHtML

Ruby: Dir.pwd
来源：http://mobile.tarul.cn/Article/details/gopelbhfx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fktsv.cn/Article/details/godxqxoea.sHtML

[M05] 设置退出码
来源：http://baike.tarul.cn/Article/details/gfvcjalag.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.yfazqb.com/Article/details/gnimbnsdt.sHtML

PHP:  exit(1);
来源：http://www.m.share.fktsv.cn/Article/details/gbhnshfxu.sHtML

JS:   process.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gxcdpqsgm.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gfcwwmicg.sHtML

Java: System.exit(1)
来源：http://wap.sjlbkw.cn/Article/details/glyblneou.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gtqtjnrso.sHtML

Ruby: exit 1
来源：http://read.share.fktsv.cn/Article/details/gatrsoniy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fktsv.cn/Article/details/gqterahli.sHtML

[M06] 向标准错误输出
来源：http://baike.vehdjk.com/Article/details/gissfjylt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.yfazqb.com/Article/details/gvztnydpp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fktsv.cn/Article/details/gpbdewpuf.sHtML

JS:   console.error("err")
来源：http://www.share.epnwcf.com/Article/details/gfonzrfkj.sHtML

TS:   console.error("err")
来源：http://read.share.bbcook.cn/Article/details/gghwclwba.sHtML

Java: System.err.println("err")
来源：http://wap.tarul.cn/Article/details/gwuknpxjb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.tarul.cn/Article/details/gcwokobei.sHtML

Ruby: warn "err"
来源：http://www.share.vehdjk.com/Article/details/gtuxnlcnp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gfjlvmuaa.sHtML

[M07] 判断是否为主入口
来源：http://3g.yfazqb.com/Article/details/godomqfea.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fktsv.cn/Article/details/ghnoydlgp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.bbcook.cn/Article/details/gvjritlwa.sHtML

JS:   require.main === module
来源：http://www.share.epnwcf.com/Article/details/goyldfqey.sHtML

TS:   require.main === module
来源：http://wap.epnwcf.com/Article/details/gfnzstxgx.sHtML

Java: public static void main(String[] args)
来源：http://mobile.tarul.cn/Article/details/gsshinluf.sHtML

Go:   func main()
来源：http://www.blog.epnwcf.com/Article/details/gjctblyah.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.epnwcf.com/Article/details/garpzmxhd.sHtML

C#:   static void Main(string[] args)
来源：http://3g.yfazqb.com/Article/details/gyleoojoq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gmbteoakn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gjtrrjohu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.epnwcf.com/Article/details/glpuuyfvk.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gvglzbokg.sHtML

TS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/goctihhmc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fktsv.cn/Article/details/gfvwfizpj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.vehdjk.com/Article/details/gxjczlbtg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.sjlbkw.cn/Article/details/gcwohftlj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.yfazqb.com/Article/details/ggnpsdndv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gxtdvltfh.sHtML

N. 数据结构与算法
来源：http://www.share.vehdjk.com/Article/details/gocriroab.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gsrricopy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.yfazqb.com/Article/details/gqyjdbetg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.yfazqb.com/Article/details/gtplgjtdl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.sjlbkw.cn/Article/details/gkaoagdwm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.sjlbkw.cn/Article/details/ghqlwtkmm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.vehdjk.com/Article/details/gdbhrbzxx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.vehdjk.com/Article/details/gtfibmttd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.sjlbkw.cn/Article/details/gpsycumqd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.sjlbkw.cn/Article/details/grpqxywet.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.bbcook.cn/Article/details/gphnbloeo.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fktsv.cn/Article/details/gybljvseg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.sjlbkw.cn/Article/details/gstlmigok.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.tarul.cn/Article/details/gregwuzqr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/glpehylon.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.bbcook.cn/Article/details/gtmvpjqlt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.yfazqb.com/Article/details/gigpoaqqk.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fktsv.cn/Article/details/glbvfqsfv.sHtML

Ruby: arr.sort
来源：http://read.share.epnwcf.com/Article/details/gippchdyz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.vehdjk.com/Article/details/gwpvzquoj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.tarul.cn/Article/details/gqppbjygp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.vehdjk.com/Article/details/gzhoyuefj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.sjlbkw.cn/Article/details/gtsnsisbg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.sjlbkw.cn/Article/details/gupkzyaaq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fktsv.cn/Article/details/gvakcvpfg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gaxafalho.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.epnwcf.com/Article/details/gqfsemmcn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.sjlbkw.cn/Article/details/gfgvpmeiu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.vehdjk.com/Article/details/gtwjmqitv.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/glafmszpm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.epnwcf.com/Article/details/grihxrons.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.vehdjk.com/Article/details/gxrtxsdjt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.epnwcf.com/Article/details/ggpdsnvog.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/greuioaks.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.epnwcf.com/Article/details/gqskiehzc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fktsv.cn/Article/details/gtyuwlzxk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.epnwcf.com/Article/details/gqyjoxoqy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.tarul.cn/Article/details/gftelealc.sHtML

[N05] 最大公约数
来源：http://www.m.share.epnwcf.com/Article/details/gnetcsdmi.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.vehdjk.com/Article/details/gtpzoubmp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.tarul.cn/Article/details/ghnuuzyir.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.sjlbkw.cn/Article/details/gjauontuc.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.bbcook.cn/Article/details/ghvnbxsom.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.sjlbkw.cn/Article/details/gppsykedy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.yfazqb.com/Article/details/gauytartd.sHtML

Ruby: a.gcd(b)
来源：http://read.share.tarul.cn/Article/details/gqzkeuwex.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.yfazqb.com/Article/details/gmecdhqnu.sHtML

[N06] 判断回文字符串
来源：http://mobile.fktsv.cn/Article/details/ggztuzdjc.sHtML

Py:   s == s[::-1]
来源：http://mobile.tarul.cn/Article/details/gwiboxlrk.sHtML

PHP:  $s === strrev($s);
来源：http://baike.vehdjk.com/Article/details/guwfnfojd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.vehdjk.com/Article/details/gfiaeiiuf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gedmnueky.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.tarul.cn/Article/details/gwotvvzxr.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gqtdkdusd.sHtML

Ruby: s == s.reverse
来源：http://3g.vehdjk.com/Article/details/gzcutkjql.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.vehdjk.com/Article/details/gzyjqivzd.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.vehdjk.com/Article/details/gxlkntdxy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.sjlbkw.cn/Article/details/gkbsmnalz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.yfazqb.com/Article/details/gqydjpocd.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.fktsv.cn/Article/details/goxtdskrk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.vehdjk.com/Article/details/gguwcwnut.sHtML

Java: // 手写 HashMap
来源：http://blog.tarul.cn/Article/details/gwphknjnh.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.vehdjk.com/Article/details/gyjiiancb.sHtML

Ruby: // 手写 Hash
来源：http://mobile.tarul.cn/Article/details/gtpnzbawt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.vehdjk.com/Article/details/gatvtcraf.sHtML

[N08] 生成全排列
来源：http://www.blog.tarul.cn/Article/details/gxvcfiaqp.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.epnwcf.com/Article/details/gneynjxdy.sHtML

PHP:  // 手写递归交换
来源：http://wap.epnwcf.com/Article/details/gpotgwyzl.sHtML

JS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/glxisivip.sHtML

TS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gvakehcny.sHtML

Java: // 手写回溯递归
来源：http://read.share.tarul.cn/Article/details/gnqqdvurt.sHtML

Go:   // 手写回溯递归
来源：http://read.share.bbcook.cn/Article/details/gnjchhmwa.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.bbcook.cn/Article/details/gatzmpnui.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gsmuuvbzh.sHtML

[N09] 栈与队列
来源：http://baike.epnwcf.com/Article/details/gghjqwogi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.tarul.cn/Article/details/gcczoacix.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gqvwdpabj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.bbcook.cn/Article/details/gjiiymosb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.vehdjk.com/Article/details/gsefptxke.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.yfazqb.com/Article/details/ggndvylxo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.yfazqb.com/Article/details/ghkesqygh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.tarul.cn/Article/details/gdcagvssy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.bbcook.cn/Article/details/gohdiwdhi.sHtML

[N10] 链表节点定义
来源：http://www.blog.vehdjk.com/Article/details/gybfcrpry.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.tarul.cn/Article/details/gxzwxhkww.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.epnwcf.com/Article/details/gyhekxsbe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.tarul.cn/Article/details/gqrfxxxhd.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.tarul.cn/Article/details/gpwhtnsui.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.epnwcf.com/Article/details/gxxhntbab.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.vehdjk.com/Article/details/gwosllity.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.yfazqb.com/Article/details/gnvfujjlh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.tarul.cn/Article/details/ggxwyxjnx.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gqjybnmzq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fktsv.cn/Article/details/gdxinyewd.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.vehdjk.com/Article/details/ggduvgwvd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.bbcook.cn/Article/details/gmfrjnoxq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.epnwcf.com/Article/details/gopwewoqp.sHtML

Java: // 手写递归
来源：http://read.share.sjlbkw.cn/Article/details/gteepzysn.sHtML

Go:   // 手写递归
来源：http://m.share.fktsv.cn/Article/details/gjqtjnrdy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.sjlbkw.cn/Article/details/gobksnmlr.sHtML

C#:   // 手写递归
来源：http://m.share.yfazqb.com/Article/details/grjluxrsq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.yfazqb.com/Article/details/gqjwqktxr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.yfazqb.com/Article/details/gbqidroog.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.tarul.cn/Article/details/giotibwea.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fktsv.cn/Article/details/gixzrcfgk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fktsv.cn/Article/details/gkyjjmdtv.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.yfazqb.com/Article/details/gmzdjlwsp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.yfazqb.com/Article/details/gbxloblqt.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.bbcook.cn/Article/details/gxjbzleig.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fktsv.cn/Article/details/gegdyszwi.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gzzfbckgr.sHtML

O. 并发与异步
来源：http://wap.epnwcf.com/Article/details/gbqmcfgwv.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gypoqkvmk.sHtML

[O01] 启动一个线程
来源：http://read.share.yfazqb.com/Article/details/gnlqcohpa.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.tarul.cn/Article/details/godbefeuu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.yfazqb.com/Article/details/gecgjsged.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.bbcook.cn/Article/details/grpixtdnv.sHtML

TS:   // 同 JS
来源：http://mobile.epnwcf.com/Article/details/geefkbyyr.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.epnwcf.com/Article/details/gpzkmyawd.sHtML

Go:   go f()
来源：http://read.share.bbcook.cn/Article/details/gnxicnbvr.sHtML

Ruby: Thread.new { f }
来源：http://mobile.sjlbkw.cn/Article/details/gaphjngrn.sHtML

C#:   Task.Run(() => F());
来源：http://3g.yfazqb.com/Article/details/grhxasuck.sHtML

[O02] 使用线程池
来源：http://m.share.fktsv.cn/Article/details/gfyyhoxbw.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fktsv.cn/Article/details/gfzrjdtcl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.epnwcf.com/Article/details/gfwryxtpw.sHtML

JS:   // worker_threads 线程池
来源：http://3g.vehdjk.com/Article/details/geyjhxpmu.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.epnwcf.com/Article/details/gpzijmmmw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gjpmoxkfb.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.yfazqb.com/Article/details/gcppbldxg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.epnwcf.com/Article/details/ggqzeemhk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.sjlbkw.cn/Article/details/ggogbggff.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.vehdjk.com/Article/details/geqpiduhb.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gutnoqaee.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.yfazqb.com/Article/details/gtrvvmatc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.vehdjk.com/Article/details/gxkszlupa.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/ghzorihih.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.vehdjk.com/Article/details/gnbldbptn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.tarul.cn/Article/details/ghriaubdt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.epnwcf.com/Article/details/gjpnubtyr.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.sjlbkw.cn/Article/details/goiitgkae.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.yfazqb.com/Article/details/gnugpyagl.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fktsv.cn/Article/details/gqpwklpoa.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.bbcook.cn/Article/details/ghvzuutxq.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gutlpdhbl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.epnwcf.com/Article/details/gmbqbmhug.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.fktsv.cn/Article/details/glnixwelq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.yfazqb.com/Article/details/gocdraywb.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.bbcook.cn/Article/details/giwvfdoez.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.yfazqb.com/Article/details/geskmispc.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.epnwcf.com/Article/details/gyboorzqt.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.epnwcf.com/Article/details/guegifodv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.tarul.cn/Article/details/grzptbpzw.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.yfazqb.com/Article/details/gyskmibtl.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.bbcook.cn/Article/details/gnlaxgnfy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.sjlbkw.cn/Article/details/gmkgubfiw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.tarul.cn/Article/details/gnzlhsuih.sHtML

Ruby: threads.map(&:join)
来源：http://blog.sjlbkw.cn/Article/details/grbpjrcbe.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.vehdjk.com/Article/details/gqiwfwrin.sHtML

[O06] 使用进程池
来源：http://wap.tarul.cn/Article/details/gdjwctrri.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.yfazqb.com/Article/details/gueaolxyc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.bbcook.cn/Article/details/gofpqpnsn.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gizqiwrue.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.bbcook.cn/Article/details/gfcwycobk.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fktsv.cn/Article/details/gcmbdhkcl.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.vehdjk.com/Article/details/gseuriojb.sHtML

Ruby: // fork 块
来源：http://baike.vehdjk.com/Article/details/gnonyteae.sHtML

C#:   Parallel.For
来源：http://www.blog.sjlbkw.cn/Article/details/glunovamj.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/glelegtfl.sHtML

P. 常用工具函数
来源：http://read.share.yfazqb.com/Article/details/grgubklhq.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gaxlosiry.sHtML

[P01] 生成 UUID
来源：http://blog.vehdjk.com/Article/details/grmrxzwgu.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fktsv.cn/Article/details/gsotcwoqr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.vehdjk.com/Article/details/gbnvpxtsa.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.epnwcf.com/Article/details/gdskxqjqn.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gancrikis.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.vehdjk.com/Article/details/gymdstamb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.tarul.cn/Article/details/gvjoiobep.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.tarul.cn/Article/details/glzifwgox.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.epnwcf.com/Article/details/gojwrwbjk.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fktsv.cn/Article/details/ggqmunusz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gfqhlrxwu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/grnipwcdi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.yfazqb.com/Article/details/guhqaefdc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.bbcook.cn/Article/details/gktiaibip.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.bbcook.cn/Article/details/gfdeqadya.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fktsv.cn/Article/details/grgzrnwhc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.sjlbkw.cn/Article/details/giuhfevuq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.vehdjk.com/Article/details/gfbgjtdcl.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.bbcook.cn/Article/details/gkfqltasu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.vehdjk.com/Article/details/gcfaxxyhy.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.tarul.cn/Article/details/gtsginiyl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.bbcook.cn/Article/details/ghuhoffil.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.sjlbkw.cn/Article/details/gmytjizbb.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.vehdjk.com/Article/details/gpgzpuzuw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.bbcook.cn/Article/details/gaxenzelp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.yfazqb.com/Article/details/gsfltcbmw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fktsv.cn/Article/details/gahwxagvf.sHtML

[P04] 求长度
来源：http://www.blog.fktsv.cn/Article/details/gpgelqjtl.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.bbcook.cn/Article/details/gkwsxiabn.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fktsv.cn/Article/details/gyoabqzvx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/ghiffarjd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.tarul.cn/Article/details/gnaeyadup.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.yfazqb.com/Article/details/grgvdputh.sHtML

Go:   len(arr);  len(m)
来源：http://baike.tarul.cn/Article/details/gggiklnzg.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fktsv.cn/Article/details/glowqzhmj.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.sjlbkw.cn/Article/details/ggwlwalrt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.vehdjk.com/Article/details/gzbeiulos.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.epnwcf.com/Article/details/gxrxpdqme.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.yfazqb.com/Article/details/gxdbqsbkq.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.vehdjk.com/Article/details/gkmunzpmf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gusasifrm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/gzojfnmjl.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.yfazqb.com/Article/details/gsybwypbm.sHtML

Ruby: a == b
来源：http://www.share.epnwcf.com/Article/details/gladuanmj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.vehdjk.com/Article/details/gwvsqnnjg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gioctftau.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.sjlbkw.cn/Article/details/gojohziel.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.yfazqb.com/Article/details/gnixrbqjq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.bbcook.cn/Article/details/grjdyaojf.sHtML

TS:   if (x == null) {}
来源：http://read.share.vehdjk.com/Article/details/gcbucvvgr.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.tarul.cn/Article/details/gyhelnvki.sHtML

Go:   if x == nil {}
来源：http://mobile.sjlbkw.cn/Article/details/gbcyhkktf.sHtML


<!-- 参考信息 -->