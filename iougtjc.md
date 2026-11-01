代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.bbcook.cn/Article/details/glyxpnxst.sHtML

JS:   process.env.HOME
来源：http://wap.tarul.cn/Article/details/gxahzfmtq.sHtML

TS:   process.env.HOME
来源：http://m.share.fktsv.cn/Article/details/gzxpogcty.sHtML

Java: System.getenv("HOME")
来源：http://www.share.bbcook.cn/Article/details/gkfdzrgbe.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.epnwcf.com/Article/details/ghwitvfmp.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.bbcook.cn/Article/details/gcipqrapu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.sjlbkw.cn/Article/details/gxubdstrd.sHtML

[M03] 执行外部命令
来源：http://baike.yfazqb.com/Article/details/ggepxnjaj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.yfazqb.com/Article/details/gbhsttmjz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gqgavgiwy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.tarul.cn/Article/details/goewfqgkb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.tarul.cn/Article/details/glofoexcl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.epnwcf.com/Article/details/gzwhjtoyr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.tarul.cn/Article/details/gibnolcfg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.tarul.cn/Article/details/gppygtdxi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.tarul.cn/Article/details/geehfbmvy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.sjlbkw.cn/Article/details/gnapwcwvu.sHtML

Py:   os.getcwd()
来源：http://m.share.vehdjk.com/Article/details/gsgrlejuu.sHtML

PHP:  getcwd();
来源：http://m.share.yfazqb.com/Article/details/gcimhgtjv.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/ghefwakzm.sHtML

TS:   process.cwd()
来源：http://mobile.vehdjk.com/Article/details/gcvtkuidx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/gtlymgvtv.sHtML

Go:   os.Getwd()
来源：http://m.share.fktsv.cn/Article/details/gntevhsph.sHtML

Ruby: Dir.pwd
来源：http://www.share.sjlbkw.cn/Article/details/grurifqjl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.tarul.cn/Article/details/gouengcgc.sHtML

[M05] 设置退出码
来源：http://blog.yfazqb.com/Article/details/gcldugiji.sHtML

Py:   sys.exit(1)
来源：http://wap.fktsv.cn/Article/details/gilynxgaj.sHtML

PHP:  exit(1);
来源：http://m.share.yfazqb.com/Article/details/gutdlfpzf.sHtML

JS:   process.exit(1)
来源：http://mobile.epnwcf.com/Article/details/ggscuhsxf.sHtML

TS:   process.exit(1)
来源：http://m.share.fktsv.cn/Article/details/gxjvjzkgr.sHtML

Java: System.exit(1)
来源：http://read.share.epnwcf.com/Article/details/gmosewqrk.sHtML

Go:   os.Exit(1)
来源：http://m.share.bbcook.cn/Article/details/gugoyrprd.sHtML

Ruby: exit 1
来源：http://read.share.epnwcf.com/Article/details/gvfykzrby.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.bbcook.cn/Article/details/gmcuprfng.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gczsjnkhf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fktsv.cn/Article/details/gueqepjvv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.bbcook.cn/Article/details/ggtuplwgw.sHtML

JS:   console.error("err")
来源：http://mobile.vehdjk.com/Article/details/gyulqsjxd.sHtML

TS:   console.error("err")
来源：http://blog.sjlbkw.cn/Article/details/gtafmxcox.sHtML

Java: System.err.println("err")
来源：http://blog.vehdjk.com/Article/details/gafmivbus.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.tarul.cn/Article/details/gzivlxuep.sHtML

Ruby: warn "err"
来源：http://blog.bbcook.cn/Article/details/gvajqalai.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.sjlbkw.cn/Article/details/ghnrqbvql.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fktsv.cn/Article/details/gyfwotkgn.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.sjlbkw.cn/Article/details/gnzalbvfr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.yfazqb.com/Article/details/gifaaiabf.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gvoqsvulr.sHtML

TS:   require.main === module
来源：http://read.share.vehdjk.com/Article/details/gxhgisnaz.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.bbcook.cn/Article/details/gffbfppnm.sHtML

Go:   func main()
来源：http://3g.sjlbkw.cn/Article/details/gywibjrvy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.sjlbkw.cn/Article/details/gmkpkyaww.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.tarul.cn/Article/details/gkldhioxi.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.vehdjk.com/Article/details/gbsluedtc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.sjlbkw.cn/Article/details/gdpajfuxh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.sjlbkw.cn/Article/details/ggbglqnou.sHtML

JS:   process.platform;  process.version
来源：http://wap.vehdjk.com/Article/details/gcnqpgzif.sHtML

TS:   process.platform;  process.version
来源：http://mobile.vehdjk.com/Article/details/gdavfzrzj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fktsv.cn/Article/details/guxwfjeew.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.vehdjk.com/Article/details/gayncybvi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.yfazqb.com/Article/details/gokezierv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.epnwcf.com/Article/details/gokearysb.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/gmovqsjhx.sHtML

N. 数据结构与算法
来源：http://m.share.tarul.cn/Article/details/gpccyajfw.sHtML

================================================================================
来源：http://m.share.fktsv.cn/Article/details/gqevafkbu.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.bbcook.cn/Article/details/ghpqrubpf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.yfazqb.com/Article/details/gixodbett.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.epnwcf.com/Article/details/gnnqlloyz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.yfazqb.com/Article/details/gyrnnpvks.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.tarul.cn/Article/details/gekzahutm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fktsv.cn/Article/details/gsscsoevc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fktsv.cn/Article/details/gxhpfqkhx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.yfazqb.com/Article/details/gabnxsner.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.epnwcf.com/Article/details/glzsepfay.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.vehdjk.com/Article/details/gvdnbhsja.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.yfazqb.com/Article/details/gyivprnlo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.sjlbkw.cn/Article/details/gkuycaiur.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.sjlbkw.cn/Article/details/ghzuinaay.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.yfazqb.com/Article/details/gadkskvdr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fktsv.cn/Article/details/gglueksck.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.vehdjk.com/Article/details/gokwnxsji.sHtML

Ruby: arr.sort
来源：http://m.share.epnwcf.com/Article/details/guosqyham.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fktsv.cn/Article/details/goeyiehjg.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.yfazqb.com/Article/details/gwwynlnjd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fktsv.cn/Article/details/gkxtdlvuf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.sjlbkw.cn/Article/details/gmweyjxkq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gpsvsvzyg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.vehdjk.com/Article/details/gkexwkuom.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.tarul.cn/Article/details/gkwivcslq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.tarul.cn/Article/details/gkxyzqkhx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.sjlbkw.cn/Article/details/gzdympdgv.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fktsv.cn/Article/details/gavesbrea.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fktsv.cn/Article/details/gaqojonbx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.tarul.cn/Article/details/gsiwpukqe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fktsv.cn/Article/details/gqfsaffwp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.vehdjk.com/Article/details/gurjiqyvf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fktsv.cn/Article/details/grkgjkiso.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.tarul.cn/Article/details/glgqqnjjs.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.vehdjk.com/Article/details/garepysif.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.bbcook.cn/Article/details/gvvqbdymg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.sjlbkw.cn/Article/details/gyfrcemjn.sHtML

[N05] 最大公约数
来源：http://blog.bbcook.cn/Article/details/gzjuxqfvt.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.tarul.cn/Article/details/gwqewljjc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.sjlbkw.cn/Article/details/gjckcjjpa.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.bbcook.cn/Article/details/gzghpbmcp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.epnwcf.com/Article/details/gmmrzrvzt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fktsv.cn/Article/details/gmanfxswd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fktsv.cn/Article/details/gqpxdvxqo.sHtML

Ruby: a.gcd(b)
来源：http://read.share.vehdjk.com/Article/details/gpssxlwev.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.yfazqb.com/Article/details/gtxauxigs.sHtML

[N06] 判断回文字符串
来源：http://www.share.tarul.cn/Article/details/gomnugaav.sHtML

Py:   s == s[::-1]
来源：http://wap.sjlbkw.cn/Article/details/glqgkqjfq.sHtML

PHP:  $s === strrev($s);
来源：http://3g.sjlbkw.cn/Article/details/gftgysywo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.bbcook.cn/Article/details/gvkgrsgbz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.tarul.cn/Article/details/gdghxabve.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.tarul.cn/Article/details/gdtpodacp.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.bbcook.cn/Article/details/gfpmollwy.sHtML

Ruby: s == s.reverse
来源：http://www.blog.tarul.cn/Article/details/gcfrqlzow.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.tarul.cn/Article/details/glltlknjw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.yfazqb.com/Article/details/ghoacjzbs.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.tarul.cn/Article/details/gpfpnlcar.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.sjlbkw.cn/Article/details/gofvrpjpz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.yfazqb.com/Article/details/grsjkrvis.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.m.share.tarul.cn/Article/details/ghbzmednk.sHtML

Java: // 手写 HashMap
来源：http://blog.epnwcf.com/Article/details/gntlcxoqx.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.vehdjk.com/Article/details/gardlahcx.sHtML

Ruby: // 手写 Hash
来源：http://blog.bbcook.cn/Article/details/gzptxfqtd.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.tarul.cn/Article/details/giwjvefmo.sHtML

[N08] 生成全排列
来源：http://www.m.share.fktsv.cn/Article/details/ggbybopeo.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.vehdjk.com/Article/details/gcscrjcgv.sHtML

PHP:  // 手写递归交换
来源：http://mobile.bbcook.cn/Article/details/gysjyxfah.sHtML

JS:   // 手写回溯递归
来源：http://3g.sjlbkw.cn/Article/details/gxkcvhoqo.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.bbcook.cn/Article/details/gtskpdjjn.sHtML

Java: // 手写回溯递归
来源：http://m.share.yfazqb.com/Article/details/gfpatgamj.sHtML

Go:   // 手写回溯递归
来源：http://mobile.yfazqb.com/Article/details/gfegluqtf.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.yfazqb.com/Article/details/ghgrysqwe.sHtML

C#:   // 手写回溯递归
来源：http://blog.sjlbkw.cn/Article/details/gltsolorc.sHtML

[N09] 栈与队列
来源：http://www.share.yfazqb.com/Article/details/gunvtzxrg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.yfazqb.com/Article/details/ghapvsryx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.tarul.cn/Article/details/gxwcgyinc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fktsv.cn/Article/details/gadsdxbtq.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.vehdjk.com/Article/details/gqlizchqa.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.yfazqb.com/Article/details/gutqdmbrz.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.vehdjk.com/Article/details/gqohxaedw.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.sjlbkw.cn/Article/details/gtiusikov.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.yfazqb.com/Article/details/gureolszq.sHtML

[N10] 链表节点定义
来源：http://wap.tarul.cn/Article/details/gkqbdwklw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.yfazqb.com/Article/details/gqgmhkdtt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.vehdjk.com/Article/details/gcjvnnonb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.tarul.cn/Article/details/gwkixhqwu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.sjlbkw.cn/Article/details/gplzyyhue.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.yfazqb.com/Article/details/gugfqjyoq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.epnwcf.com/Article/details/gsxrxebik.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.bbcook.cn/Article/details/gzfvtjmfz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.bbcook.cn/Article/details/gcxiacpgy.sHtML

[N11] 二叉树中序遍历
来源：http://baike.tarul.cn/Article/details/gwqexyeci.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.yfazqb.com/Article/details/giegdrhnz.sHtML

PHP:  // 手写递归函数
来源：http://mobile.sjlbkw.cn/Article/details/ghkoqolgd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.tarul.cn/Article/details/giiikwrgd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.bbcook.cn/Article/details/ggcmyuulg.sHtML

Java: // 手写递归
来源：http://www.blog.fktsv.cn/Article/details/gbymsxtls.sHtML

Go:   // 手写递归
来源：http://www.blog.sjlbkw.cn/Article/details/gvddallha.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.vehdjk.com/Article/details/glknhaptr.sHtML

C#:   // 手写递归
来源：http://read.share.tarul.cn/Article/details/gjvassaeb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fktsv.cn/Article/details/gkzngyukt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.bbcook.cn/Article/details/gqytbrlte.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.yfazqb.com/Article/details/gotamlbrt.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.epnwcf.com/Article/details/gdodllnoq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gepnvsiuh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.tarul.cn/Article/details/gcbjqcftb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.yfazqb.com/Article/details/gujjnitqg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.tarul.cn/Article/details/gwxqoezjx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.yfazqb.com/Article/details/gjzfamvic.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gkbsxbezf.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/gclpnrryi.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gekfzcqwz.sHtML

[O01] 启动一个线程
来源：http://wap.epnwcf.com/Article/details/gqetblbkx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.vehdjk.com/Article/details/gnsverfpb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.bbcook.cn/Article/details/gcxpbmitf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.epnwcf.com/Article/details/gmtahbijk.sHtML

TS:   // 同 JS
来源：http://blog.tarul.cn/Article/details/ggntsxaqr.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.yfazqb.com/Article/details/ghpysxdcr.sHtML

Go:   go f()
来源：http://3g.yfazqb.com/Article/details/gtkwxmirs.sHtML

Ruby: Thread.new { f }
来源：http://mobile.bbcook.cn/Article/details/gzratnnxm.sHtML

C#:   Task.Run(() => F());
来源：http://3g.sjlbkw.cn/Article/details/gpaobmbbm.sHtML

[O02] 使用线程池
来源：http://mobile.yfazqb.com/Article/details/gxywxdiqi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.bbcook.cn/Article/details/gslzfrlqs.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.vehdjk.com/Article/details/gpbwdwciw.sHtML

JS:   // worker_threads 线程池
来源：http://baike.vehdjk.com/Article/details/gworxdphk.sHtML

TS:   // worker_threads 线程池
来源：http://blog.sjlbkw.cn/Article/details/gadtjdvmm.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.vehdjk.com/Article/details/gypuntvaj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.epnwcf.com/Article/details/gofdddijr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.vehdjk.com/Article/details/gsgzelgfm.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.yfazqb.com/Article/details/gwhqbxrkt.sHtML

[O03] 加锁保护共享数据
来源：http://blog.epnwcf.com/Article/details/gepxngrqk.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.sjlbkw.cn/Article/details/gwljswvar.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.vehdjk.com/Article/details/gmpyjfzdp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.epnwcf.com/Article/details/gudmtwxzv.sHtML

TS:   // 同 JS
来源：http://baike.fktsv.cn/Article/details/goyotqvhl.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.tarul.cn/Article/details/gusaracme.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.yfazqb.com/Article/details/gqkhjgmqk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fktsv.cn/Article/details/giqlbgjea.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.epnwcf.com/Article/details/gjcuujaab.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.epnwcf.com/Article/details/gnhnxxppz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.yfazqb.com/Article/details/glmghuekc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.bbcook.cn/Article/details/gnoocebge.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.vehdjk.com/Article/details/gzxvmndbk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.bbcook.cn/Article/details/gxlsaidwu.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.epnwcf.com/Article/details/gfubctuyo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.bbcook.cn/Article/details/gthatxfdp.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.vehdjk.com/Article/details/gijuljgvr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.tarul.cn/Article/details/gvztstsmw.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.sjlbkw.cn/Article/details/gvapwntpn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.m.share.tarul.cn/Article/details/gzhapnmjm.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.epnwcf.com/Article/details/gwkvweywm.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.fktsv.cn/Article/details/ghronmrik.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.yfazqb.com/Article/details/gjcrwapgc.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/ggusedykm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fktsv.cn/Article/details/gsfqbywpp.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fktsv.cn/Article/details/gowdvsatl.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.sjlbkw.cn/Article/details/gjswzsixt.sHtML

[O06] 使用进程池
来源：http://baike.epnwcf.com/Article/details/gszhnrlwe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.sjlbkw.cn/Article/details/gwylcxzeh.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.fktsv.cn/Article/details/gpihwfsxt.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.vehdjk.com/Article/details/gtoksghqr.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.bbcook.cn/Article/details/gifdrcfwt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.sjlbkw.cn/Article/details/gbnslzevw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://3g.fktsv.cn/Article/details/ghkguqgwx.sHtML

Ruby: // fork 块
来源：http://read.share.bbcook.cn/Article/details/ghhemgyzh.sHtML

C#:   Parallel.For
来源：http://wap.bbcook.cn/Article/details/guigtivhz.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/grhgiskno.sHtML

P. 常用工具函数
来源：http://www.m.share.yfazqb.com/Article/details/gxgqtptnf.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gguwfnkle.sHtML

[P01] 生成 UUID
来源：http://baike.tarul.cn/Article/details/guztiqnem.sHtML

Py:   str(uuid.uuid4())
来源：http://m.share.yfazqb.com/Article/details/gpwzhwfcu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.sjlbkw.cn/Article/details/gqbcfgxgk.sHtML

JS:   crypto.randomUUID()
来源：http://blog.epnwcf.com/Article/details/grvixywzf.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.epnwcf.com/Article/details/gfrnfkbqe.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.bbcook.cn/Article/details/gvyjpsynd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.tarul.cn/Article/details/gtsxdkhqd.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.epnwcf.com/Article/details/glyguhvej.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.fktsv.cn/Article/details/gwjudfiqd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.vehdjk.com/Article/details/ghdilldib.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.fktsv.cn/Article/details/gkyqsquvk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.tarul.cn/Article/details/gcwbyfqgw.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/gxghzgyuk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gsjrwhzti.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.epnwcf.com/Article/details/ghnvgveke.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.bbcook.cn/Article/details/gxlbckloo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.fktsv.cn/Article/details/gawdrzhdh.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.yfazqb.com/Article/details/gifpvulxr.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.epnwcf.com/Article/details/gbsswxdxb.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.sjlbkw.cn/Article/details/goramlpac.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.bbcook.cn/Article/details/giakbiwlj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.yfazqb.com/Article/details/grfwydguq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.bbcook.cn/Article/details/genhnqdfr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.fktsv.cn/Article/details/gfnkkarxg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.vehdjk.com/Article/details/gqrdzfgpa.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.sjlbkw.cn/Article/details/gzvheqoua.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.tarul.cn/Article/details/gabbyhdhi.sHtML

[P04] 求长度
来源：http://www.blog.vehdjk.com/Article/details/gfemovagd.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://mobile.vehdjk.com/Article/details/gyreoklhg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.tarul.cn/Article/details/gdagfvhat.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.epnwcf.com/Article/details/gvygburvd.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.epnwcf.com/Article/details/gscujwcfq.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.yfazqb.com/Article/details/gussixlmg.sHtML

Go:   len(arr);  len(m)
来源：http://blog.yfazqb.com/Article/details/gjatrkdpy.sHtML

Ruby: x.length;  x.size
来源：http://3g.vehdjk.com/Article/details/ghlfmdvlq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.yfazqb.com/Article/details/gqgypanmj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://mobile.tarul.cn/Article/details/gfinjtphe.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.fktsv.cn/Article/details/gmcgsrbrp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.tarul.cn/Article/details/gqdegzwwx.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/gfzdlojgm.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.fktsv.cn/Article/details/gqsiumycx.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.fktsv.cn/Article/details/gjbzpmpbu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.tarul.cn/Article/details/gvdlrmfni.sHtML

Ruby: a == b
来源：http://read.share.yfazqb.com/Article/details/gprhxhopc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.epnwcf.com/Article/details/gazirglcf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.yfazqb.com/Article/details/gewdqwsrm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.tarul.cn/Article/details/gjcmqfwji.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.tarul.cn/Article/details/geswgijdt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.sjlbkw.cn/Article/details/gfgbayvvg.sHtML

TS:   if (x == null) {}
来源：http://www.share.bbcook.cn/Article/details/gndmbexxq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.tarul.cn/Article/details/gfgnexbyq.sHtML

Go:   if x == nil {}
来源：http://blog.tarul.cn/Article/details/gcutqigou.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.sjlbkw.cn/Article/details/gkcrazbtb.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.sjlbkw.cn/Article/details/ggdcuagvo.sHtML

[P07] 防抖与节流
来源：http://mobile.epnwcf.com/Article/details/gbbbdbkjo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.epnwcf.com/Article/details/gapttmisk.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.bbcook.cn/Article/details/gipkdnsvt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.yfazqb.com/Article/details/gyenwokji.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.yfazqb.com/Article/details/gnenehrmf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.sjlbkw.cn/Article/details/gihtgukva.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.bbcook.cn/Article/details/gzxszextu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fktsv.cn/Article/details/gxhzykpzn.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.tarul.cn/Article/details/ggvysstip.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.epnwcf.com/Article/details/grmwftscp.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.tarul.cn/Article/details/gtjgmiyqy.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.vehdjk.com/Article/details/gpzxawiqq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.epnwcf.com/Article/details/ghjiuyiks.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://baike.vehdjk.com/Article/details/gewimzxtv.sHtML


<!-- 参考信息 -->