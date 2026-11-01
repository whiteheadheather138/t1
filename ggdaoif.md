代发 wailian999

Ruby: ARGV
来源：http://wap.tarul.cn/Article/details/gtztgwtct.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.bbcook.cn/Article/details/gbltcckzw.sHtML

[M02] 读取环境变量
来源：http://wap.sjlbkw.cn/Article/details/gcqtjtbsg.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.sjlbkw.cn/Article/details/gemkksfov.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.bbcook.cn/Article/details/gydvehpdq.sHtML

JS:   process.env.HOME
来源：http://wap.yfazqb.com/Article/details/ghqvfqgya.sHtML

TS:   process.env.HOME
来源：http://m.share.sjlbkw.cn/Article/details/gnkjijytd.sHtML

Java: System.getenv("HOME")
来源：http://3g.bbcook.cn/Article/details/gyflvpvgw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.yfazqb.com/Article/details/ghzwzbdso.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.bbcook.cn/Article/details/gblbtzlzg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.tarul.cn/Article/details/gptfwxnpc.sHtML

[M03] 执行外部命令
来源：http://www.blog.epnwcf.com/Article/details/gcrxrkxfm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.tarul.cn/Article/details/gmmiozuzq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.bbcook.cn/Article/details/gsjobdqfe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.yfazqb.com/Article/details/githznjaw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.tarul.cn/Article/details/gftpebdly.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.yfazqb.com/Article/details/gevwgedrj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.sjlbkw.cn/Article/details/gvyczdrqm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.sjlbkw.cn/Article/details/gueffvbsv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.sjlbkw.cn/Article/details/gzgadiqvv.sHtML

[M04] 获取当前工作目录
来源：http://www.share.yfazqb.com/Article/details/gtyrblpzl.sHtML

Py:   os.getcwd()
来源：http://www.m.share.tarul.cn/Article/details/gxuvcprcp.sHtML

PHP:  getcwd();
来源：http://m.share.epnwcf.com/Article/details/gqzwercld.sHtML

JS:   process.cwd()
来源：http://www.m.share.epnwcf.com/Article/details/gcmumegmy.sHtML

TS:   process.cwd()
来源：http://www.share.epnwcf.com/Article/details/gjqqmswth.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.bbcook.cn/Article/details/guslxesox.sHtML

Go:   os.Getwd()
来源：http://mobile.bbcook.cn/Article/details/gtqgxbezd.sHtML

Ruby: Dir.pwd
来源：http://www.share.bbcook.cn/Article/details/gocknhzbs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.bbcook.cn/Article/details/gznfhmubz.sHtML

[M05] 设置退出码
来源：http://3g.tarul.cn/Article/details/grdphangx.sHtML

Py:   sys.exit(1)
来源：http://mobile.fktsv.cn/Article/details/gnocnnwik.sHtML

PHP:  exit(1);
来源：http://baike.epnwcf.com/Article/details/gegejnfqx.sHtML

JS:   process.exit(1)
来源：http://mobile.vehdjk.com/Article/details/gxbsfrdqv.sHtML

TS:   process.exit(1)
来源：http://3g.yfazqb.com/Article/details/gtqnphaoy.sHtML

Java: System.exit(1)
来源：http://www.blog.vehdjk.com/Article/details/gfaomaqmk.sHtML

Go:   os.Exit(1)
来源：http://read.share.vehdjk.com/Article/details/gthgdwcbc.sHtML

Ruby: exit 1
来源：http://m.share.epnwcf.com/Article/details/gviypvdnm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.vehdjk.com/Article/details/gjighfali.sHtML

[M06] 向标准错误输出
来源：http://read.share.vehdjk.com/Article/details/gfevctcmq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.bbcook.cn/Article/details/gsfjwnqjg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.bbcook.cn/Article/details/gzvywmbxg.sHtML

JS:   console.error("err")
来源：http://read.share.vehdjk.com/Article/details/gycztyftk.sHtML

TS:   console.error("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gqsgbywmk.sHtML

Java: System.err.println("err")
来源：http://blog.fktsv.cn/Article/details/gympntqlv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.epnwcf.com/Article/details/gbigcmkio.sHtML

Ruby: warn "err"
来源：http://blog.yfazqb.com/Article/details/gowwukhvy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.yfazqb.com/Article/details/gfjkzyivo.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.epnwcf.com/Article/details/guampqjej.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.epnwcf.com/Article/details/gptktpbei.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.epnwcf.com/Article/details/gzuzzerjr.sHtML

JS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gqryxtmpz.sHtML

TS:   require.main === module
来源：http://mobile.bbcook.cn/Article/details/gvtualbsd.sHtML

Java: public static void main(String[] args)
来源：http://wap.sjlbkw.cn/Article/details/getkysuwu.sHtML

Go:   func main()
来源：http://read.share.vehdjk.com/Article/details/gppcbzxec.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.tarul.cn/Article/details/gwtanoqnw.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gynndljqc.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.epnwcf.com/Article/details/gqjblrdsd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.sjlbkw.cn/Article/details/gruuyiqhb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.bbcook.cn/Article/details/gzohaavie.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.vehdjk.com/Article/details/gplungabx.sHtML

TS:   process.platform;  process.version
来源：http://wap.sjlbkw.cn/Article/details/gymzcwtem.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.bbcook.cn/Article/details/gfuxybncw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.yfazqb.com/Article/details/glnliuabg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gilkmqbur.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.sjlbkw.cn/Article/details/ghksplcvt.sHtML

================================================================================
来源：http://baike.vehdjk.com/Article/details/gserfxihf.sHtML

N. 数据结构与算法
来源：http://mobile.vehdjk.com/Article/details/gdjbrihnd.sHtML

================================================================================
来源：http://www.blog.yfazqb.com/Article/details/gulukksul.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.epnwcf.com/Article/details/gpnjhqkxs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.tarul.cn/Article/details/gskihxmfi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fktsv.cn/Article/details/gutvpsrbx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.epnwcf.com/Article/details/gfufiivjh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.tarul.cn/Article/details/gspixvsvv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.epnwcf.com/Article/details/gsvrayviq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fktsv.cn/Article/details/gbleowzfc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.vehdjk.com/Article/details/gmkubldrk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.vehdjk.com/Article/details/gpzsmpstj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.sjlbkw.cn/Article/details/gorzzlnei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.bbcook.cn/Article/details/gnfqwryfx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.sjlbkw.cn/Article/details/glcwjpgeq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.tarul.cn/Article/details/gjwchumaq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fktsv.cn/Article/details/gorzkxmyb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.vehdjk.com/Article/details/gilipbeij.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.epnwcf.com/Article/details/gzbvonzeu.sHtML

Ruby: arr.sort
来源：http://wap.sjlbkw.cn/Article/details/gbepyvhni.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.yfazqb.com/Article/details/gweagzkoj.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.yfazqb.com/Article/details/gbupmzzpi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.vehdjk.com/Article/details/gutnhczuk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fktsv.cn/Article/details/gthgygjdc.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.bbcook.cn/Article/details/gtxlzbvum.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.yfazqb.com/Article/details/gufyskbde.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.sjlbkw.cn/Article/details/gjahlrfuw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.tarul.cn/Article/details/gooevwjeo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.bbcook.cn/Article/details/gsfqscnqs.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.tarul.cn/Article/details/gdthcauju.sHtML

[N04] 斐波那契数列
来源：http://www.blog.sjlbkw.cn/Article/details/gczxdpbow.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.tarul.cn/Article/details/gqfkwrlsj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.bbcook.cn/Article/details/gzafivsns.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.bbcook.cn/Article/details/gpeqripzc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.bbcook.cn/Article/details/gxpcvjkpb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.bbcook.cn/Article/details/gbaepscnn.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fktsv.cn/Article/details/gutbvfekf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.tarul.cn/Article/details/gkbrifnxd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fktsv.cn/Article/details/gksrjcjfb.sHtML

[N05] 最大公约数
来源：http://mobile.epnwcf.com/Article/details/gwoqdqnnr.sHtML

Py:   math.gcd(a, b)
来源：http://wap.bbcook.cn/Article/details/gkvwlpgdy.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.bbcook.cn/Article/details/grlskogne.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.vehdjk.com/Article/details/gnhwhbcfd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.vehdjk.com/Article/details/ggesecmuy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.epnwcf.com/Article/details/gyblzmspb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.vehdjk.com/Article/details/ghssrmibd.sHtML

Ruby: a.gcd(b)
来源：http://blog.tarul.cn/Article/details/gmqtuiuyn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fktsv.cn/Article/details/gaujqrqfa.sHtML

[N06] 判断回文字符串
来源：http://mobile.tarul.cn/Article/details/gyjelfguk.sHtML

Py:   s == s[::-1]
来源：http://www.share.tarul.cn/Article/details/gxrkamgyw.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.epnwcf.com/Article/details/gfiiuhbav.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.yfazqb.com/Article/details/gqofvxbmb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.vehdjk.com/Article/details/goghlnrui.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.bbcook.cn/Article/details/gwijzlndc.sHtML

Go:   // 双指针从两端比较
来源：http://wap.tarul.cn/Article/details/gdjhzpdrd.sHtML

Ruby: s == s.reverse
来源：http://3g.epnwcf.com/Article/details/ggtriobvk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.epnwcf.com/Article/details/gqaancwzu.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fktsv.cn/Article/details/gvmvagzvz.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.bbcook.cn/Article/details/gomuylqjl.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.yfazqb.com/Article/details/ggxlfhdvb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.epnwcf.com/Article/details/gngjhlzue.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.sjlbkw.cn/Article/details/gpjepyxyk.sHtML

Java: // 手写 HashMap
来源：http://3g.sjlbkw.cn/Article/details/gdjqykids.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.vehdjk.com/Article/details/gwjbwcapz.sHtML

Ruby: // 手写 Hash
来源：http://blog.vehdjk.com/Article/details/gzzruwvqo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.sjlbkw.cn/Article/details/geckewjbm.sHtML

[N08] 生成全排列
来源：http://baike.bbcook.cn/Article/details/glenhhjsc.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.yfazqb.com/Article/details/gstzwyciv.sHtML

PHP:  // 手写递归交换
来源：http://baike.bbcook.cn/Article/details/gpsoyxppa.sHtML

JS:   // 手写回溯递归
来源：http://baike.fktsv.cn/Article/details/ghqwzepbp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.bbcook.cn/Article/details/gguqcbjhz.sHtML

Java: // 手写回溯递归
来源：http://mobile.epnwcf.com/Article/details/ggztrlfot.sHtML

Go:   // 手写回溯递归
来源：http://mobile.bbcook.cn/Article/details/getikaqpz.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/gvsqknhah.sHtML

C#:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gyxmggrlc.sHtML

[N09] 栈与队列
来源：http://www.share.tarul.cn/Article/details/gioovuwvr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fktsv.cn/Article/details/gwbfygxjb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.fktsv.cn/Article/details/gdyjbfryt.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.sjlbkw.cn/Article/details/gjxafxydm.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fktsv.cn/Article/details/gcoksjbsi.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.yfazqb.com/Article/details/gyxkrwgph.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.tarul.cn/Article/details/ggcjvcuao.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gewocwkhe.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.bbcook.cn/Article/details/gduortdbj.sHtML

[N10] 链表节点定义
来源：http://blog.tarul.cn/Article/details/glzjoqgfh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.bbcook.cn/Article/details/gvvbgdjwv.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.sjlbkw.cn/Article/details/gzifbelhg.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.epnwcf.com/Article/details/ghfdofqqq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.bbcook.cn/Article/details/ggcnfpqqj.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.vehdjk.com/Article/details/gkykiluow.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.vehdjk.com/Article/details/gvcwtcner.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fktsv.cn/Article/details/gneqihatl.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.epnwcf.com/Article/details/gawtdrlpd.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.yfazqb.com/Article/details/gsjhvcscb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fktsv.cn/Article/details/ggpretglc.sHtML

PHP:  // 手写递归函数
来源：http://www.share.bbcook.cn/Article/details/genzrarkn.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.yfazqb.com/Article/details/gfudknqxd.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.vehdjk.com/Article/details/gvxoiofgq.sHtML

Java: // 手写递归
来源：http://www.share.sjlbkw.cn/Article/details/gfhqedvqb.sHtML

Go:   // 手写递归
来源：http://3g.tarul.cn/Article/details/gjkpfhlnm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.epnwcf.com/Article/details/gshawawli.sHtML

C#:   // 手写递归
来源：http://read.share.vehdjk.com/Article/details/gelmxbvnr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fktsv.cn/Article/details/glkkgrkmq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.fktsv.cn/Article/details/gltnqdpls.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.bbcook.cn/Article/details/gojpkljvj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.tarul.cn/Article/details/gpnffcpio.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.yfazqb.com/Article/details/gyrtystgo.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.tarul.cn/Article/details/gpqenrwfe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.vehdjk.com/Article/details/gyidimwqb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.vehdjk.com/Article/details/gmhdyiupz.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.vehdjk.com/Article/details/gxsyqwoed.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/gaxiezeqz.sHtML

O. 并发与异步
来源：http://3g.vehdjk.com/Article/details/ggxwsmafb.sHtML

================================================================================
来源：http://m.share.epnwcf.com/Article/details/gjnxjmqep.sHtML

[O01] 启动一个线程
来源：http://www.share.vehdjk.com/Article/details/gykoktfau.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.yfazqb.com/Article/details/gektszqik.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.tarul.cn/Article/details/gjoypmmfw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.vehdjk.com/Article/details/gzoxguewz.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/ghowaztdu.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.fktsv.cn/Article/details/gfcjwdtpi.sHtML

Go:   go f()
来源：http://www.m.share.sjlbkw.cn/Article/details/grliwytdf.sHtML

Ruby: Thread.new { f }
来源：http://blog.vehdjk.com/Article/details/gffosdodc.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.vehdjk.com/Article/details/gmasexpqt.sHtML

[O02] 使用线程池
来源：http://mobile.fktsv.cn/Article/details/gdfwudgif.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.yfazqb.com/Article/details/gabpvuzas.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.tarul.cn/Article/details/ginjpzzdc.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.sjlbkw.cn/Article/details/gtvqzdpzf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.yfazqb.com/Article/details/gjjuszscc.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fktsv.cn/Article/details/gnvvyhcxh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gpzjkhzbz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.epnwcf.com/Article/details/gryyahlul.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.bbcook.cn/Article/details/gmtqbmpwh.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.yfazqb.com/Article/details/gpsdtojqn.sHtML

Py:   with lock: shared += 1
来源：http://www.share.vehdjk.com/Article/details/gcbsruxpp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fktsv.cn/Article/details/glzgxbsdc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.fktsv.cn/Article/details/gvvivlveo.sHtML

TS:   // 同 JS
来源：http://3g.yfazqb.com/Article/details/gcxrzbaqf.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gfwemtwoh.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://blog.vehdjk.com/Article/details/gmyngyxpz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.bbcook.cn/Article/details/glxsmkqqh.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.fktsv.cn/Article/details/ghklweeib.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fktsv.cn/Article/details/ghoueyvhd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.bbcook.cn/Article/details/gtzgtslhh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.epnwcf.com/Article/details/gqwtpuxlx.sHtML

JS:   async function f() { await g(); }
来源：http://blog.bbcook.cn/Article/details/gbwbuamwr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.sjlbkw.cn/Article/details/grobtagmk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gyhsqkgkw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gyigsozxh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.vehdjk.com/Article/details/gymlxbsbp.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.yfazqb.com/Article/details/gvhyatpnn.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.tarul.cn/Article/details/gkegisbfe.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.sjlbkw.cn/Article/details/gpiyowntb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.tarul.cn/Article/details/gzbnziuwg.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fktsv.cn/Article/details/gxzpkplqb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.yfazqb.com/Article/details/goehommqt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.vehdjk.com/Article/details/gtipkcwsk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.yfazqb.com/Article/details/gtmzruodq.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.bbcook.cn/Article/details/glnkwpelx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.yfazqb.com/Article/details/gtvjbamjv.sHtML

[O06] 使用进程池
来源：http://blog.bbcook.cn/Article/details/gkealvcnu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.tarul.cn/Article/details/gqfwveitd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.yfazqb.com/Article/details/gjfhbhzca.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.epnwcf.com/Article/details/gfblyzgty.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.yfazqb.com/Article/details/gqkbujqdw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.sjlbkw.cn/Article/details/gxolrvgof.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.bbcook.cn/Article/details/gargplgjl.sHtML

Ruby: // fork 块
来源：http://m.share.yfazqb.com/Article/details/gxzcokdjg.sHtML

C#:   Parallel.For
来源：http://wap.sjlbkw.cn/Article/details/gifyllmbi.sHtML

================================================================================
来源：http://wap.vehdjk.com/Article/details/gtzvpyeiu.sHtML

P. 常用工具函数
来源：http://wap.yfazqb.com/Article/details/glrostxel.sHtML

================================================================================
来源：http://www.m.share.epnwcf.com/Article/details/geyqitswn.sHtML

[P01] 生成 UUID
来源：http://www.m.share.yfazqb.com/Article/details/giccvcjse.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.sjlbkw.cn/Article/details/godjbtnix.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.bbcook.cn/Article/details/gdmswygjm.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.yfazqb.com/Article/details/gplzvibwp.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.yfazqb.com/Article/details/ggfhzgynm.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.tarul.cn/Article/details/gfafutapi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://mobile.tarul.cn/Article/details/gkgwphjyx.sHtML

Ruby: SecureRandom.uuid
来源：http://www.m.share.fktsv.cn/Article/details/guspxunvr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fktsv.cn/Article/details/gflfqtcsf.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.vehdjk.com/Article/details/gzkfwbqlj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.vehdjk.com/Article/details/glpzdkukt.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.vehdjk.com/Article/details/gfiqyestq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fktsv.cn/Article/details/gkrudfaoz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.epnwcf.com/Article/details/gbkhrlkav.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.bbcook.cn/Article/details/gmnuanzlk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.yfazqb.com/Article/details/gngudeqap.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://wap.fktsv.cn/Article/details/guykqxkky.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.vehdjk.com/Article/details/ggzntkcpr.sHtML

[P03] 生成短随机字符串
来源：http://m.share.sjlbkw.cn/Article/details/ghopeqher.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.tarul.cn/Article/details/gmvvchhjj.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fktsv.cn/Article/details/gahnjoadg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.yfazqb.com/Article/details/gmuaqtrcz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fktsv.cn/Article/details/gxugzobkj.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.vehdjk.com/Article/details/gjmgootdb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.bbcook.cn/Article/details/gpbavyrgp.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.tarul.cn/Article/details/ggrjmvprm.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fktsv.cn/Article/details/ghxmaqpxr.sHtML

[P04] 求长度
来源：http://www.blog.sjlbkw.cn/Article/details/gvrqiebvj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.bbcook.cn/Article/details/gntytbcil.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fktsv.cn/Article/details/gipepxqmu.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.fktsv.cn/Article/details/gzbnepzwt.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fktsv.cn/Article/details/gyambwxlj.sHtML

Java: list.size();  map.size();  s.length()
来源：http://wap.yfazqb.com/Article/details/gzdxpkjpx.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.epnwcf.com/Article/details/gaysicixd.sHtML

Ruby: x.length;  x.size
来源：http://baike.tarul.cn/Article/details/gwmremixg.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.tarul.cn/Article/details/gcmwezxrr.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.bbcook.cn/Article/details/gdtygjxan.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.sjlbkw.cn/Article/details/gtfksozxb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.bbcook.cn/Article/details/gmckdeqcb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.yfazqb.com/Article/details/glfqbvqac.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fktsv.cn/Article/details/gzrczopgw.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.tarul.cn/Article/details/gybillmbt.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.yfazqb.com/Article/details/gdmrlpmhr.sHtML

Ruby: a == b
来源：http://read.share.tarul.cn/Article/details/gnoisekvl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gkcmutuye.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.epnwcf.com/Article/details/glbhljwfm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fktsv.cn/Article/details/gmnphgdtf.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.yfazqb.com/Article/details/gfmarawve.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.yfazqb.com/Article/details/gztrnfmhs.sHtML

TS:   if (x == null) {}
来源：http://www.blog.bbcook.cn/Article/details/gvyshzfaq.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.vehdjk.com/Article/details/grvcxovca.sHtML

Go:   if x == nil {}
来源：http://read.share.fktsv.cn/Article/details/ggfmalvjp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.yfazqb.com/Article/details/glkohcdww.sHtML

C#:   if (x is null) {}
来源：http://mobile.vehdjk.com/Article/details/gkscywdgm.sHtML

[P07] 防抖与节流
来源：http://read.share.bbcook.cn/Article/details/grxptyinr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.sjlbkw.cn/Article/details/gexxqvwvt.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.vehdjk.com/Article/details/gzlsrqbtt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.sjlbkw.cn/Article/details/gnneurezv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fktsv.cn/Article/details/gkyqxeqwv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.epnwcf.com/Article/details/glsepwddp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.epnwcf.com/Article/details/gdmxkasea.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.tarul.cn/Article/details/gfowbzvck.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.vehdjk.com/Article/details/gvuljlzcg.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.vehdjk.com/Article/details/gaiwamhqa.sHtML


<!-- 参考信息 -->