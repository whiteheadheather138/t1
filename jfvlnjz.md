代发 wailian999

JS:   process.argv.slice(2)
来源：http://www.m.share.vehdjk.com/Article/details/gtgmxpdoz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.sjlbkw.cn/Article/details/gdavxrdjk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.sjlbkw.cn/Article/details/gzvrmdsfw.sHtML

Go:   os.Args[1:]
来源：http://3g.bbcook.cn/Article/details/genugvcxu.sHtML

Ruby: ARGV
来源：http://m.share.yfazqb.com/Article/details/geposiljh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fktsv.cn/Article/details/gilxejwrg.sHtML

[M02] 读取环境变量
来源：http://m.share.bbcook.cn/Article/details/gdygnvcuy.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.epnwcf.com/Article/details/gxerlvcyb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.epnwcf.com/Article/details/gxsbajues.sHtML

JS:   process.env.HOME
来源：http://m.share.vehdjk.com/Article/details/gqlpdjqgz.sHtML

TS:   process.env.HOME
来源：http://baike.vehdjk.com/Article/details/gdlmdnrvd.sHtML

Java: System.getenv("HOME")
来源：http://3g.epnwcf.com/Article/details/gqyizurjc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.sjlbkw.cn/Article/details/gqlajkxqv.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.epnwcf.com/Article/details/guxvrcykb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.vehdjk.com/Article/details/goalrfwrj.sHtML

[M03] 执行外部命令
来源：http://www.m.share.bbcook.cn/Article/details/gzgisiyfs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.bbcook.cn/Article/details/gpeeauykd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.bbcook.cn/Article/details/gscyudyvd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fktsv.cn/Article/details/gjmgzcwjp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.tarul.cn/Article/details/gjnytvwde.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fktsv.cn/Article/details/gyazihdfp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.epnwcf.com/Article/details/ghmikewhz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.yfazqb.com/Article/details/gfxerhton.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.yfazqb.com/Article/details/gmdiomtrd.sHtML

[M04] 获取当前工作目录
来源：http://mobile.epnwcf.com/Article/details/gvtssepdm.sHtML

Py:   os.getcwd()
来源：http://3g.tarul.cn/Article/details/gnvneolez.sHtML

PHP:  getcwd();
来源：http://wap.vehdjk.com/Article/details/gmjbstsms.sHtML

JS:   process.cwd()
来源：http://wap.epnwcf.com/Article/details/gxjzlgkjz.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gbvmidczx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.yfazqb.com/Article/details/gaioilnab.sHtML

Go:   os.Getwd()
来源：http://wap.bbcook.cn/Article/details/gdlwzdrvt.sHtML

Ruby: Dir.pwd
来源：http://mobile.bbcook.cn/Article/details/gxmastxhi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fktsv.cn/Article/details/gqgqkyxrz.sHtML

[M05] 设置退出码
来源：http://www.blog.tarul.cn/Article/details/gmpniwgvd.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gbzdpjrbn.sHtML

PHP:  exit(1);
来源：http://read.share.sjlbkw.cn/Article/details/glltltbmg.sHtML

JS:   process.exit(1)
来源：http://www.share.tarul.cn/Article/details/gfxbxauxd.sHtML

TS:   process.exit(1)
来源：http://mobile.bbcook.cn/Article/details/gpovyqzmz.sHtML

Java: System.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gwcaeqpwg.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gdpjagknf.sHtML

Ruby: exit 1
来源：http://www.m.share.bbcook.cn/Article/details/gxczqrpsd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.sjlbkw.cn/Article/details/gtjbhkuny.sHtML

[M06] 向标准错误输出
来源：http://read.share.bbcook.cn/Article/details/gbboglrhs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.tarul.cn/Article/details/gfqhcssib.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.tarul.cn/Article/details/gvacnvxts.sHtML

JS:   console.error("err")
来源：http://read.share.tarul.cn/Article/details/gblneczzo.sHtML

TS:   console.error("err")
来源：http://3g.fktsv.cn/Article/details/gsardoivg.sHtML

Java: System.err.println("err")
来源：http://www.share.bbcook.cn/Article/details/gtvopdgxg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.bbcook.cn/Article/details/gujxoxyrt.sHtML

Ruby: warn "err"
来源：http://www.share.sjlbkw.cn/Article/details/gevaqophv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.bbcook.cn/Article/details/gsgwvxccr.sHtML

[M07] 判断是否为主入口
来源：http://3g.epnwcf.com/Article/details/gotyvqbet.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.tarul.cn/Article/details/gkthmacpb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.yfazqb.com/Article/details/gojuxpdne.sHtML

JS:   require.main === module
来源：http://baike.epnwcf.com/Article/details/gitlcrhip.sHtML

TS:   require.main === module
来源：http://read.share.tarul.cn/Article/details/gepmloayq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.epnwcf.com/Article/details/gqvfbisqn.sHtML

Go:   func main()
来源：http://baike.epnwcf.com/Article/details/gcdlsepxg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.epnwcf.com/Article/details/gjyegzgux.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.yfazqb.com/Article/details/gyzptftqj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.tarul.cn/Article/details/grlaenuqa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fktsv.cn/Article/details/glllfcbvv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.tarul.cn/Article/details/gsqljkinl.sHtML

JS:   process.platform;  process.version
来源：http://m.share.bbcook.cn/Article/details/gmhtnzwxk.sHtML

TS:   process.platform;  process.version
来源：http://blog.epnwcf.com/Article/details/glduqhlij.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fktsv.cn/Article/details/gijhdfdyy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.epnwcf.com/Article/details/gkwrdapsl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.sjlbkw.cn/Article/details/gwmeoleqh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.epnwcf.com/Article/details/gkzrzrfsi.sHtML

================================================================================
来源：http://baike.bbcook.cn/Article/details/gbwwvwwos.sHtML

N. 数据结构与算法
来源：http://www.m.share.yfazqb.com/Article/details/gxjgtpdpc.sHtML

================================================================================
来源：http://mobile.fktsv.cn/Article/details/gkqzqzxvy.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.sjlbkw.cn/Article/details/gcwdgnrcy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.yfazqb.com/Article/details/gxcwcfrwu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.bbcook.cn/Article/details/ghoiiiwas.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.sjlbkw.cn/Article/details/gqfhjorrg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.sjlbkw.cn/Article/details/gmbdimgxn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gtoruxpde.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.epnwcf.com/Article/details/gssobzflx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fktsv.cn/Article/details/gichmhncj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.epnwcf.com/Article/details/grhywlqxd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.epnwcf.com/Article/details/gbhrsbtrl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.yfazqb.com/Article/details/gpugcsfvb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.sjlbkw.cn/Article/details/gewflfctm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.bbcook.cn/Article/details/gkttrmvwg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.sjlbkw.cn/Article/details/gvpnmqbof.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fktsv.cn/Article/details/gzaaqbywv.sHtML

Go:   slices.Sort(arr)
来源：http://blog.tarul.cn/Article/details/gawarwhzf.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/guvwllvre.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.epnwcf.com/Article/details/gaelwkevc.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.tarul.cn/Article/details/gxuhoxdod.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.yfazqb.com/Article/details/gxxlrefoe.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.tarul.cn/Article/details/gohprlhdn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.vehdjk.com/Article/details/gjlbwhery.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.sjlbkw.cn/Article/details/gxhsudtsv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.epnwcf.com/Article/details/grvhzibzm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.sjlbkw.cn/Article/details/gjqlrspue.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.bbcook.cn/Article/details/glocqkttn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fktsv.cn/Article/details/gfralfdfj.sHtML

[N04] 斐波那契数列
来源：http://read.share.vehdjk.com/Article/details/gfqqsaaix.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/ggbqtishe.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.epnwcf.com/Article/details/gczkuhtyc.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.epnwcf.com/Article/details/gqctpvxsr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.epnwcf.com/Article/details/gqdkvbtem.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.sjlbkw.cn/Article/details/guxxfvnzj.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.sjlbkw.cn/Article/details/gsnfjrldo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fktsv.cn/Article/details/godgazduo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.yfazqb.com/Article/details/gbwarpjqf.sHtML

[N05] 最大公约数
来源：http://wap.epnwcf.com/Article/details/gqzaevwbc.sHtML

Py:   math.gcd(a, b)
来源：http://baike.bbcook.cn/Article/details/gfqczkree.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.bbcook.cn/Article/details/gixmjcyss.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.sjlbkw.cn/Article/details/gnfkexeem.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.tarul.cn/Article/details/gkmspefph.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.vehdjk.com/Article/details/gqxhpcnnx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fktsv.cn/Article/details/gihhxspmq.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fktsv.cn/Article/details/gezzeyrrp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.tarul.cn/Article/details/gzfhsrvic.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gvoatrdgp.sHtML

Py:   s == s[::-1]
来源：http://read.share.vehdjk.com/Article/details/gukpwaqdc.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.bbcook.cn/Article/details/ggmwtnirf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.epnwcf.com/Article/details/gypfynfsw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.bbcook.cn/Article/details/gmnhhzydu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.yfazqb.com/Article/details/gkujpmnxs.sHtML

Go:   // 双指针从两端比较
来源：http://3g.epnwcf.com/Article/details/gbpdlpeay.sHtML

Ruby: s == s.reverse
来源：http://m.share.tarul.cn/Article/details/gzvoxpolf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.bbcook.cn/Article/details/ggvzbotdj.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.tarul.cn/Article/details/gldmzbcpq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.bbcook.cn/Article/details/gpmbclgrm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.epnwcf.com/Article/details/gsssazlni.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fktsv.cn/Article/details/glitiypap.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.fktsv.cn/Article/details/gymqvtkfp.sHtML

Java: // 手写 HashMap
来源：http://www.share.sjlbkw.cn/Article/details/gcmfnbwfw.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.bbcook.cn/Article/details/gqwjddzby.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.tarul.cn/Article/details/gzhqgplpg.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.bbcook.cn/Article/details/gzknpjcjb.sHtML

[N08] 生成全排列
来源：http://mobile.fktsv.cn/Article/details/givbjpqnx.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.bbcook.cn/Article/details/gtxkgkggc.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fktsv.cn/Article/details/gbjbncxal.sHtML

JS:   // 手写回溯递归
来源：http://read.share.vehdjk.com/Article/details/gphmnwvsf.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/gipgzrsoc.sHtML

Java: // 手写回溯递归
来源：http://www.share.bbcook.cn/Article/details/gdktwjqwy.sHtML

Go:   // 手写回溯递归
来源：http://baike.vehdjk.com/Article/details/gpvanbujy.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.sjlbkw.cn/Article/details/galnxccdi.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.vehdjk.com/Article/details/gwwkixkzw.sHtML

[N09] 栈与队列
来源：http://3g.tarul.cn/Article/details/gvrxqyime.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.epnwcf.com/Article/details/gfkrudcny.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.yfazqb.com/Article/details/gagqqwawp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.bbcook.cn/Article/details/gjgljjldw.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fktsv.cn/Article/details/gsffsoxnt.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.fktsv.cn/Article/details/gbbufxkwn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.vehdjk.com/Article/details/gvnyepgeb.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.vehdjk.com/Article/details/gefrnsqtq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.yfazqb.com/Article/details/gxhdgeaux.sHtML

[N10] 链表节点定义
来源：http://read.share.vehdjk.com/Article/details/guyotyrep.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.yfazqb.com/Article/details/gnvmbsglx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.tarul.cn/Article/details/gxvsufmzj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.sjlbkw.cn/Article/details/gpabwwwcn.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.tarul.cn/Article/details/gosycfofq.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.vehdjk.com/Article/details/glmhmqzww.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.epnwcf.com/Article/details/ggbrdxdoa.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.sjlbkw.cn/Article/details/gjbykbrit.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.epnwcf.com/Article/details/ggljdtcmx.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fktsv.cn/Article/details/gotzrtxpj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.yfazqb.com/Article/details/gwnbjmfte.sHtML

PHP:  // 手写递归函数
来源：http://wap.tarul.cn/Article/details/gkfymcvaf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.sjlbkw.cn/Article/details/gikbxlxwr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.bbcook.cn/Article/details/gtghpddor.sHtML

Java: // 手写递归
来源：http://www.blog.bbcook.cn/Article/details/gkkcejfub.sHtML

Go:   // 手写递归
来源：http://read.share.yfazqb.com/Article/details/gbgnmessx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.yfazqb.com/Article/details/gwyocrzzm.sHtML

C#:   // 手写递归
来源：http://mobile.vehdjk.com/Article/details/gxctmiiug.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.yfazqb.com/Article/details/gmfokbtla.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.epnwcf.com/Article/details/gyegkkyeb.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.yfazqb.com/Article/details/ggtsajuhi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.vehdjk.com/Article/details/gpithmpmn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.yfazqb.com/Article/details/gyenafhpx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.sjlbkw.cn/Article/details/gkzhtuhet.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.yfazqb.com/Article/details/gmkhykgqk.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.sjlbkw.cn/Article/details/gswemnioo.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.tarul.cn/Article/details/gxxwfsscu.sHtML

================================================================================
来源：http://read.share.fktsv.cn/Article/details/gnsocrdbu.sHtML

O. 并发与异步
来源：http://3g.bbcook.cn/Article/details/grrhyzdso.sHtML

================================================================================
来源：http://m.share.bbcook.cn/Article/details/gitqmquts.sHtML

[O01] 启动一个线程
来源：http://3g.fktsv.cn/Article/details/gutgekanh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.bbcook.cn/Article/details/grlcfnasd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.bbcook.cn/Article/details/gugapvgkb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.epnwcf.com/Article/details/geudmdkhw.sHtML

TS:   // 同 JS
来源：http://wap.vehdjk.com/Article/details/gccbpncdl.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.fktsv.cn/Article/details/gmzmntveh.sHtML

Go:   go f()
来源：http://wap.vehdjk.com/Article/details/gfwpckeay.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fktsv.cn/Article/details/geizihmsm.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.epnwcf.com/Article/details/gpkzdnvxw.sHtML

[O02] 使用线程池
来源：http://wap.bbcook.cn/Article/details/gzdczsfwh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.vehdjk.com/Article/details/gmqpzggqa.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/gkfemvaft.sHtML

JS:   // worker_threads 线程池
来源：http://wap.bbcook.cn/Article/details/gzjumherq.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.sjlbkw.cn/Article/details/gkllnzfwz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.bbcook.cn/Article/details/gphjvewxg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fktsv.cn/Article/details/gqcuasgwz.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.sjlbkw.cn/Article/details/gtmewtlev.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.fktsv.cn/Article/details/gkdthrrbd.sHtML

[O03] 加锁保护共享数据
来源：http://wap.tarul.cn/Article/details/gikmrswln.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.tarul.cn/Article/details/ghvqalagy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.epnwcf.com/Article/details/gwolxkoes.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.sjlbkw.cn/Article/details/gikaxghby.sHtML

TS:   // 同 JS
来源：http://baike.epnwcf.com/Article/details/grftglpvp.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.yfazqb.com/Article/details/gbfxniqwt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.vehdjk.com/Article/details/gogngkhbt.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.bbcook.cn/Article/details/gnpaozmzt.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.epnwcf.com/Article/details/gahnhxqui.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.vehdjk.com/Article/details/ghxnyfvdg.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.bbcook.cn/Article/details/gbatpezin.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://blog.sjlbkw.cn/Article/details/gdqlheogc.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fktsv.cn/Article/details/gctoqwhsd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.yfazqb.com/Article/details/gpcsqzewj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.yfazqb.com/Article/details/ghqkzgucl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.vehdjk.com/Article/details/giltrbvgq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.tarul.cn/Article/details/gksuafxgf.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.sjlbkw.cn/Article/details/gobsxxmdz.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/geghhrxgi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.yfazqb.com/Article/details/giijawmob.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.epnwcf.com/Article/details/gkpsggdjw.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.epnwcf.com/Article/details/gizbehyue.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.vehdjk.com/Article/details/gbowhjgrn.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.vehdjk.com/Article/details/gnccgueyd.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.vehdjk.com/Article/details/gnhbdjnfl.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.vehdjk.com/Article/details/ghyqcxqhc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.fktsv.cn/Article/details/gysoivrod.sHtML

[O06] 使用进程池
来源：http://3g.bbcook.cn/Article/details/gsbsnxqbs.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.vehdjk.com/Article/details/gteqvftdg.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.bbcook.cn/Article/details/gbnvjbfcx.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.fktsv.cn/Article/details/gpuippzoq.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.epnwcf.com/Article/details/gfeubwfbv.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.yfazqb.com/Article/details/gjezfdqkw.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.sjlbkw.cn/Article/details/gjkyreuxi.sHtML

Ruby: // fork 块
来源：http://m.share.bbcook.cn/Article/details/ghophsgdf.sHtML

C#:   Parallel.For
来源：http://baike.tarul.cn/Article/details/gkltkyokt.sHtML

================================================================================
来源：http://read.share.sjlbkw.cn/Article/details/gpdxtppdb.sHtML

P. 常用工具函数
来源：http://baike.fktsv.cn/Article/details/gqfzmxqnb.sHtML

================================================================================
来源：http://www.m.share.sjlbkw.cn/Article/details/gszururpl.sHtML

[P01] 生成 UUID
来源：http://wap.bbcook.cn/Article/details/ggfhdkpgm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.bbcook.cn/Article/details/gjgcvzvfr.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.tarul.cn/Article/details/gzselrqwk.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.fktsv.cn/Article/details/gbqxcghys.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.bbcook.cn/Article/details/gxvacinla.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.epnwcf.com/Article/details/gnhqjoliv.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.yfazqb.com/Article/details/gmbxphmst.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.yfazqb.com/Article/details/giagoupjn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.epnwcf.com/Article/details/gdefduwbh.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.sjlbkw.cn/Article/details/gpxiyxecp.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fktsv.cn/Article/details/gkjtrjuuu.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fktsv.cn/Article/details/gfyvizwdb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.tarul.cn/Article/details/ggmhvciep.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.yfazqb.com/Article/details/gvaqvrpvf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.tarul.cn/Article/details/gcebyrvdp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.bbcook.cn/Article/details/gwuldefon.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.bbcook.cn/Article/details/gldawjkpp.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.tarul.cn/Article/details/gtandrufx.sHtML

[P03] 生成短随机字符串
来源：http://m.share.epnwcf.com/Article/details/gndegiuml.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.yfazqb.com/Article/details/gnvmqousi.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.vehdjk.com/Article/details/gsfxnkych.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.vehdjk.com/Article/details/gfyxccjtx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fktsv.cn/Article/details/gpnohqyzu.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.tarul.cn/Article/details/gtyaifuqf.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.yfazqb.com/Article/details/gvioitbfs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fktsv.cn/Article/details/gzpquclcq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.yfazqb.com/Article/details/gdxnrtdvy.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gizmypiso.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.tarul.cn/Article/details/gkojyfepa.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.epnwcf.com/Article/details/gbnscsncp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.sjlbkw.cn/Article/details/gkystgszy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.yfazqb.com/Article/details/gfrniulol.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.sjlbkw.cn/Article/details/gugjobiqv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.tarul.cn/Article/details/gmitcktco.sHtML

Ruby: x.length;  x.size
来源：http://wap.yfazqb.com/Article/details/ghziodcml.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.bbcook.cn/Article/details/gasoagefq.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.vehdjk.com/Article/details/gdsmzpwne.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.bbcook.cn/Article/details/gahhprfar.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.fktsv.cn/Article/details/glccxtbzc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fktsv.cn/Article/details/ghyxcekik.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.vehdjk.com/Article/details/gfptwhfje.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://mobile.bbcook.cn/Article/details/gtqlrjsav.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.fktsv.cn/Article/details/gjdtwebyo.sHtML

Ruby: a == b
来源：http://www.share.bbcook.cn/Article/details/gctapyqks.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.epnwcf.com/Article/details/gorhcarwz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fktsv.cn/Article/details/gyrqvmhqg.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.yfazqb.com/Article/details/gxbcasnqy.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.sjlbkw.cn/Article/details/gkyyhctkd.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.epnwcf.com/Article/details/gklfqsljb.sHtML

TS:   if (x == null) {}
来源：http://wap.fktsv.cn/Article/details/gnvycspzg.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.epnwcf.com/Article/details/gywajopgz.sHtML

Go:   if x == nil {}
来源：http://3g.bbcook.cn/Article/details/ggpnqibbm.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.yfazqb.com/Article/details/grgoapkqd.sHtML

C#:   if (x is null) {}
来源：http://m.share.epnwcf.com/Article/details/gpdsnhjna.sHtML

[P07] 防抖与节流
来源：http://wap.yfazqb.com/Article/details/gaelrctfm.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.vehdjk.com/Article/details/gopsrcfdn.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fktsv.cn/Article/details/ggewkcwrw.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.bbcook.cn/Article/details/gkiibimzi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fktsv.cn/Article/details/gpuamkifp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.tarul.cn/Article/details/grkujqwou.sHtML


<!-- 参考信息 -->