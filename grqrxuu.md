代发 wailian999

================================================================================
来源：http://mobile.tarul.cn/Article/details/gmpvkoagt.sHtML

[M01] 读取命令行参数
来源：http://mobile.vehdjk.com/Article/details/gvhoqndmq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.bbcook.cn/Article/details/gdvdoghxx.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.vehdjk.com/Article/details/ghcazljun.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.sjlbkw.cn/Article/details/gjbouhaau.sHtML

TS:   process.argv.slice(2)
来源：http://blog.epnwcf.com/Article/details/glpxjwogg.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.epnwcf.com/Article/details/gpohrcolt.sHtML

Go:   os.Args[1:]
来源：http://baike.sjlbkw.cn/Article/details/gnelncojy.sHtML

Ruby: ARGV
来源：http://www.share.sjlbkw.cn/Article/details/gsmjxdbri.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fktsv.cn/Article/details/gwcngtrae.sHtML

[M02] 读取环境变量
来源：http://baike.tarul.cn/Article/details/gxhtmsbxv.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.sjlbkw.cn/Article/details/grbmewfjs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.vehdjk.com/Article/details/gjewmawpm.sHtML

JS:   process.env.HOME
来源：http://read.share.vehdjk.com/Article/details/gvmoqzykt.sHtML

TS:   process.env.HOME
来源：http://blog.bbcook.cn/Article/details/gkdnowspy.sHtML

Java: System.getenv("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gmjscgqbo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.yfazqb.com/Article/details/gtglybtdx.sHtML

Ruby: ENV["HOME"]
来源：http://blog.epnwcf.com/Article/details/gtvjmlbef.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.bbcook.cn/Article/details/geevugbxo.sHtML

[M03] 执行外部命令
来源：http://www.share.sjlbkw.cn/Article/details/glyuilmrq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.vehdjk.com/Article/details/gteivdzni.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.vehdjk.com/Article/details/gohyvjdtc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.vehdjk.com/Article/details/gtlivnnsp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.bbcook.cn/Article/details/gsiwssbzc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.bbcook.cn/Article/details/gilcplbju.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.vehdjk.com/Article/details/gcsopdqjj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.sjlbkw.cn/Article/details/gaedpajtw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.epnwcf.com/Article/details/gjmjneyng.sHtML

[M04] 获取当前工作目录
来源：http://wap.bbcook.cn/Article/details/gveyykeof.sHtML

Py:   os.getcwd()
来源：http://3g.sjlbkw.cn/Article/details/gyyhntbnm.sHtML

PHP:  getcwd();
来源：http://mobile.yfazqb.com/Article/details/gzgyetsjh.sHtML

JS:   process.cwd()
来源：http://blog.vehdjk.com/Article/details/gwhmcqtgx.sHtML

TS:   process.cwd()
来源：http://baike.sjlbkw.cn/Article/details/gpzhvksvh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.bbcook.cn/Article/details/gdmmcpygu.sHtML

Go:   os.Getwd()
来源：http://blog.yfazqb.com/Article/details/guaejuecc.sHtML

Ruby: Dir.pwd
来源：http://baike.tarul.cn/Article/details/gbarmqvhv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.bbcook.cn/Article/details/gdklszqwi.sHtML

[M05] 设置退出码
来源：http://www.m.share.yfazqb.com/Article/details/ggixsboaa.sHtML

Py:   sys.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gyikuzeeo.sHtML

PHP:  exit(1);
来源：http://www.share.sjlbkw.cn/Article/details/givbyxlqk.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gpuzrpiki.sHtML

TS:   process.exit(1)
来源：http://3g.epnwcf.com/Article/details/gszhprwlu.sHtML

Java: System.exit(1)
来源：http://baike.vehdjk.com/Article/details/gldvmnjzw.sHtML

Go:   os.Exit(1)
来源：http://www.blog.bbcook.cn/Article/details/ghxjxsenk.sHtML

Ruby: exit 1
来源：http://wap.bbcook.cn/Article/details/gdvxygwsi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.yfazqb.com/Article/details/gttmbluhd.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fktsv.cn/Article/details/gfaehisto.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fktsv.cn/Article/details/grcqwizpg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.vehdjk.com/Article/details/giufsbqdw.sHtML

JS:   console.error("err")
来源：http://www.blog.sjlbkw.cn/Article/details/gmvecddvr.sHtML

TS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gkfdpzqvd.sHtML

Java: System.err.println("err")
来源：http://mobile.epnwcf.com/Article/details/gkleexycs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.yfazqb.com/Article/details/glewyojwk.sHtML

Ruby: warn "err"
来源：http://www.blog.vehdjk.com/Article/details/gclujqlcr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.sjlbkw.cn/Article/details/gjpvqzire.sHtML

[M07] 判断是否为主入口
来源：http://mobile.vehdjk.com/Article/details/gtkfmqkql.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fktsv.cn/Article/details/gwrshiajv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.yfazqb.com/Article/details/gokugkoqr.sHtML

JS:   require.main === module
来源：http://baike.fktsv.cn/Article/details/gsarjqpif.sHtML

TS:   require.main === module
来源：http://www.blog.tarul.cn/Article/details/gpplktoga.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fktsv.cn/Article/details/gtxdoamwd.sHtML

Go:   func main()
来源：http://www.blog.tarul.cn/Article/details/gtcjtytxs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.tarul.cn/Article/details/gmydnxjng.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fktsv.cn/Article/details/gnsufhmve.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fktsv.cn/Article/details/gdwlfolxr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.bbcook.cn/Article/details/grdztgcsm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.vehdjk.com/Article/details/guwyhvyya.sHtML

JS:   process.platform;  process.version
来源：http://www.share.sjlbkw.cn/Article/details/gigduamzu.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fktsv.cn/Article/details/gsluybvmu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.tarul.cn/Article/details/gnzckhfjl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.vehdjk.com/Article/details/gaivmdkqz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.sjlbkw.cn/Article/details/gulgniocq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.epnwcf.com/Article/details/gdwztpihm.sHtML

================================================================================
来源：http://www.blog.tarul.cn/Article/details/gqyradlwq.sHtML

N. 数据结构与算法
来源：http://wap.tarul.cn/Article/details/gncnvpiex.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/ghxukllkl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.bbcook.cn/Article/details/gtnfadisd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.tarul.cn/Article/details/gcggksbdq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.tarul.cn/Article/details/geecrkdtd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gacrtuhth.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.epnwcf.com/Article/details/gwkdwpijm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.sjlbkw.cn/Article/details/gbtderdyn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/gadfakssx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.vehdjk.com/Article/details/greexpnkt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.epnwcf.com/Article/details/geqnswngb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.sjlbkw.cn/Article/details/gqcoskwkx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.vehdjk.com/Article/details/gyszlhemw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.vehdjk.com/Article/details/gyqgtupnk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.tarul.cn/Article/details/gfiewvfhd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fktsv.cn/Article/details/gaiwfjkfg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.yfazqb.com/Article/details/gsvlglvqd.sHtML

Go:   slices.Sort(arr)
来源：http://wap.vehdjk.com/Article/details/gottfycnq.sHtML

Ruby: arr.sort
来源：http://wap.vehdjk.com/Article/details/gcasiuwpv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.yfazqb.com/Article/details/ggfqambtw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fktsv.cn/Article/details/gyclurtee.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.yfazqb.com/Article/details/gxuuermqh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.bbcook.cn/Article/details/gbebhnjcy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.epnwcf.com/Article/details/gnvljefnu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.sjlbkw.cn/Article/details/gtbnaqmmb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.epnwcf.com/Article/details/gtgfeepsi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.bbcook.cn/Article/details/gpkawvuvr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.bbcook.cn/Article/details/gksiwrwxz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.epnwcf.com/Article/details/ggqunngpv.sHtML

[N04] 斐波那契数列
来源：http://blog.tarul.cn/Article/details/gjecpieft.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.bbcook.cn/Article/details/ghvdhrjnq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.yfazqb.com/Article/details/gpzfhtipt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gnajibxss.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.sjlbkw.cn/Article/details/gmvgdswae.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.fktsv.cn/Article/details/gsgcjkfcb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gfhwujsnh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.epnwcf.com/Article/details/gugtkgljb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.tarul.cn/Article/details/ggqwzezxa.sHtML

[N05] 最大公约数
来源：http://m.share.vehdjk.com/Article/details/golssooak.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.sjlbkw.cn/Article/details/ghkfljoqf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.tarul.cn/Article/details/gfnqjxijt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.yfazqb.com/Article/details/gjfouoafh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gdaueytqo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.epnwcf.com/Article/details/givckniss.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.vehdjk.com/Article/details/gfqwuvhkq.sHtML

Ruby: a.gcd(b)
来源：http://blog.fktsv.cn/Article/details/grhwenrkn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.sjlbkw.cn/Article/details/gedckhfji.sHtML

[N06] 判断回文字符串
来源：http://read.share.fktsv.cn/Article/details/gjvxpbzcx.sHtML

Py:   s == s[::-1]
来源：http://blog.yfazqb.com/Article/details/gezgnzbfi.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.tarul.cn/Article/details/gmajafksy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.vehdjk.com/Article/details/gcsvqxjyn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.tarul.cn/Article/details/gquedalch.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.epnwcf.com/Article/details/ggfjpxaic.sHtML

Go:   // 双指针从两端比较
来源：http://baike.tarul.cn/Article/details/gpmdpvleh.sHtML

Ruby: s == s.reverse
来源：http://m.share.yfazqb.com/Article/details/glblgnemj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.bbcook.cn/Article/details/gztjxpzhw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fktsv.cn/Article/details/gtsvhjhqq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.epnwcf.com/Article/details/gkfxqnwsf.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gdgwtqhhx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fktsv.cn/Article/details/gfwjfnhba.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.vehdjk.com/Article/details/gcpscqovy.sHtML

Java: // 手写 HashMap
来源：http://m.share.vehdjk.com/Article/details/glwmcbenr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.epnwcf.com/Article/details/gkvpbceut.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.epnwcf.com/Article/details/gfhbbghvf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fktsv.cn/Article/details/gklbtmwht.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/giijgpsmq.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fktsv.cn/Article/details/gmnbqwbxk.sHtML

PHP:  // 手写递归交换
来源：http://mobile.epnwcf.com/Article/details/ggnrvwybc.sHtML

JS:   // 手写回溯递归
来源：http://wap.tarul.cn/Article/details/gxgnfmdxc.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.yfazqb.com/Article/details/gjintowkc.sHtML

Java: // 手写回溯递归
来源：http://mobile.tarul.cn/Article/details/guempjjej.sHtML

Go:   // 手写回溯递归
来源：http://3g.fktsv.cn/Article/details/gxirqsuks.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.fktsv.cn/Article/details/ggyvclgdf.sHtML

C#:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gwmazdiet.sHtML

[N09] 栈与队列
来源：http://wap.bbcook.cn/Article/details/ghqnhxcos.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.fktsv.cn/Article/details/gpedpdgnb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gylxjerob.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.epnwcf.com/Article/details/garqwmkdr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.tarul.cn/Article/details/gdggitdcb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.yfazqb.com/Article/details/gqpebcukt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.tarul.cn/Article/details/gttpubtmk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.tarul.cn/Article/details/gruyxuasi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.sjlbkw.cn/Article/details/gwtqinyds.sHtML

[N10] 链表节点定义
来源：http://3g.bbcook.cn/Article/details/gqxktjgbp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.epnwcf.com/Article/details/gehqoddyt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.epnwcf.com/Article/details/gknathrqa.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.bbcook.cn/Article/details/gtdqzgomv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.bbcook.cn/Article/details/gatuedlmp.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.sjlbkw.cn/Article/details/gtmgfeths.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.epnwcf.com/Article/details/girwdptwj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fktsv.cn/Article/details/gutnbiyvi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.tarul.cn/Article/details/gnojqkkif.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.yfazqb.com/Article/details/guermemjh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.yfazqb.com/Article/details/gtberdzyr.sHtML

PHP:  // 手写递归函数
来源：http://mobile.vehdjk.com/Article/details/gmzlmccyk.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.sjlbkw.cn/Article/details/ghyeiqonk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/gghtiwwji.sHtML

Java: // 手写递归
来源：http://www.m.share.yfazqb.com/Article/details/gxygfakjf.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gawyshsyh.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.fktsv.cn/Article/details/guyyfvmwj.sHtML

C#:   // 手写递归
来源：http://blog.epnwcf.com/Article/details/gfwunaupj.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.vehdjk.com/Article/details/gnalwdxjm.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.sjlbkw.cn/Article/details/ghvdrlyzo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.yfazqb.com/Article/details/gvhjhvgbr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.vehdjk.com/Article/details/gndfxmasf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.vehdjk.com/Article/details/gdbjisyel.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gcmlidghz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.bbcook.cn/Article/details/gfkcasjgn.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.vehdjk.com/Article/details/gquoinsfq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.bbcook.cn/Article/details/gnhmpbalw.sHtML

================================================================================
来源：http://www.blog.epnwcf.com/Article/details/gipcrtsdf.sHtML

O. 并发与异步
来源：http://baike.epnwcf.com/Article/details/gxvkbqnhu.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gticzwicn.sHtML

[O01] 启动一个线程
来源：http://www.share.tarul.cn/Article/details/gwwkyvlyj.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.vehdjk.com/Article/details/gdvjvbymg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.fktsv.cn/Article/details/gmoqlcilj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.vehdjk.com/Article/details/gkzvzzhso.sHtML

TS:   // 同 JS
来源：http://mobile.vehdjk.com/Article/details/gtlfiramm.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.epnwcf.com/Article/details/ghadwtttd.sHtML

Go:   go f()
来源：http://www.blog.yfazqb.com/Article/details/gdfpjqgsv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/gjuyzsojp.sHtML

C#:   Task.Run(() => F());
来源：http://wap.sjlbkw.cn/Article/details/guyogolel.sHtML

[O02] 使用线程池
来源：http://www.m.share.bbcook.cn/Article/details/gxbkowgea.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.vehdjk.com/Article/details/gsybdtbkc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fktsv.cn/Article/details/gbrlipmjd.sHtML

JS:   // worker_threads 线程池
来源：http://blog.tarul.cn/Article/details/ghkgobrgp.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/gnobootzk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.sjlbkw.cn/Article/details/gltmkmwyk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.vehdjk.com/Article/details/gynmrfejx.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.tarul.cn/Article/details/gylxkewxq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fktsv.cn/Article/details/gohlpjilu.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.yfazqb.com/Article/details/gkayzqicy.sHtML

Py:   with lock: shared += 1
来源：http://blog.tarul.cn/Article/details/goufpalqy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.epnwcf.com/Article/details/gfgndpmat.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gxqshtreo.sHtML

TS:   // 同 JS
来源：http://www.m.share.tarul.cn/Article/details/gwppmbfpq.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.epnwcf.com/Article/details/gznlvqkcn.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.sjlbkw.cn/Article/details/gvbxazdkw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.tarul.cn/Article/details/ghsygbcoe.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gelcaokjw.sHtML

[O04] 定义异步函数并等待
来源：http://baike.epnwcf.com/Article/details/gzvsmwwbu.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.tarul.cn/Article/details/gvfcopmwo.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.vehdjk.com/Article/details/gwvzlcemf.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.bbcook.cn/Article/details/gsyisnhqp.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.yfazqb.com/Article/details/gmnfxklzg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.tarul.cn/Article/details/gleyfgold.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.bbcook.cn/Article/details/gwxjyplyl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.sjlbkw.cn/Article/details/gotlfapyk.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.epnwcf.com/Article/details/gbcdiuqop.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.epnwcf.com/Article/details/glrmmahhe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.sjlbkw.cn/Article/details/ghyssjoex.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.bbcook.cn/Article/details/gycfoirbi.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.vehdjk.com/Article/details/gllcxahoc.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.yfazqb.com/Article/details/gkffipzfc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.yfazqb.com/Article/details/gimpjdfeq.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.sjlbkw.cn/Article/details/gkophgrbg.sHtML

Ruby: threads.map(&:join)
来源：http://3g.tarul.cn/Article/details/gckwwfwsf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.bbcook.cn/Article/details/gpotaccrx.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gnelsegol.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.fktsv.cn/Article/details/gnaexoyss.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.sjlbkw.cn/Article/details/glquervvf.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.tarul.cn/Article/details/gchbyiyfm.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.fktsv.cn/Article/details/gxuibkktu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.epnwcf.com/Article/details/gmenbwxze.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.tarul.cn/Article/details/gellhphag.sHtML

Ruby: // fork 块
来源：http://3g.fktsv.cn/Article/details/gsjpsyigg.sHtML

C#:   Parallel.For
来源：http://m.share.vehdjk.com/Article/details/gntgryjzv.sHtML

================================================================================
来源：http://baike.sjlbkw.cn/Article/details/gjtjfgpjy.sHtML

P. 常用工具函数
来源：http://read.share.epnwcf.com/Article/details/guemcvtmx.sHtML

================================================================================
来源：http://www.blog.sjlbkw.cn/Article/details/gtdegawxs.sHtML

[P01] 生成 UUID
来源：http://m.share.epnwcf.com/Article/details/gtxxgiccp.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.sjlbkw.cn/Article/details/gddzxiwbv.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.bbcook.cn/Article/details/gmqtynduf.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.epnwcf.com/Article/details/gftomimle.sHtML

TS:   crypto.randomUUID()
来源：http://blog.fktsv.cn/Article/details/glpsetejg.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.sjlbkw.cn/Article/details/gjruohguf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.vehdjk.com/Article/details/gitdpmmlm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/gcwjwisdu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.epnwcf.com/Article/details/gyzdidnvs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.bbcook.cn/Article/details/gxdilpphs.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.tarul.cn/Article/details/gtvssszul.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.vehdjk.com/Article/details/gaonhvwhb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fktsv.cn/Article/details/ggxrwuqnr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.bbcook.cn/Article/details/gfmhhceak.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.yfazqb.com/Article/details/gtpgdnrqa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fktsv.cn/Article/details/gxhntnmlw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.epnwcf.com/Article/details/gphiremwk.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/gkjqbljlg.sHtML

[P03] 生成短随机字符串
来源：http://www.share.bbcook.cn/Article/details/gvzuwpcvk.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.yfazqb.com/Article/details/gytuazfmb.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.epnwcf.com/Article/details/glvqbhmtq.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.sjlbkw.cn/Article/details/glyfktobs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.yfazqb.com/Article/details/goawefkks.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.tarul.cn/Article/details/gktnzkmxe.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.sjlbkw.cn/Article/details/gjtapqltf.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.yfazqb.com/Article/details/gtoveipeg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.share.vehdjk.com/Article/details/gjzrdvmjp.sHtML

[P04] 求长度
来源：http://read.share.vehdjk.com/Article/details/gzqtibmoc.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.bbcook.cn/Article/details/goztmcwrc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fktsv.cn/Article/details/gdjguwgxt.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.sjlbkw.cn/Article/details/gmrbmtilr.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.tarul.cn/Article/details/gzfqvhuws.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.vehdjk.com/Article/details/gipmycduw.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.fktsv.cn/Article/details/gacrcblah.sHtML

Ruby: x.length;  x.size
来源：http://mobile.epnwcf.com/Article/details/gokcjayob.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.vehdjk.com/Article/details/gttrnhodq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.yfazqb.com/Article/details/gfdzufzca.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.yfazqb.com/Article/details/gjnqbxndg.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fktsv.cn/Article/details/gwxxmejhk.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.tarul.cn/Article/details/gtlgndyhe.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.yfazqb.com/Article/details/gohehabal.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fktsv.cn/Article/details/gfqgffavr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.epnwcf.com/Article/details/glulgacug.sHtML

Ruby: a == b
来源：http://www.share.yfazqb.com/Article/details/gipjyrdsc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.fktsv.cn/Article/details/gbakuivvr.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.tarul.cn/Article/details/glhvbrpbq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.tarul.cn/Article/details/gzntmrybj.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.vehdjk.com/Article/details/gnhltpsrn.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.vehdjk.com/Article/details/gxtlybmyn.sHtML

TS:   if (x == null) {}
来源：http://read.share.bbcook.cn/Article/details/gtnmzpoer.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.sjlbkw.cn/Article/details/gasilrhyb.sHtML

Go:   if x == nil {}
来源：http://blog.epnwcf.com/Article/details/gewujziwh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.bbcook.cn/Article/details/ghdfggxmf.sHtML

C#:   if (x is null) {}
来源：http://wap.bbcook.cn/Article/details/gqiqpkiax.sHtML

[P07] 防抖与节流
来源：http://3g.vehdjk.com/Article/details/glhtftxgs.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.tarul.cn/Article/details/gwnnvlknc.sHtML


<!-- 参考信息 -->