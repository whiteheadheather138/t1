代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.vehdjk.com/Article/details/gjbwdoick.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.tarul.cn/Article/details/gzzylbnsq.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gvspeikut.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.vehdjk.com/Article/details/gyznavumt.sHtML

================================================================================
来源：http://wap.tarul.cn/Article/details/gwqfbfoen.sHtML

[M01] 读取命令行参数
来源：http://3g.yfazqb.com/Article/details/gtucvurhf.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.tarul.cn/Article/details/goemwcxec.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.bbcook.cn/Article/details/grpdmngme.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gntbgltkn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.vehdjk.com/Article/details/gwbunryqn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fktsv.cn/Article/details/goufboyiy.sHtML

Go:   os.Args[1:]
来源：http://m.share.fktsv.cn/Article/details/gjcnkzanf.sHtML

Ruby: ARGV
来源：http://m.share.vehdjk.com/Article/details/guyvpwygt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.yfazqb.com/Article/details/gshhkqydy.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gnkvsjker.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.sjlbkw.cn/Article/details/gwyamjvbv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/giqxotyjk.sHtML

JS:   process.env.HOME
来源：http://www.blog.tarul.cn/Article/details/gksgfvvls.sHtML

TS:   process.env.HOME
来源：http://read.share.bbcook.cn/Article/details/gvluwwcuv.sHtML

Java: System.getenv("HOME")
来源：http://mobile.yfazqb.com/Article/details/grmoohlez.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fktsv.cn/Article/details/gnkmmenue.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fktsv.cn/Article/details/gxmughfsk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.yfazqb.com/Article/details/gctrpmesy.sHtML

[M03] 执行外部命令
来源：http://www.share.vehdjk.com/Article/details/gsxnamqjv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.tarul.cn/Article/details/gthcnchhd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.bbcook.cn/Article/details/gapcxmdyy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.bbcook.cn/Article/details/gqyxghcpu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.tarul.cn/Article/details/gleqkcqkq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fktsv.cn/Article/details/ghtjldsxr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.epnwcf.com/Article/details/gcvjctxqn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fktsv.cn/Article/details/gfrnkenhs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.tarul.cn/Article/details/gwmmatlnk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.bbcook.cn/Article/details/gwargmcbl.sHtML

Py:   os.getcwd()
来源：http://wap.tarul.cn/Article/details/gbtfivcjj.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/galzwuagw.sHtML

JS:   process.cwd()
来源：http://baike.fktsv.cn/Article/details/gyoxfsweg.sHtML

TS:   process.cwd()
来源：http://blog.yfazqb.com/Article/details/glenzgbgd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.tarul.cn/Article/details/ghrgqqcgg.sHtML

Go:   os.Getwd()
来源：http://blog.bbcook.cn/Article/details/grqqwjynv.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.vehdjk.com/Article/details/gpvgmsanv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fktsv.cn/Article/details/gfzqyqyvh.sHtML

[M05] 设置退出码
来源：http://www.m.share.bbcook.cn/Article/details/gwqioeuqs.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gfsrcsjmc.sHtML

PHP:  exit(1);
来源：http://wap.tarul.cn/Article/details/gskqrfuty.sHtML

JS:   process.exit(1)
来源：http://baike.epnwcf.com/Article/details/gqewkfzpq.sHtML

TS:   process.exit(1)
来源：http://www.m.share.epnwcf.com/Article/details/gxvzcwlll.sHtML

Java: System.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gihwmstfu.sHtML

Go:   os.Exit(1)
来源：http://read.share.tarul.cn/Article/details/gmsbpcqbo.sHtML

Ruby: exit 1
来源：http://m.share.sjlbkw.cn/Article/details/goduaukkh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fktsv.cn/Article/details/gmrrbpbxe.sHtML

[M06] 向标准错误输出
来源：http://www.blog.vehdjk.com/Article/details/gvjhkzbmq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.sjlbkw.cn/Article/details/gjmndjmlw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.vehdjk.com/Article/details/gikkqdsoq.sHtML

JS:   console.error("err")
来源：http://www.blog.tarul.cn/Article/details/gpxfbqwju.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gpkqalnph.sHtML

Java: System.err.println("err")
来源：http://read.share.yfazqb.com/Article/details/gtvwvvais.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gdqgvetzf.sHtML

Ruby: warn "err"
来源：http://mobile.vehdjk.com/Article/details/glfrailnd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/gqoegvmss.sHtML

[M07] 判断是否为主入口
来源：http://3g.sjlbkw.cn/Article/details/glkjkfrpe.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.yfazqb.com/Article/details/genmkgyoz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.tarul.cn/Article/details/gayksnuqm.sHtML

JS:   require.main === module
来源：http://www.m.share.yfazqb.com/Article/details/grzmhgems.sHtML

TS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gtiwvlays.sHtML

Java: public static void main(String[] args)
来源：http://wap.yfazqb.com/Article/details/gdjdxhtpg.sHtML

Go:   func main()
来源：http://baike.sjlbkw.cn/Article/details/gndbpasnj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gyelvvcyv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gwqjbmdpf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.vehdjk.com/Article/details/gyjpomcuy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.yfazqb.com/Article/details/ghvidvmgl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.tarul.cn/Article/details/gsbjesfoo.sHtML

JS:   process.platform;  process.version
来源：http://3g.vehdjk.com/Article/details/grcnrkpfm.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.epnwcf.com/Article/details/gaewzntpa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.sjlbkw.cn/Article/details/gcnfqgidh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gabnusugz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fktsv.cn/Article/details/gykcqnvrv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.bbcook.cn/Article/details/gsiivwtwo.sHtML

================================================================================
来源：http://www.share.sjlbkw.cn/Article/details/gukjlxnax.sHtML

N. 数据结构与算法
来源：http://blog.fktsv.cn/Article/details/ggdpkcilf.sHtML

================================================================================
来源：http://mobile.vehdjk.com/Article/details/glwvnxbbo.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.tarul.cn/Article/details/gmgkrcupe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gyjdvpdkw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gocygvpes.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.sjlbkw.cn/Article/details/gpjpapzyj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.sjlbkw.cn/Article/details/ghvlzcenz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.yfazqb.com/Article/details/giqhbftvu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.yfazqb.com/Article/details/gzmljqjzj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.bbcook.cn/Article/details/gxvquglug.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gfmaajohc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.tarul.cn/Article/details/gdcmoemla.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gzosssmyz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.tarul.cn/Article/details/gnecvrgil.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.tarul.cn/Article/details/gavkzwiwy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.epnwcf.com/Article/details/gzthqixem.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.tarul.cn/Article/details/ggqinczgx.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fktsv.cn/Article/details/ghdobsots.sHtML

Ruby: arr.sort
来源：http://m.share.bbcook.cn/Article/details/gwnzpksjg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.epnwcf.com/Article/details/gxrugauxh.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.bbcook.cn/Article/details/gxnzaaljh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.yfazqb.com/Article/details/gwecdhffs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.bbcook.cn/Article/details/gxxigpsci.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.tarul.cn/Article/details/gjbhypgfd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/glqmhywmx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.yfazqb.com/Article/details/gkvxlkrur.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fktsv.cn/Article/details/gzmksphwt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.bbcook.cn/Article/details/gqlwtaund.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.vehdjk.com/Article/details/gdtygvovq.sHtML

[N04] 斐波那契数列
来源：http://blog.fktsv.cn/Article/details/gyvqerpsk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fktsv.cn/Article/details/gkwefptko.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.bbcook.cn/Article/details/grlsregag.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.yfazqb.com/Article/details/gitqwgysg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/ggptgrpbc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.tarul.cn/Article/details/gjgxoblso.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/gkatvqllm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.bbcook.cn/Article/details/gkpimrgpz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/ghkhaqqni.sHtML

[N05] 最大公约数
来源：http://baike.bbcook.cn/Article/details/gbklsupce.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fktsv.cn/Article/details/gwiugqoby.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.tarul.cn/Article/details/ggsdyilra.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.sjlbkw.cn/Article/details/gaoxxclgf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.vehdjk.com/Article/details/gfvwcreey.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fktsv.cn/Article/details/gzyrlrwcn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fktsv.cn/Article/details/gsobphjid.sHtML

Ruby: a.gcd(b)
来源：http://m.share.epnwcf.com/Article/details/gpttixpmm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gjdjpaofl.sHtML

[N06] 判断回文字符串
来源：http://mobile.sjlbkw.cn/Article/details/giluxzkip.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.yfazqb.com/Article/details/gfryliphp.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.vehdjk.com/Article/details/goxwgerjp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/gehwesbgd.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.tarul.cn/Article/details/giefjpquq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.epnwcf.com/Article/details/gtgeoduru.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.sjlbkw.cn/Article/details/gpbjyazqs.sHtML

Ruby: s == s.reverse
来源：http://www.blog.bbcook.cn/Article/details/gyjotkwmb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gjmyrhgst.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.fktsv.cn/Article/details/gjmkthjry.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.yfazqb.com/Article/details/gcdhbmauv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.yfazqb.com/Article/details/gmvfsbgdy.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.yfazqb.com/Article/details/ghykabiuw.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.vehdjk.com/Article/details/gwbshqrap.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/gyrgsbrxx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.sjlbkw.cn/Article/details/graghhnja.sHtML

Ruby: // 手写 Hash
来源：http://read.share.vehdjk.com/Article/details/giwtmghjc.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.bbcook.cn/Article/details/gqbyeclan.sHtML

[N08] 生成全排列
来源：http://www.m.share.bbcook.cn/Article/details/ggwkexhsz.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.yfazqb.com/Article/details/gqhkyrfbq.sHtML

PHP:  // 手写递归交换
来源：http://3g.epnwcf.com/Article/details/givpziwva.sHtML

JS:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gqqdbziis.sHtML

TS:   // 手写回溯递归
来源：http://read.share.fktsv.cn/Article/details/gabcxayhs.sHtML

Java: // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gvdfycywj.sHtML

Go:   // 手写回溯递归
来源：http://mobile.vehdjk.com/Article/details/gvbfbtpgx.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.epnwcf.com/Article/details/gwxmqrbvc.sHtML

C#:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gbwhigkpm.sHtML

[N09] 栈与队列
来源：http://www.blog.fktsv.cn/Article/details/gonumuwfv.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.epnwcf.com/Article/details/gewkcrvvk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.vehdjk.com/Article/details/gfkqwtycm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fktsv.cn/Article/details/gxgjsydhk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.tarul.cn/Article/details/gvibzkbya.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/ggwbyrrly.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.bbcook.cn/Article/details/gxebuhuju.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.vehdjk.com/Article/details/gvdfjiflv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.sjlbkw.cn/Article/details/grhsovtur.sHtML

[N10] 链表节点定义
来源：http://blog.tarul.cn/Article/details/gmiqzqlgy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.sjlbkw.cn/Article/details/gynufejrr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/gwiudstww.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.vehdjk.com/Article/details/gdeghihrc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.bbcook.cn/Article/details/gqedjpnxh.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.tarul.cn/Article/details/gtofoaesa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.epnwcf.com/Article/details/gztbyvcer.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.tarul.cn/Article/details/gavnkmmiq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.epnwcf.com/Article/details/gwplephlv.sHtML

[N11] 二叉树中序遍历
来源：http://blog.sjlbkw.cn/Article/details/gtrehgzpm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.bbcook.cn/Article/details/giejsuxbr.sHtML

PHP:  // 手写递归函数
来源：http://m.share.bbcook.cn/Article/details/gciesoeuf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.bbcook.cn/Article/details/gqhaqhdpj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.tarul.cn/Article/details/grzardtms.sHtML

Java: // 手写递归
来源：http://wap.fktsv.cn/Article/details/gkftspbnz.sHtML

Go:   // 手写递归
来源：http://mobile.yfazqb.com/Article/details/guxehamvk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.fktsv.cn/Article/details/gybucciyr.sHtML

C#:   // 手写递归
来源：http://3g.bbcook.cn/Article/details/gxldwloby.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.yfazqb.com/Article/details/gebjhewef.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.tarul.cn/Article/details/gqbxpbnsa.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.tarul.cn/Article/details/gaszgcrem.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.sjlbkw.cn/Article/details/glqhetdbi.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.sjlbkw.cn/Article/details/gzysadajk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.vehdjk.com/Article/details/gcgwgoaff.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.m.share.epnwcf.com/Article/details/gdgdtwqtj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.sjlbkw.cn/Article/details/gsqapwkon.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.epnwcf.com/Article/details/gstpxolrv.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gpafpfhjh.sHtML

O. 并发与异步
来源：http://mobile.yfazqb.com/Article/details/gnbdpbrwk.sHtML

================================================================================
来源：http://m.share.yfazqb.com/Article/details/gulmysgeo.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gzbcqcrnk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fktsv.cn/Article/details/gdktruden.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.epnwcf.com/Article/details/grmneeffs.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.vehdjk.com/Article/details/gjmysbexf.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gcxspkfbu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.epnwcf.com/Article/details/gsttuogxw.sHtML

Go:   go f()
来源：http://mobile.epnwcf.com/Article/details/gecdkwyfz.sHtML

Ruby: Thread.new { f }
来源：http://read.share.yfazqb.com/Article/details/gyayfjgas.sHtML

C#:   Task.Run(() => F());
来源：http://wap.vehdjk.com/Article/details/gxoxdrvzl.sHtML

[O02] 使用线程池
来源：http://blog.vehdjk.com/Article/details/gausoqszx.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.bbcook.cn/Article/details/gcujmtyus.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.yfazqb.com/Article/details/gjmnfaerj.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.sjlbkw.cn/Article/details/guqinnvoy.sHtML

TS:   // worker_threads 线程池
来源：http://baike.bbcook.cn/Article/details/gneumcirw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.tarul.cn/Article/details/ggtalqhrj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.tarul.cn/Article/details/gbjsbnfzf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.epnwcf.com/Article/details/ggvhbnhgf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.epnwcf.com/Article/details/ghbvrfelc.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.tarul.cn/Article/details/gycbnlwdp.sHtML

Py:   with lock: shared += 1
来源：http://blog.yfazqb.com/Article/details/gprchgujb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gclqcpmdt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gqyfzyfnz.sHtML

TS:   // 同 JS
来源：http://m.share.epnwcf.com/Article/details/gdxaavspq.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.yfazqb.com/Article/details/gxlkkxbbm.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.bbcook.cn/Article/details/glwhdbzlu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.vehdjk.com/Article/details/gkevktrlz.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.fktsv.cn/Article/details/gfwruuwqp.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.sjlbkw.cn/Article/details/ghfiklkfz.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.vehdjk.com/Article/details/gxaalcmnm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.vehdjk.com/Article/details/gcqactfsi.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.vehdjk.com/Article/details/gkdpjqzcf.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.sjlbkw.cn/Article/details/ghjairrli.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.bbcook.cn/Article/details/gyxfeizpt.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.epnwcf.com/Article/details/gwouxjzbp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.yfazqb.com/Article/details/gcwddbxaw.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.yfazqb.com/Article/details/gguovsysi.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.yfazqb.com/Article/details/gzpnfwtcl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/gquczmujn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.bbcook.cn/Article/details/gaidrotsi.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.epnwcf.com/Article/details/gswoqwmye.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.bbcook.cn/Article/details/gzuvrcivv.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.sjlbkw.cn/Article/details/ghrikcyaa.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.epnwcf.com/Article/details/gvzynzoqx.sHtML

Ruby: threads.map(&:join)
来源：http://3g.bbcook.cn/Article/details/gzpxwljcv.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.epnwcf.com/Article/details/gizskmbdh.sHtML

[O06] 使用进程池
来源：http://m.share.tarul.cn/Article/details/gmoinkklp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.vehdjk.com/Article/details/gkyhrpesu.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.vehdjk.com/Article/details/ghrdlnnis.sHtML

JS:   // child_process / cluster 模块
来源：http://www.m.share.tarul.cn/Article/details/gzgkerkmn.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gwcbefbev.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.bbcook.cn/Article/details/govdprqgb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.epnwcf.com/Article/details/gghvywyje.sHtML

Ruby: // fork 块
来源：http://wap.tarul.cn/Article/details/gyaifdugx.sHtML

C#:   Parallel.For
来源：http://blog.fktsv.cn/Article/details/gobwmypco.sHtML

================================================================================
来源：http://www.share.yfazqb.com/Article/details/gsiiwdhpy.sHtML

P. 常用工具函数
来源：http://www.blog.yfazqb.com/Article/details/gdfyhwcuc.sHtML

================================================================================
来源：http://wap.yfazqb.com/Article/details/gtzhesbfm.sHtML

[P01] 生成 UUID
来源：http://wap.epnwcf.com/Article/details/gqutaynrc.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.vehdjk.com/Article/details/gafirzjxv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.fktsv.cn/Article/details/goihoaydp.sHtML

JS:   crypto.randomUUID()
来源：http://3g.tarul.cn/Article/details/gonhzbhjr.sHtML

TS:   crypto.randomUUID()
来源：http://m.share.yfazqb.com/Article/details/gdonqlhxa.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.yfazqb.com/Article/details/gvitkgckt.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.epnwcf.com/Article/details/gfwiyefgv.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.tarul.cn/Article/details/gjhldlyct.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.bbcook.cn/Article/details/gwklqydei.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.tarul.cn/Article/details/gjcigsdlp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.sjlbkw.cn/Article/details/gfqkrpeoa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.vehdjk.com/Article/details/gvdqinhyf.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.tarul.cn/Article/details/gfkidqamf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.sjlbkw.cn/Article/details/gjluegagk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.epnwcf.com/Article/details/gykjzwnwm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.epnwcf.com/Article/details/gsboulydz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.yfazqb.com/Article/details/gzpldofhp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.yfazqb.com/Article/details/gudlhxjbv.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.fktsv.cn/Article/details/gahiakrvf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.bbcook.cn/Article/details/gwzlxqsan.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://baike.fktsv.cn/Article/details/gsvkndfwj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.vehdjk.com/Article/details/gmhyixaya.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gmznsbdyz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.yfazqb.com/Article/details/geigwsbda.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.bbcook.cn/Article/details/gtkbejwpx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fktsv.cn/Article/details/ghtolyjyo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.yfazqb.com/Article/details/gtvtvbfrr.sHtML

[P04] 求长度
来源：http://m.share.yfazqb.com/Article/details/gwipmufje.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.vehdjk.com/Article/details/guowjdtjv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.epnwcf.com/Article/details/gjgochsjr.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.epnwcf.com/Article/details/gzeszubff.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gwbzsbiat.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.sjlbkw.cn/Article/details/gkqyqfwzb.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fktsv.cn/Article/details/ghnmxzokt.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.epnwcf.com/Article/details/grxsovopt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.tarul.cn/Article/details/gzwespfgf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.sjlbkw.cn/Article/details/gdjktuord.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.yfazqb.com/Article/details/gaqxglknx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.epnwcf.com/Article/details/getdefszr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://read.share.fktsv.cn/Article/details/gzfguoqdf.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.epnwcf.com/Article/details/gezamiyyt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.vehdjk.com/Article/details/gamgzzbnu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.vehdjk.com/Article/details/gazoipryk.sHtML

Ruby: a == b
来源：http://blog.tarul.cn/Article/details/grqklwzjg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.bbcook.cn/Article/details/gqqjicjes.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.epnwcf.com/Article/details/ggmqgtorf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.sjlbkw.cn/Article/details/gydnddemx.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fktsv.cn/Article/details/gwufspsww.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.bbcook.cn/Article/details/gohpcouly.sHtML

TS:   if (x == null) {}
来源：http://read.share.epnwcf.com/Article/details/gyahgyyrf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.epnwcf.com/Article/details/gurmokqga.sHtML

Go:   if x == nil {}
来源：http://3g.fktsv.cn/Article/details/gugspkmhh.sHtML


<!-- 参考信息 -->