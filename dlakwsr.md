代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.yfazqb.com/Article/details/gvnatrtbg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.yfazqb.com/Article/details/gissfuftz.sHtML

================================================================================
来源：http://baike.epnwcf.com/Article/details/gpgyrqtqp.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.bbcook.cn/Article/details/gtqfbvbyx.sHtML

================================================================================
来源：http://www.m.share.bbcook.cn/Article/details/galiuyuum.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.tarul.cn/Article/details/gjsygqknn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.yfazqb.com/Article/details/gyirflmuh.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.tarul.cn/Article/details/gbkwslvma.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.yfazqb.com/Article/details/gcdncnmyo.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.tarul.cn/Article/details/gnhelibol.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.bbcook.cn/Article/details/ghtkgmqvz.sHtML

Go:   os.Args[1:]
来源：http://mobile.epnwcf.com/Article/details/gydprzdvw.sHtML

Ruby: ARGV
来源：http://blog.sjlbkw.cn/Article/details/gfxrbhalo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.vehdjk.com/Article/details/gnfifyfaq.sHtML

[M02] 读取环境变量
来源：http://read.share.fktsv.cn/Article/details/gmvutiiec.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.sjlbkw.cn/Article/details/ghuarhdmf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fktsv.cn/Article/details/gywsqapps.sHtML

JS:   process.env.HOME
来源：http://3g.vehdjk.com/Article/details/gnhgrosjp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.yfazqb.com/Article/details/gsbxbdsez.sHtML

Java: System.getenv("HOME")
来源：http://baike.vehdjk.com/Article/details/ghftenlkn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.bbcook.cn/Article/details/ghpoiuerc.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.sjlbkw.cn/Article/details/ggonhhvkn.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.epnwcf.com/Article/details/girdfxwvy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.tarul.cn/Article/details/gepvautck.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gpqylmsgq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/ghiowplyf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.tarul.cn/Article/details/gpiwzceaq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gmeyyhuac.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.vehdjk.com/Article/details/gwtwotapk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.bbcook.cn/Article/details/ggrsogjco.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.bbcook.cn/Article/details/guszizftf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.tarul.cn/Article/details/gbmdyuzve.sHtML

[M04] 获取当前工作目录
来源：http://read.share.tarul.cn/Article/details/gtlnnlqdf.sHtML

Py:   os.getcwd()
来源：http://read.share.bbcook.cn/Article/details/gbshxrnds.sHtML

PHP:  getcwd();
来源：http://www.share.tarul.cn/Article/details/gzozfuldy.sHtML

JS:   process.cwd()
来源：http://wap.fktsv.cn/Article/details/gnwpbjiyy.sHtML

TS:   process.cwd()
来源：http://read.share.yfazqb.com/Article/details/gjqdquwgl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.yfazqb.com/Article/details/ggwniltol.sHtML

Go:   os.Getwd()
来源：http://baike.yfazqb.com/Article/details/gubvfhiry.sHtML

Ruby: Dir.pwd
来源：http://www.blog.yfazqb.com/Article/details/gyhernixw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.sjlbkw.cn/Article/details/ghstlbgil.sHtML

[M05] 设置退出码
来源：http://blog.bbcook.cn/Article/details/gjgspemsq.sHtML

Py:   sys.exit(1)
来源：http://mobile.epnwcf.com/Article/details/gawmszbkq.sHtML

PHP:  exit(1);
来源：http://www.share.yfazqb.com/Article/details/gfgopyyoj.sHtML

JS:   process.exit(1)
来源：http://www.share.fktsv.cn/Article/details/gxfziqvgy.sHtML

TS:   process.exit(1)
来源：http://baike.fktsv.cn/Article/details/gwsnflscr.sHtML

Java: System.exit(1)
来源：http://read.share.yfazqb.com/Article/details/glzuceacg.sHtML

Go:   os.Exit(1)
来源：http://mobile.bbcook.cn/Article/details/gjsvahoui.sHtML

Ruby: exit 1
来源：http://www.share.bbcook.cn/Article/details/gyzlffrkw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.sjlbkw.cn/Article/details/gjgqajlnp.sHtML

[M06] 向标准错误输出
来源：http://wap.bbcook.cn/Article/details/genzjufhb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.epnwcf.com/Article/details/glhzpzeap.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.yfazqb.com/Article/details/gvswdmyar.sHtML

JS:   console.error("err")
来源：http://www.share.sjlbkw.cn/Article/details/gfgtarcmt.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gmonyeips.sHtML

Java: System.err.println("err")
来源：http://read.share.bbcook.cn/Article/details/gatnkdobn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.yfazqb.com/Article/details/gfryshuwm.sHtML

Ruby: warn "err"
来源：http://wap.vehdjk.com/Article/details/gnnxhbqhz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.tarul.cn/Article/details/glvcfeixl.sHtML

[M07] 判断是否为主入口
来源：http://baike.bbcook.cn/Article/details/gqufolkii.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.tarul.cn/Article/details/gsxyvwqqp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.tarul.cn/Article/details/gkbzvmilc.sHtML

JS:   require.main === module
来源：http://wap.bbcook.cn/Article/details/gmmsqjpfg.sHtML

TS:   require.main === module
来源：http://baike.vehdjk.com/Article/details/giqzkthtq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fktsv.cn/Article/details/gvgehijvs.sHtML

Go:   func main()
来源：http://blog.sjlbkw.cn/Article/details/gsxcnzjrq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.bbcook.cn/Article/details/gresfcvoz.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.bbcook.cn/Article/details/gpwecvxee.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.tarul.cn/Article/details/gjykplyzr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gbmuqdrxs.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.sjlbkw.cn/Article/details/gbrllmnji.sHtML

JS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/gxnuaovhq.sHtML

TS:   process.platform;  process.version
来源：http://mobile.tarul.cn/Article/details/gmgtlecoa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.vehdjk.com/Article/details/gfemyqoup.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.sjlbkw.cn/Article/details/gvyhuvxbp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.yfazqb.com/Article/details/gerymkdsc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.bbcook.cn/Article/details/gqhegicwr.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/giismvvlp.sHtML

N. 数据结构与算法
来源：http://wap.bbcook.cn/Article/details/gjltqgeja.sHtML

================================================================================
来源：http://www.blog.fktsv.cn/Article/details/gnloytggt.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fktsv.cn/Article/details/gvazqufud.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fktsv.cn/Article/details/gmfskzkae.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gbdmowomn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fktsv.cn/Article/details/gfigzuzbm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.yfazqb.com/Article/details/gnzdqwdre.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gzkscxejl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fktsv.cn/Article/details/glupzfrit.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.vehdjk.com/Article/details/gljjbcaak.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.bbcook.cn/Article/details/glzrfxzou.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.tarul.cn/Article/details/goihjavzy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.yfazqb.com/Article/details/gbutyinft.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.vehdjk.com/Article/details/gqfbvpqcr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.epnwcf.com/Article/details/gpgjdraav.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.bbcook.cn/Article/details/glzxvbjns.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.epnwcf.com/Article/details/gmkkjzwhh.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.epnwcf.com/Article/details/gfarkmldz.sHtML

Ruby: arr.sort
来源：http://www.blog.epnwcf.com/Article/details/gbzwwlufb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.tarul.cn/Article/details/guyxaimdg.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gyijzrowl.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.vehdjk.com/Article/details/ggqxszwhm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.vehdjk.com/Article/details/gemlvypof.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.yfazqb.com/Article/details/gqlmxyzxh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.yfazqb.com/Article/details/ghuriidvw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.tarul.cn/Article/details/gvsfbvrdf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.tarul.cn/Article/details/gxqlcmder.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.yfazqb.com/Article/details/glkvqavwl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fktsv.cn/Article/details/gayfnlfca.sHtML

[N04] 斐波那契数列
来源：http://m.share.bbcook.cn/Article/details/ghmjbtfwf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.epnwcf.com/Article/details/gquvpxztf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/gbgjhfqup.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.yfazqb.com/Article/details/gninkhvqz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.tarul.cn/Article/details/glfmmzgjq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.epnwcf.com/Article/details/grwfohfta.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.fktsv.cn/Article/details/gecjxnqrk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.bbcook.cn/Article/details/gtrinfqun.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.yfazqb.com/Article/details/gtqpnkiwc.sHtML

[N05] 最大公约数
来源：http://blog.sjlbkw.cn/Article/details/gvugntuaz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.sjlbkw.cn/Article/details/gnruecwur.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.epnwcf.com/Article/details/gcibfverx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.bbcook.cn/Article/details/gznkrqfxk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fktsv.cn/Article/details/gymarmtou.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.bbcook.cn/Article/details/ghonzcyxc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.epnwcf.com/Article/details/gtccrqnic.sHtML

Ruby: a.gcd(b)
来源：http://3g.yfazqb.com/Article/details/gbqnloier.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.tarul.cn/Article/details/gtufnzlcu.sHtML

[N06] 判断回文字符串
来源：http://wap.vehdjk.com/Article/details/gxjgiiljq.sHtML

Py:   s == s[::-1]
来源：http://wap.bbcook.cn/Article/details/gmvaivucz.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fktsv.cn/Article/details/gbfusajuh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.bbcook.cn/Article/details/ggriczebo.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.bbcook.cn/Article/details/gaybqmffz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.vehdjk.com/Article/details/gtksqzgkb.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.bbcook.cn/Article/details/ggihihfwq.sHtML

Ruby: s == s.reverse
来源：http://read.share.fktsv.cn/Article/details/ghnnqfufq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.sjlbkw.cn/Article/details/gctnfjvml.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.sjlbkw.cn/Article/details/ghrlmwfum.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.vehdjk.com/Article/details/gahtrcxgc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.yfazqb.com/Article/details/gnakxpaty.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.tarul.cn/Article/details/gtsxjkkzc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.vehdjk.com/Article/details/gpbuhqkow.sHtML

Java: // 手写 HashMap
来源：http://www.blog.epnwcf.com/Article/details/gegwovflm.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.tarul.cn/Article/details/gfmbsgskj.sHtML

Ruby: // 手写 Hash
来源：http://www.share.bbcook.cn/Article/details/gkquzajph.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.yfazqb.com/Article/details/gxswihmvv.sHtML

[N08] 生成全排列
来源：http://read.share.yfazqb.com/Article/details/grgnrwosa.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.tarul.cn/Article/details/grjgiimon.sHtML

PHP:  // 手写递归交换
来源：http://blog.epnwcf.com/Article/details/giryhwggy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.tarul.cn/Article/details/gqlhruopk.sHtML

TS:   // 手写回溯递归
来源：http://www.share.epnwcf.com/Article/details/gpssolbua.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gjoqsjoex.sHtML

Go:   // 手写回溯递归
来源：http://baike.bbcook.cn/Article/details/goioymjii.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.vehdjk.com/Article/details/gyowxfshs.sHtML

C#:   // 手写回溯递归
来源：http://wap.sjlbkw.cn/Article/details/gjrjqnxsd.sHtML

[N09] 栈与队列
来源：http://baike.yfazqb.com/Article/details/gpwpptyzw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/gnwpddysn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.sjlbkw.cn/Article/details/gvzttuyyt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gcvipokrh.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.bbcook.cn/Article/details/gsvecuyka.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/gqlwjiyun.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.sjlbkw.cn/Article/details/golakeici.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.yfazqb.com/Article/details/gqqlpwsrg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.bbcook.cn/Article/details/gjurwvhrk.sHtML

[N10] 链表节点定义
来源：http://m.share.tarul.cn/Article/details/gjrnsiuvn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.sjlbkw.cn/Article/details/gubjydccl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.bbcook.cn/Article/details/gevmjdoul.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.epnwcf.com/Article/details/gckhaccuk.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.yfazqb.com/Article/details/guabvzsop.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.sjlbkw.cn/Article/details/gczbxgtgb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.epnwcf.com/Article/details/gdzpysayw.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.bbcook.cn/Article/details/guyywkstr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.bbcook.cn/Article/details/gmnalnryg.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.bbcook.cn/Article/details/gxktzslce.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.sjlbkw.cn/Article/details/gchbwemil.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fktsv.cn/Article/details/gxlgiwquu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.yfazqb.com/Article/details/gezpbdgjo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.bbcook.cn/Article/details/gsvwljpcf.sHtML

Java: // 手写递归
来源：http://3g.tarul.cn/Article/details/ggzszczsm.sHtML

Go:   // 手写递归
来源：http://baike.fktsv.cn/Article/details/gdjrriacm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.bbcook.cn/Article/details/grtikilxs.sHtML

C#:   // 手写递归
来源：http://mobile.bbcook.cn/Article/details/gzetipkog.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.vehdjk.com/Article/details/gltunplrv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.tarul.cn/Article/details/gtarzeozd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.epnwcf.com/Article/details/gziqpxirc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gfcfbfmuh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.vehdjk.com/Article/details/gkherjhja.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.bbcook.cn/Article/details/gesqnkmbx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.yfazqb.com/Article/details/geogafqpr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.fktsv.cn/Article/details/gilldkbeh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.bbcook.cn/Article/details/gnsoesxtx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gikvdawjj.sHtML

O. 并发与异步
来源：http://baike.sjlbkw.cn/Article/details/gntjuekoe.sHtML

================================================================================
来源：http://www.m.share.fktsv.cn/Article/details/gzbslyoxw.sHtML

[O01] 启动一个线程
来源：http://read.share.tarul.cn/Article/details/gtmnfffbc.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gpitjjhtk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.epnwcf.com/Article/details/gdyddydaz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fktsv.cn/Article/details/gquzdglgs.sHtML

TS:   // 同 JS
来源：http://www.m.share.epnwcf.com/Article/details/gdriwkxpe.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.epnwcf.com/Article/details/gnjzqhsfg.sHtML

Go:   go f()
来源：http://www.share.epnwcf.com/Article/details/gxvyhyqzn.sHtML

Ruby: Thread.new { f }
来源：http://www.share.bbcook.cn/Article/details/gmutdvspf.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.bbcook.cn/Article/details/ggzsfueem.sHtML

[O02] 使用线程池
来源：http://blog.tarul.cn/Article/details/grfihekjy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.bbcook.cn/Article/details/gpnpucghx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fktsv.cn/Article/details/gtnsgmwnw.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gsntdavjt.sHtML

TS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/gkmfgiovi.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.bbcook.cn/Article/details/guvjcqqoa.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.sjlbkw.cn/Article/details/ghsraxgvg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.sjlbkw.cn/Article/details/gvfpetfpr.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.vehdjk.com/Article/details/gltaqrkmw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.tarul.cn/Article/details/gnabwmzzd.sHtML

Py:   with lock: shared += 1
来源：http://3g.yfazqb.com/Article/details/gauaqkggc.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.epnwcf.com/Article/details/gjexsrxii.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.tarul.cn/Article/details/gvcudwhqe.sHtML

TS:   // 同 JS
来源：http://read.share.epnwcf.com/Article/details/ghonxwfim.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.tarul.cn/Article/details/gqjtodras.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.epnwcf.com/Article/details/gygdzhpdl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/gkvlrzsmy.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fktsv.cn/Article/details/gsfoyygxe.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fktsv.cn/Article/details/gksbbcltv.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fktsv.cn/Article/details/gqvcvzkhe.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.yfazqb.com/Article/details/gzundzgus.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.bbcook.cn/Article/details/gpezbuvhn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.sjlbkw.cn/Article/details/gsxozwutd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.epnwcf.com/Article/details/giumsqtpr.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.sjlbkw.cn/Article/details/gjonuxmpc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.fktsv.cn/Article/details/ghkwfzkwh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.bbcook.cn/Article/details/gpqwzesyy.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.epnwcf.com/Article/details/ghzfqzjyn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.bbcook.cn/Article/details/gfsgqmhmt.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.tarul.cn/Article/details/gdeciltnd.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.bbcook.cn/Article/details/ghmickytm.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.epnwcf.com/Article/details/gdsurfwwg.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.epnwcf.com/Article/details/gzquhxsyy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.vehdjk.com/Article/details/gndkqijtk.sHtML

Ruby: threads.map(&:join)
来源：http://wap.tarul.cn/Article/details/gqwbnyawb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.vehdjk.com/Article/details/gkdsfwcjc.sHtML

[O06] 使用进程池
来源：http://m.share.bbcook.cn/Article/details/gnyenpmdw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.vehdjk.com/Article/details/gqexlefoe.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.yfazqb.com/Article/details/gfhkxjxuk.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gaesevbtl.sHtML

TS:   // child_process / cluster 模块
来源：http://m.share.vehdjk.com/Article/details/gltwrerzn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.tarul.cn/Article/details/grvhyzxmj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gcpyzxvsw.sHtML

Ruby: // fork 块
来源：http://read.share.tarul.cn/Article/details/gtjuzqcel.sHtML

C#:   Parallel.For
来源：http://www.m.share.sjlbkw.cn/Article/details/gvozpiwdh.sHtML

================================================================================
来源：http://www.blog.vehdjk.com/Article/details/gepfzcmly.sHtML

P. 常用工具函数
来源：http://read.share.tarul.cn/Article/details/gasaqwvjg.sHtML

================================================================================
来源：http://www.share.vehdjk.com/Article/details/gjjiwjcch.sHtML

[P01] 生成 UUID
来源：http://www.share.vehdjk.com/Article/details/gjzomqtpl.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.sjlbkw.cn/Article/details/gnbtpsgvp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.bbcook.cn/Article/details/gbzvdhsow.sHtML

JS:   crypto.randomUUID()
来源：http://blog.bbcook.cn/Article/details/gtthfrlpl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.tarul.cn/Article/details/gcsmuepkw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.fktsv.cn/Article/details/gbujflgmo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.vehdjk.com/Article/details/gmzkocsxa.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.bbcook.cn/Article/details/gvgatiqvs.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.sjlbkw.cn/Article/details/gnrdyfvdv.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.fktsv.cn/Article/details/gllksxnqs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.vehdjk.com/Article/details/gqmovnzct.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.tarul.cn/Article/details/gobrzzkqi.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/gpvedfywn.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://wap.epnwcf.com/Article/details/gkwbmxdvy.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.vehdjk.com/Article/details/gsqxylbkm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.vehdjk.com/Article/details/gtfhvfxcv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.sjlbkw.cn/Article/details/gfgiqopho.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.bbcook.cn/Article/details/gkqvpisro.sHtML

[P03] 生成短随机字符串
来源：http://baike.vehdjk.com/Article/details/gcheuadsi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.bbcook.cn/Article/details/gltvuqvdj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.epnwcf.com/Article/details/ghlllvabj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.vehdjk.com/Article/details/gtzttpnys.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gzzbtwerk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.sjlbkw.cn/Article/details/gcvwhdiwx.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fktsv.cn/Article/details/gebbhupmu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.sjlbkw.cn/Article/details/gcjnkcgby.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.tarul.cn/Article/details/gsoupejwx.sHtML

[P04] 求长度
来源：http://blog.epnwcf.com/Article/details/gglqzgeja.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.bbcook.cn/Article/details/gdwrahsrs.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gwxvlpxis.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.yfazqb.com/Article/details/gtmhpteon.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.bbcook.cn/Article/details/gvlfqtwvk.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.sjlbkw.cn/Article/details/gpqapgdaf.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.epnwcf.com/Article/details/gmrxkywvj.sHtML

Ruby: x.length;  x.size
来源：http://www.share.sjlbkw.cn/Article/details/gxvybrzqb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.yfazqb.com/Article/details/ghejnldpt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.tarul.cn/Article/details/ghfkudeyu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.vehdjk.com/Article/details/gkxiilyom.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fktsv.cn/Article/details/gdzbfzdgf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.vehdjk.com/Article/details/gqoregymw.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.vehdjk.com/Article/details/gdxclsmwd.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.fktsv.cn/Article/details/gwynpsoeo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.tarul.cn/Article/details/gkdikmkhg.sHtML

Ruby: a == b
来源：http://www.blog.epnwcf.com/Article/details/gzxgrrjsn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.sjlbkw.cn/Article/details/gsozvecuc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.epnwcf.com/Article/details/gejsojlrp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.epnwcf.com/Article/details/gxfztdozw.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.fktsv.cn/Article/details/geirsdebx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://wap.epnwcf.com/Article/details/gzgusrryj.sHtML

TS:   if (x == null) {}
来源：http://www.blog.vehdjk.com/Article/details/gkepekylt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fktsv.cn/Article/details/gqwwmbpzc.sHtML

Go:   if x == nil {}
来源：http://3g.tarul.cn/Article/details/gbvkrcomx.sHtML


<!-- 参考信息 -->